# Tool 01 — AI Visibility Rank Checker

**Status:** Ship-ready spec
**Priority:** First tool to ship (MVP)
**Engineering estimate:** 8-10 days (if rank checker core exists) or 15-20 days (from scratch)
**Related docs:** `../03-content-plan.md`, `../04-free-tools.md`, `../07-measurement-framework.md`

---

## One-sentence scope

User enters a domain → gets AI visibility score across 4 engines + competitor comparison + 3 authority signals → email-gated full report → upgrade path to paid product.

---

## Scope boundaries

### ✅ IN SCOPE

**Core rank checking:**
- Domain input (single field)
- Auto-detect category from domain content
- Auto-detect 2-3 competitors from category
- Run 5 predefined queries across 4 AI engines
- Parse responses for brand citations
- Calculate AMQ Score (0-100)
- Display rank vs competitors

**3 light authority flags:**
- Wikipedia presence (yes/no)
- G2 listing (yes/no)
- Domain age (years, from WHOIS)

**Results + conversion:**
- Partial free results (score + binary flags)
- Email gate for full report
- Shareable result URL
- Upgrade CTA to paid product

### ❌ OUT OF SCOPE (defer to Tool 2+ or paid tier)

- Auth domain deep-dive (Reddit counts, YouTube, Quora) → paid tier
- Technical site audit (AI crawler access, schema, SSR) → Tool 2
- Blog-level content audit → Tool 3 (Month 4-5)
- Custom query input → paid tier
- Historical tracking → paid tier
- Multi-brand tracking → paid tier
- Alert system → paid tier
- Mobile app → never (web only)

---

## Component Architecture

### 1. Landing Page

**URL:** `answermonk.ai` or `/tools/ai-visibility`

**Hero:**
- H1: "See where your brand ranks in AI answers"
- Sub: "Free check across ChatGPT, Claude, Perplexity, and Google AI Mode. No signup required."
- Input field: domain URL
- Primary CTA: "Check my AI visibility"

**Below fold:**
- 3-step "how it works" explainer
- Sample result screenshot (anonymized)
- FAQ (5 questions harvested from PAA)
- Trust signals (as accumulated)

**Technical requirements:**
- Meta title, description, OG tags
- SoftwareApplication schema
- Server-rendered (SSR)
- Mobile responsive
- Core Web Vitals compliant
- FAQPage schema for FAQ

### 2. Input Validation

- URL format check (must be valid domain)
- Normalize: strip `http://`, `https://`, `www`, trailing slashes → root domain
- Reject invalid inputs with friendly error message
- Rate limit: 5 checks per IP per hour

### 3. Category Auto-Detection

**Input:** Normalized domain URL

**Process:**
- Fetch homepage HTML
- Extract: `<title>`, meta description, H1, first 500 words of visible text
- Send to LLM (Claude or GPT): "What B2B SaaS category does this belong to? Return one: SaaS Marketing, SaaS Sales, SaaS Analytics, CRM, E-commerce, Content Platform, etc."
- Store in session

**Fallback:** If LLM fails, default to "B2B SaaS" generic
**Cost:** ~$0.01 per detection

### 4. Competitor Auto-Detection

**Input:** Category

**Process:**
- Query LLM: "Top 3 [category] brands by mention frequency in AI search"
- Or use pre-built category → competitor mapping table
- Or let user override with manual input (optional field)

**Output:** 2-3 competitor domains

**Fallback:** Top 3 well-known brands per category (maintained list)

### 5. Query Generation

**Input:** Category

**Process:** 5 pre-built query templates per category

Example for SaaS Marketing:
- "Best email marketing platform for SaaS"
- "Best marketing automation for B2B"
- "Top marketing tools for startups"
- "Best alternatives to HubSpot"
- "AI-powered marketing tools 2026"

**Output:** 5 query strings

**Maintenance:** Review + refresh query templates quarterly

### 6. Multi-Engine Query Execution

For each of 5 queries, query all 4 engines in parallel:

**ChatGPT:**
- OpenAI API with browsing enabled
- Extract brand mentions from response

**Claude:**
- Anthropic API
- Extract brand mentions

**Perplexity:**
- Perplexity API
- Extract brand mentions

**Google AI Mode:**
- SerpAPI or DataForSEO for SERP scraping
- Detect AI Overview presence
- Extract cited domains from AI Overview

**Rate limiting:**
- Parallel execution with 30s timeout
- Retry once on failure
- Graceful degradation if one engine fails

**Cost per check:**
- OpenAI (GPT-4): ~$0.10
- Claude: ~$0.05
- Perplexity: ~$0.05
- SerpAPI: ~$0.05
- **Total: ~$0.25 per check**

