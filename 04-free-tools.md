# 04 — Free Tools

**Purpose:** 3 free tools that drive top-of-funnel awareness, capture emails, and convert to paid product.
**Pattern:** HubSpot Website Grader / Ahrefs Free Tools — the proven B2B SaaS category-creation play.

---

## Strategy

### What free tools are for
- Top-of-funnel traffic (SEO + social virality)
- Email capture (gated "full report")
- Demonstration of product value (compressed into a single check)
- Link magnets (tools attract backlinks organically)
- Category education (each tool teaches AEO concepts)

### What free tools are NOT
- Permanent free product tier (Sieve [PB:437] warns against this)
- Replacement for paid product
- Unlimited queries / no limits

### The conversion path (every tool uses this)
```
Tool discovered (organic, social, referral)
  → User runs check (URL input, 30 sec)
  → Instant partial result shown (the hook)
  → Email gate for "full report" (60-day historical, recommendations, competitor data)
  → Email captured → nurture sequence (5 emails over 10 days)
  → Trial signup CTA (14-day free Starter tier)
  → Paid conversion ($149/mo+)
```

### Cadence
- **Tool 1:** Ship Week 2-3
- **Tool 2:** Ship Week 3 (AMQ Score — dual role as content + tool)
- **Tool 3:** Ship Weeks 9-10 (post-launch, drives second growth wave)

---

## Tool 1: AI Crawler Access Checker

**URL:** `/tools/ai-crawler-checker`
**Also accessible from:** `/free-tools` hub page

### What it does
User enters a domain → tool checks if major AI crawlers are blocked via robots.txt.

### Crawlers checked
- GPTBot (OpenAI)
- ChatGPT-User (OpenAI browsing)
- Google-Extended (Google AI training)
- Claude-Web (Anthropic)
- Claude-User (Anthropic chat)
- PerplexityBot (Perplexity)
- CCBot (Common Crawl)
- Bytespider (ByteDance / Doubao)
- anthropic-ai (alternative Anthropic agent)

### User flow
1. Landing page: Simple hero with input field — "Check if AI can crawl your website"
2. User enters domain → click "Check"
3. Instant result (~2 seconds): Pass/fail for each crawler
4. "Want the full audit?" → Email gate → Full report delivered (includes remediation code snippets)

### Free vs gated

**Free (no email):**
- Shows pass/fail for all 9 crawlers
- Generic remediation advice

**Gated (email captured):**
- Remediation code specific to detected CMS
- Full robots.txt analysis
- llms.txt status check
- Schema markup presence check
- Downloadable PDF report
- Entry into nurture sequence

### Engineering estimate
- Backend: 2 days (robots.txt parser + CMS detection)
- Frontend: 2 days (landing + result page + email capture)
- Design: 1 day (visual result card with pass/fail icons)
- **Total: 5 days**

### SEO positioning
- Primary keyword: "is gptbot blocked" (target KD < 10)
- Secondary: "ai crawler check", "robots.txt ai", "check ai access"
- Content: H1 "Check If AI Can Crawl Your Website" + explanation of each crawler

### Distribution day-1
- LinkedIn post (founder): "Built a free tool to check if ChatGPT can crawl your site. 40%+ of sites I tested are accidentally blocking AI"
- ProductHunt launch (Saturday — higher up-vote weight)
- Reddit: r/SEO, r/SaaS (with add-value first, then share tool)
- Submit to AI tool directories

### Conversion target
- 5-10% of unique visitors use the tool
- 40-60% of tool users give email for full report
- 3-5% of emails convert to free trial within 60 days

### Viral mechanic
"We block GPTBot by mistake" is an embarrassing-but-common discovery. Users share it on LinkedIn/Twitter with "Just ran this on our site — we were blocking ChatGPT. Fixed." Each share = organic distribution.

---

## Tool 2: AMQ Score Calculator

**URL:** `/amq-score` (also lives as a content page — see `03-content-plan.md` Page 6)
**Also accessible from:** `/free-tools` hub page

### What it does
User enters a domain → tool runs a compressed version of the AnswerMonk measurement against that domain.

### Calculation
AMQ Score = (Citation Frequency × Position Weight × Engine Coverage × Sentiment) × 100

Score range: 0-100