### 7. Response Parsing

For each AI response:
- Extract mentioned brands (regex + entity recognition)
- Determine position (1st mentioned, 2nd, buried, not cited)
- Classify sentiment (positive recommendation, neutral, negative)
- Store structured result

**Logic per brand:**
- User's brand: citation count + position + sentiment across 5 queries × 4 engines
- Each competitor: same analysis
- "Other brands cited" overall count

### 8. AMQ Score Calculation

**Formula:**
```
AMQ Score = (
  Citation Frequency × Position Weight × 
  Engine Coverage × Sentiment
) × 100
```

**Variable definitions:**
- **Citation Frequency:** citations / total_queries (max 20 queries = 5 queries × 4 engines)
- **Position Weight:** 1.0 (1st mention), 0.7 (2nd), 0.4 (3rd+), 0.1 (buried)
- **Engine Coverage:** % of 4 engines where cited (0.25 per engine)
- **Sentiment:** 1.0 (positive), 0.8 (neutral), 0.3 (negative)

**Output:** Integer 0-100

**Benchmark comparison:**
- Show vs category average (from AnswerMonk aggregate data)
- Show vs top competitor
- Percentile rank within category

### 9. Authority Signal Checks (3 flags)

**Flag 1: Wikipedia Presence**
- API: MediaWiki `action=query&titles=[brand]`
- Response: page exists (yes/no)
- Build time: 30 min
- Cost: Free

**Flag 2: G2 Listing**
- Check: `g2.com/products/[normalized-brand-name]` returns 200
- Or scrape: `g2.com/search?query=[brand]` for exact match
- Response: page exists (yes/no)
- Build time: 1 hour
- Cost: Free (light scraping) or ~$0.01 (SerpAPI)

**Flag 3: Domain Age**
- API: WHOIS via RDAP or WhoisXML API
- Response: registration date → calculate years
- Build time: 1 hour
- Cost: ~$0.001 (WhoisXML) or free (RDAP with rate limits)

**UI presentation:**
- Compare across user + competitors in simple table
- Show "You have this" vs "You don't have this"

### 10. Result UI

**Score card (top):**
```
┌─ Your AMQ Score ────────────┐
│                             │
│         58/100              │
│    (industry avg: 42)       │
│                             │
│  Cited in 2 of 4 engines   │
└─────────────────────────────┘
```

**Engine breakdown:**
```
ChatGPT:     ✓ Cited (2nd position)
Claude:      ✗ Not cited
Perplexity:  ✓ Cited (3rd position)
Google AI:   ✗ Not cited
```

**Competitor comparison table:**
```
                 You    Competitor A  Competitor B
AMQ Score        58     78            65
ChatGPT          ✓      ✓             ✓
Claude           ✗      ✓             ✗
Perplexity       ✓      ✓             ✗
Google AI        ✗      ✓             ✓
Wikipedia        ✗      ✓             ✓
G2 listing       ✓      ✓             ✓
Domain age       3y     8y            5y
```

**One-line insight:**
"You're cited half as often as Competitor A. Key gaps: Claude visibility, Wikipedia presence, brand authority age."

**Primary CTA:**
"Want the full report + competitor deep-dive? Enter your email →"

### 11. Email Gate

**Free (visible before email):**
- AMQ Score
- 4-engine citation status (binary)
- Competitor comparison (3 brands)
- 3 authority flags
- One-line insight

**Gated (requires email):**
- Full 5-query breakdown per engine
- Citation text/context from each AI response
- Detailed competitor analysis (what they cite, when)
- Industry percentile data
- Downloadable PDF report
- 14-day free trial of paid product

**Email capture flow:**
- Simple form: email + company (optional)
- GDPR compliance: clear opt-in
- Single opt-in (no double opt-in needed for US SaaS)
- Redirect to full report page after submission
- Send confirmation email with report + trial CTA

### 12. Nurture Email Sequence

| Day | Subject | Focus |
|---|---|---|
| 0 | Full report delivered | Value + "See how to improve" |
| 2 | 3 quick wins to boost your AMQ score | Actionable tips |
| 5 | How [notable brand] went from 32 to 78 AMQ | Case study |
| 8 | Your competitors are moving — stay ahead | Urgency |
| 12 | Try AnswerMonk Pro free for 14 days | Hard conversion |

**Platform:** Loops, Resend, or ConvertKit
**Conversion target:** 5-10% email → trial signup

### 13. Shareability

**Share mechanism:**
- Unique result URL per check: `answermonk.ai/results/[hash]`
- Pre-generated OG image for each result (LinkedIn/Twitter preview)
- Pre-formatted share copy:
  - LinkedIn: "I just checked our AI visibility score — we're at 58/100. Interesting what's broken..."
  - Twitter: "Our AMQ Score: 58/100. Cited in 2 of 4 AI engines. What's yours? [link]"

**Strategic rationale:**
- Sieve [P:7115]: intrinsic virality via two-sided benefit
- Users tag competitors, share scores
- Every share = organic acquisition channel

### 14. Analytics Events

Track these in GA4 / Mixpanel:

| Event | Trigger |
|---|---|
| `tool_landing_view` | User loads landing page |
| `tool_check_started` | User clicks "Check" |
| `tool_check_completed` | Results displayed |
| `tool_email_captured` | Email submitted |
| `tool_result_shared` | User shares result URL |
| `tool_trial_clicked` | User clicks "Start free trial" |
| `tool_trial_signed_up` | User completes trial signup |
| `tool_pro_converted` | User converts to paid |

**Funnel visualization:**
```
Landing → Check started → Check completed → 
Email captured → Trial clicked → Trial signed up → Paid
```

### 15. Infrastructure

**Backend:**
- Existing AnswerMonk core API (extend existing endpoints)
- Wrapper endpoint: `/api/free-tool/rank-check`
- Rate limiting middleware
- Caching layer (Redis or Supabase): 24h TTL per domain

**Frontend:**
- Next.js on Vercel (matches existing stack)
- Server-rendered for SEO
- Tailwind for styling

**Database:**
- Supabase (existing stack)
- Tables:
  - `free_tool_checks` (domain, results, timestamp, user_id if email captured)
  - `domain_cache` (domain, category, competitors, cached_at)

**Email:**
- Loops or Resend for transactional + nurture
- Webhook from check completion → trigger email sequence

**External APIs:**
- OpenAI (ChatGPT browsing)
- Anthropic (Claude)
- Perplexity
- SerpAPI (Google AI Mode detection)
- MediaWiki (Wikipedia)
- WhoisXML (domain age)

**Cost per check:** ~$0.25

---

## Engineering estimate

### Phase 1: Enhance existing rank checker to ship-ready (5-7 days)

- Add category auto-detection (1 day)
- Add competitor auto-detection (1 day)
- Add 3 authority flags (1 day)
- Improve result UI (2 days)
- Email capture + nurture setup (2 days)

### Phase 2: Polish + launch prep (3 days)

- Shareability + OG image generation (1 day)
- Analytics events (1 day)
- QA across browsers + edge cases (1 day)

### Total

- **If rank checker core exists:** 8-10 days
- **If starting from scratch:** 15-20 days

---

## UX Flow

```
1. Landing page
   └─> User enters domain
       └─> 2. Progress screen (30-45s)
           ├─> Detecting category...
           ├─> Finding competitors...
           ├─> Querying ChatGPT...
           ├─> Querying Claude...
           ├─> Querying Perplexity...
           ├─> Querying Google AI Mode...
           ├─> Checking Wikipedia...
           ├─> Checking G2...
           ├─> Checking domain age...
           └─> Computing AMQ Score...
           
3. Partial results (free, no email required)
   ├─> AMQ Score + engine breakdown
   ├─> Competitor comparison
   ├─> 3 authority flags
   └─> "Get full report" CTA
       └─> 4. Email gate
           └─> User submits email
               └─> 5. Full results page
                   ├─> Full query-by-query breakdown
                   ├─> Competitor deep-dive
                   ├─> Industry benchmark
                   └─> "Try AnswerMonk Pro" CTA
                       └─> 6. Paid product trial signup
```

---

## Launch Checklist

### Pre-launch (Week 1)

- [ ] All components built + tested
- [ ] 10 real-domain test checks run (verify output quality)
- [ ] Rate limiting tested
- [ ] Email nurture sequence configured
- [ ] Analytics events firing correctly
- [ ] Mobile responsive verified
- [ ] Meta tags + schema validated
- [ ] Shareable URLs tested (OG preview)
- [ ] Error states designed (API failures, invalid inputs)
- [ ] Privacy policy + ToS updated

### Launch day (Day 0)

- [ ] Landing page deployed to production
- [ ] G2 AEO Insights category submission
- [ ] 5 AI tool directory submissions
- [ ] Founder LinkedIn launch post
- [ ] ProductHunt launch
- [ ] Reddit r/SideProject + r/SaaS posts
- [ ] Email blast to existing waitlist
- [ ] Twitter/X launch thread
- [ ] 10 personalized DMs to target ICP