Benchmarks (computed from AnswerMonk's aggregate product data across 500+ B2B SaaS brands):
- 0-20: Invisible to AI
- 21-40: Below average (bottom 25%)
- 41-60: Average (B2B SaaS typical)
- 61-80: Strong (top 25%)
- 81-100: Category leader (top 5%)

### User flow
1. Landing page with interactive calculator
2. User enters domain + selects category (dropdown: SaaS, E-commerce, Media, etc.)
3. 30-60 second "scan in progress" with progress indicators
4. Tool runs ~10-20 queries across 4 AI engines in background
5. Instant score + comparison to category benchmark
6. Email gate for "full report" + "3 actionable recommendations"

### Free vs gated

**Free (no email):**
- AMQ Score number (0-100)
- Category benchmark comparison
- 1 top-line insight ("Your score is [X] points below category average")

**Gated (email captured):**
- Full 20-query citation data across 4 engines
- Competitor AMQ Scores (up to 3 competitors auto-detected)
- 3 specific recommendations to improve
- Historical tracking opt-in
- PDF report

### Engineering estimate
- Backend: 4 days (wraps existing AnswerMonk citation engine, limits to 20 queries)
- Frontend: 3 days (calculator widget + result dashboard)
- Design: 2 days (polished score reveal animation)
- **Total: 9 days**

### SEO positioning
- Primary keyword: "search visibility score" (450, KD 20)
- Secondary: "ai visibility score", "measure ai visibility", "brand ai citation rate"
- Content: comprehensive explanation of the formula, industry benchmarks, methodology

### Distribution day-1 + ongoing
- **Founder day-1:** DM 15 B2B SaaS / SEO influencers on LinkedIn — "built this based on your feedback, want to try?"
- **LinkedIn post:** Thread showing scores for 10 well-known B2B SaaS brands (HubSpot: 82, Semrush: 78, etc.)
- **PRNewswire:** Short announcement ("AnswerMonk launches first industry standard for AI visibility measurement")
- **Ongoing:** Category reports quarterly ("The State of AI Visibility in B2B SaaS — AMQ Scores for top 500 brands")

### Conversion target
- Higher than Tool 1 (specific score creates commitment)
- 60-75% of tool users give email for full report
- 10-15% of emails convert to trial within 60 days

### Moat mechanism
Once "AMQ Score" enters the category vocabulary (projected: 6-12 months), every writer / consultant discussing AI visibility must reference it. Competitors must either (a) adopt the metric, giving AnswerMonk attribution, or (b) invent their own, fragmenting the market.

---

## Tool 3: Google vs ChatGPT Audit

**URL:** `/tools/google-vs-chatgpt`
**Also accessible from:** `/free-tools` hub page

### What it does
User enters a domain + category → tool runs identical queries in Google and ChatGPT, shows side-by-side ranking comparison.

### User flow
1. Landing page: Headline "See the gap between your Google rankings and ChatGPT citations"
2. User enters domain + selects category
3. Tool generates 4 category-specific queries (e.g., "best [category]", "[category] for [use case]", etc.)
4. Runs them in Google (top 10 results) and ChatGPT (cited brands)
5. Shows side-by-side comparison: where do you rank in each?
6. Highlights the "gap" — brands in Google top 10 but NOT in ChatGPT response

### Free vs gated

**Free (no email):**
- 1 query's worth of side-by-side comparison
- Summary stat: "You rank [X] on Google, cited [Y] times in ChatGPT"

**Gated (email captured):**
- Full 4-query comparison
- Competitor data (brands that appear in both vs one)
- Gap analysis report
- PDF with screenshots (shareable)

### Engineering estimate
- Backend: 5 days (Google search API integration + ChatGPT integration via own product)
- Frontend: 4 days (comparison UI)
- Design: 3 days (polished side-by-side visualization)
- **Total: 12 days**

### SEO positioning
- Primary: "google vs chatgpt", "chatgpt vs google search"
- Secondary: "ai search vs google", "chatgpt rankings"
- Content: Comprehensive explainer of the gap + why it matters

### Distribution day-1
- Paired with flagship study: "We analyzed X B2B brands — the Google-ChatGPT gap is [stat]"
- LinkedIn: viral carousel post (we drafted this in earlier TRYPS-adjacent work)
- Tier-1 PR pre-brief: "First-of-its-kind Google vs ChatGPT visibility audit"

### Conversion target
- Highest of the 3 tools (most dramatic result, highest "wow" factor)
- 70-80% email capture rate
- 15-20% trial conversion within 60 days

### Positioning vs competitors
This is the tool that distinguishes AnswerMonk most clearly from Profound. Profound focuses on "AI answers only" — AnswerMonk explicitly compares across both surfaces (Google + AI).

---

## The Free Tools Hub

**URL:** `/free-tools`

**Purpose:** Central page listing all free tools. Individual tool URLs can also be linked directly.

**Structure:**
- H1: "Free AI Visibility Tools"
- Brief intro (50 words)
- Card layout with 3 tools:
  - AI Crawler Access Checker
  - AMQ Score Calculator
  - Google vs ChatGPT Audit
- Each card: Icon + 1-sentence description + "Run free check →" button
- Below: "Want continuous tracking? Try AnswerMonk Pro →"

**Schema:** ItemList + SoftwareApplication for each

---

## Tools NOT to build (explicit kills)

### ❌ AEO-Optimized Blog Writer
**Why not:** Competes with Clearscope, MarketMuse, Surfer SEO (different category). Dilutes AnswerMonk's "tracking + measurement" positioning.

### ❌ AEO Audit Tool (full site audit)
**Why not:** Commoditized by Screaming Frog, Sitebulb, ScreamingFrog. Our Crawler Checker captures the AEO-specific slice.

### ❌ Keyword Research Tool
**Why not:** Semrush / Ahrefs' home turf. Not AEO-specific enough.

### ❌ Rank Checker (traditional)
**Why not:** Not category-defining. Generic.

### ❌ Schema Generator
**Why not:** Schema.org already has tools; we'd be building to commodity.

### ❌ Competitor Analyzer (standalone)
**Why not:** This is a product feature, not a tool. Should be paywalled.

---

## Free tool measurement

### Per tool, track weekly:
- Unique visitors to tool landing page
- Tool runs (completions)
- Email captures
- Email-to-trial conversion rate
- Trial-to-paid conversion rate
- LinkedIn/social shares
- Inbound backlinks (Ahrefs)

### Aggregate metrics:
- Total free tool users/month
- Email list growth from tools
- Top-performing tool by conversion
- Organic traffic to /tools/ pages

### Kill criteria (per tool):
- <100 runs/month after 60 days → diagnose distribution
- <5% email capture rate → rewrite the gating copy
- 0 backlinks after 90 days → diagnose PR distribution

---

## Free tools → paid product conversion funnel

```
Week 1-2: Ship Tool 1 (AI Crawler Checker)
  → Drives 1-2K monthly visitors by Week 6
  → 40-60% give email → 500-1,200 emails/month

Week 3: Ship Tool 2 (AMQ Score)
  → Drives 3-5K monthly visitors by Week 10
  → 60-75% give email → 2,000-3,500 emails/month
  → Higher commercial intent (users see a score, want to improve it)

Week 9-10: Ship Tool 3 (Google vs ChatGPT Audit)
  → Viral potential
  → Tier-1 PR opportunity

Month 3+: 5,000+ emails in the list
  → 3-10% convert to paid trial → 150-500 trials
  → 15-25% of trials convert to paid → 25-125 paid customers
  → At $149-499/mo average → $4K-50K MRR from free tools alone
```

---

## Free tool branding rules

1. Each tool should feel like a standalone mini-product, not a marketing asset
2. URL structure: `/tools/[tool-name]` (not `/free-tools/[tool-name]`)
3. Design should be on par with the paid product (signal quality)
4. CTA to paid product: subtle, not aggressive
5. Tool results should be shareable (public URLs for each result, with AnswerMonk branding)
6. All tools must work on mobile (60%+ of tech content is consumed mobile)
7. Every tool needs: loading state, error state, empty state, result state
8. Accessibility: WCAG 2.1 AA compliance

---

## Compliance + legal

- Tools query third-party sites (via public APIs or public data) — no auth needed
- Email capture: GDPR-compliant (double opt-in for EU users)
- Privacy policy + terms updated for tool usage
- Rate limiting: 5 runs per IP per hour (prevent abuse)
- Cache results for 24h per URL (reduce duplicate queries)

---

## Next steps for tool development

### Week 1 (pre-launch of any tool)
- [ ] Finalize branding for /tools/ namespace
- [ ] Design system: tool result card template
- [ ] Engineering: rate limiting + caching infrastructure
- [ ] Analytics: event tracking (tool start, tool complete, email capture, conversion)

### Before Tool 1 ships (Week 2)
- [ ] robots.txt parser tested on 50 real sites
- [ ] UX tested with 5 target customers
- [ ] Email capture flow connected to CRM / mail service
- [ ] Landing page copy reviewed against blog rules
- [ ] Schema.org markup for SoftwareApplication

### Before Tool 2 ships (Week 3)
- [ ] AMQ Score formula locked (peer-reviewed by founder + 2 advisors)
- [ ] Benchmark data computed from product (500+ brand sample)
- [ ] Full report template designed
- [ ] Influencer seed list prepped (15 names, LinkedIn DMs ready)

### Before Tool 3 ships (Week 9-10)
- [ ] Google search API budget set ($200-500/mo)
- [ ] Product-level integration validated
- [ ] Tier-1 press pre-brief list prepped

---

## Summary

**3 tools in 12 weeks:**

| Tool | Ship week | Engineering effort | Primary conversion path |
|---|---|---|---|
| AI Crawler Checker | Week 2 | 5 days | Email capture → trial → Starter |
| AMQ Score Calculator | Week 3 | 9 days | Email capture → trial → Starter/Pro |
| Google vs ChatGPT Audit | Week 9-10 | 12 days | Email capture → trial → Pro |

**Total engineering: ~26 days** (solo) or **10 days** (parallel team of 3)

**Expected outcome by Day 90:**
- 5,000+ emails in nurture list
- 150-500 trial signups
- 25-125 paying customers
- $4K-50K MRR from tools-driven acquisition alone