### Week 1 post-launch

- [ ] Daily engagement on LinkedIn (respond to comments)
- [ ] Track all funnel metrics
- [ ] Monitor API costs vs usage
- [ ] Gather user feedback (first 50 users)
- [ ] Iterate on pain points

---

## Success Criteria (Day 30)

- [ ] 500+ checks run
- [ ] 250+ emails captured (50% capture rate)
- [ ] 10+ social shares
- [ ] 5+ trial signups
- [ ] 2+ paying customers from tool
- [ ] 1+ inbound press/mention
- [ ] Average check completion rate >70%
- [ ] No critical bugs

**If targets hit:** proceed to Tool 2 (AEO Tech Audit) build
**If targets missed:** diagnose (landing page conversion, check quality, email sequence) before building more

---

## Scope Creep Anti-Patterns (explicit DO NOT add)

- ❌ Historical tracking → paid feature, creates ongoing infrastructure burden
- ❌ Custom query input → users abuse, increases cost, reduces comparison quality
- ❌ More than 3 authority flags → eats into paid product value
- ❌ Continuous monitoring → THIS IS the paid product
- ❌ Multi-brand tracking → enterprise feature
- ❌ API access → enterprise feature
- ❌ White-label option → enterprise feature
- ❌ Custom reports → bloats MVP
- ❌ Advanced sentiment analysis → Pro tier depth
- ❌ Citation context quotes → makes free too useful, weakens paid

**The discipline:** Free tool shows you're missing value. Paid product delivers the value.

---

## Dependencies

### Must be live before launching Tool 1

- [ ] AnswerMonk core product backend (rank checking engine exists)
- [ ] Supabase DB configured
- [ ] Domain: `answermonk.ai` live with SSL
- [ ] Paid product tier available (trial signup path must work)
- [ ] Email platform connected (Loops/Resend)
- [ ] OpenAI, Anthropic, Perplexity, SerpAPI accounts + API keys
- [ ] Privacy policy + ToS pages

### Nice-to-have (but not blocking)

- [ ] Analytics platform beyond GA4 (Mixpanel/Amplitude)
- [ ] Customer support chat (Intercom, Crisp)
- [ ] Cookie consent banner (if targeting EU)

---

## Decision Gates

### Ship now IF

- Rank checker core is working
- 5-7 days available for enhancements (or 15-20 if starting fresh)
- Email infrastructure ready
- 10 test domains produce quality output
- Paid product trial flow works end-to-end

### Delay IF

- API cost structure unclear
- Paid product not yet ready (tool generates leads with nowhere to send them)
- Rank checker core has reliability issues
- Legal/compliance review pending

**If ready:** ship in 7-10 days. Start distribution immediately after.

---

## Integration with broader GTM plan

This tool is **Tool 2 in `../04-free-tools.md` (AMQ Score Calculator)** expanded to include:
- Category auto-detection
- Competitor auto-detection
- 3 authority flags
- Full result visualization

It replaces the previously-planned standalone AMQ Score Calculator with a more comprehensive rank-checker experience. The AMQ Score IS the score produced — just with richer context (engines, competitors, authority flags).

**Next tool to build after this:** Tool 2 — AEO Technical Audit (AI crawler access, schema, SSR, llms.txt). See future `tools/02-aeo-tech-audit-spec.md`.

---

## Cost projection (first 30 days)

Assuming 500 checks in Month 1:
- API costs: 500 × $0.25 = **$125**
- Email service: **$30-50/mo**
- Hosting (Vercel + Supabase): **$50-100/mo**
- Total Month 1 infrastructure: **~$200-275**

Revenue target (Month 1):
- 2+ paid customers × $149 = **$298+ MRR**
- Breakeven on Month 1 even at conservative targets

**Scale math (Month 3):**
- 5,000 checks → $1,250 API
- 30 paid customers × $149 = $4,470 MRR
- Gross margin: ~72%

---

## Maintenance plan (post-launch)

### Weekly
- Monitor API costs vs check volume
- Review error rates per engine
- Update category → query templates if new trends emerge

### Monthly
- Analyze email → trial conversion funnel
- Review category detection accuracy (sample 20 random checks)
- Refresh competitor benchmark data

### Quarterly
- Review query templates per category
- Update authority flag logic (new signals to add?)
- Consider expansion to more engines (Gemini, Grok, Mistral)

---

## One-line scope

**Domain → 5 queries × 4 engines → AMQ Score + competitor comparison + 3 authority flags → email gate → full report → upgrade path.**

Nothing else. Everything else waits for Tool 2+.
