# Proposal: Driving 10% AI Appearance Rate + Organic Traffic Growth for Valeo Health

**Prepared for:** Sundeep — Valeo Health (feelvaleo.com)
**Prepared by:** Arun Sharma
**Date:** 2026-04-23
**Timeline:** 3 months (12 weeks), starting week of 2026-04-28
**Basis:** SEO + AEO + GEO Audit of feelvaleo.com (2026-04-14)

---

## Executive Summary

**Valeo Health has done the hard work of brand-building. The domain ranks #2 on Google for "best at home blood test Dubai UAE lab service". Trustpilot, App Store, and Dubai Review directory listings exist. The brand's Brand AI Presence score is 75% — one of the strongest in the GCC healthcare space.**

**Yet the current AI appearance rate (citations across ChatGPT, Claude, Perplexity, Google AI Mode) is estimated at under 2% for category queries.**

The gap isn't brand. It's **architecture**. The canonical root page (`feelvaleo.com`) is a 106-word language/country splash gateway that AI crawlers cannot navigate through. The actual content (2,677 words) lives at `/en-ae/dubai` but AI engines only see the splash. That one architectural decision is costing Valeo roughly 95% of its AI citation potential.

**This proposal:** a 12-week program to reach **10% appearance rate across 4 AI engines** and drive **40-60% increase in organic traffic** through four connected workstreams:

1. **Foundation Fix** (Weeks 1-3) — Replace the splash gateway with a real content page at the root; port enhanced schema; fix technical anti-patterns.
2. **Schema + E-E-A-T** (Weeks 4-6) — Medical director credentials, DHA licensing visible, AggregateRating from Trustpilot, FAQPage schema sitewide.
3. **Content Production** (Weeks 7-10) — City × service matrix expansion, competitor gap content, featured-snippet-optimized FAQ clusters.
4. **Authority + Monitoring** (Weeks 11-12) — Trustpilot integration, press outreach, ongoing measurement framework.

**Expected outcome by Week 12:**
- AI appearance rate: 2% → **10-12%**
- Organic traffic: +40-60% (driven by Fix #1 alone)
- Page Citation Readiness: 55% (F) → **85% (B+)**
- Citation rank: Valeo in top 3 cited sources for category queries in ChatGPT / Perplexity

---

## The Diagnosis (from the April 14 audit)

### What's working
- **Brand AI Presence: 75% (B-)** — Strongest in category
- SERP position #2 for "best at home blood test Dubai"
- Massive sitemap coverage (6,705 URLs across 4 countries × 2 languages)
- Trustpilot + App Store + Dubai Review directory presence
- Explicit AI bot allowances (GPTBot, ClaudeBot, PerplexityBot, OAI-SearchBot, Google-Extended)
- Next.js SSR (content IS in raw HTML, not JS-dependent)
- Clean technical SEO fundamentals (TTFB 602ms, HTTP/2, CDN)

### What's broken (ranked by impact)

| # | Problem | Current | Target | Impact |
|---|---|---|---|---|
| 1 | **Root page is a 106-word splash gateway** | 5% AEO Extraction | 85%+ | CATASTROPHIC |
| 2 | No MedicalBusiness / LocalBusiness schema on root | 2 schema blocks | 6+ blocks | CRITICAL |
| 3 | Dynamic `dateModified` (cosmetic timestamp) | Re-stamped every fetch | Real content timestamp | HIGH |
| 4 | No AggregateRating schema (despite Trustpilot existing) | None | Trustpilot-derived | HIGH |
| 5 | No medical director / founder Person schema | None | Both with credentials | HIGH |
| 6 | 0 FAQ pairs on root (SKIN111 has 5) | None | 6-8 pairs | HIGH |
| 7 | DHA license not visible on root | Present at `/en-ae/dubai` only | Present on root | HIGH (YMYL) |
| 8 | Missing HSTS header | None | 2-year preload | MEDIUM (security + trust) |
| 9 | Cache-Control too aggressive for CDN caching | `no-store` | `s-maxage=3600` | MEDIUM |
| 10 | Logo plain URL (not ImageObject with dimensions) | String | Full ImageObject | LOW |

### The single biggest gap

Content depth at root: **106 words vs SKIN111's 2,000-2,500 words (20x less)**.

Implementing Fix #1 alone (serve real content at root, not splash) pushes AEO Extraction from 5% to ~85% and Selection from 17% to ~75% — because the content already exists at `/en-ae/dubai`. It just needs to be the default root experience, not something users have to "select their way into".

---

## The Opportunity

### Why 10% appearance rate is realistic

**Baseline comparison (audited this session):**

| Brand | Brand AI Presence | Page Citation Readiness | Current Appearance Rate |
|---|---|---|---|
| TRYPS (pre-launch SaaS) | 12% | 15% | ~0% |
| AnswerMonk (pre-launch SaaS) | 0% | 10% | 0% |
| **Valeo Health** | **75%** | **55%** | **~2%** (estimated) |

**Valeo is in a different league on brand strength.** The brand already has:
- SERP authority (#2 for category)
- Third-party validation (Trustpilot, App Store, Dubai Review)
- Social presence (4 sameAs)
- Multi-country operation
- Real-world regulatory positioning (DHA licensed)

The 10% target is **realistic because the brand is pre-positioned**. What's missing is page-level citation-readiness — which is 100% under Valeo's control and fixable in weeks, not months.

### Why traffic growth will compound

Three independent traffic levers stack:

**Lever 1: Architectural fix captures existing demand**
Currently, the root page ranks #2 but delivers 106 words of "select language". Many users bounce. A proper content page at root captures the same SERP traffic at a higher conversion rate.

**Lever 2: AI citations drive direct referral traffic**
Perplexity, ChatGPT (with browsing), and Google AI Mode all include source citations. When Valeo is cited, users click through. Estimate: 0.5-2% of AI-cited-users click the source.

**Lever 3: AI citations drive branded search**
Users who see Valeo mentioned in AI answers later Google the brand. Branded search volume increases. This compounds monthly.

**Combined effect estimate: +40-60% organic traffic by end of Month 3, +80-120% by end of Month 6 (if program continues).**

---

## Approach: 4 Workstreams

### Workstream 1: Foundation Fix (Weeks 1-3)
**Goal:** Turn the splash gateway into a real content page + eliminate technical anti-patterns.

**Owner:** Engineering + Content (Sundeep approves architecture; Arun provides specs)

**Why this matters:** Without fixing the architectural issue, no other workstream compounds. This is the unblock that makes everything downstream valuable.

### Workstream 2: Schema + E-E-A-T (Weeks 4-6)
**Goal:** Bring root-level schema to parity with `/en-ae/dubai` + add healthcare-specific E-E-A-T signals (medical director, DHA license, Person credentials).

**Owner:** Engineering + Medical team (for credentials/licenses)

**Why this matters:** Healthcare = YMYL. Google and AI engines apply higher trust thresholds. Without visible medical director credentials + DHA license + real AggregateRating, Valeo loses to less-authoritative competitors who surface these signals.

### Workstream 3: Content Production (Weeks 7-10)
**Goal:** Expand content across city × service matrix; close competitor gaps (SKIN111); produce FAQ content clusters targeted at AI citation queries.

**Owner:** Content team (with Arun spec support)

**Why this matters:** Single-page optimization hits a ceiling. Sitemap has 6,705 URLs — most probably underperforming. Content production captures long-tail traffic + feeds AI citations across hundreds of queries, not just one.

### Workstream 4: Authority + Monitoring (Weeks 11-12)
**Goal:** Integrate Trustpilot data into schema; press outreach; set up ongoing measurement framework.

**Owner:** Marketing + Arun (measurement setup)

**Why this matters:** Ensures improvements are measurable + sustainable. Without monitoring, regression goes undetected.

---

## The 12-Week Calendar

### Each week follows the same cadence:
- **Monday:** Analysis + priority setting (morning)
- **Tuesday-Thursday:** Execution
- **Friday:** Measurement + stakeholder update

---

### WEEK 1 (Apr 28 — May 2): Discovery + Root Page Content Spec

**Monday:**
- Kickoff call with Sundeep + engineering lead
- Align on 10% appearance rate target + 40-60% traffic target
- Lock KPI dashboard (appearance rate, traffic, rank, RD)
- Baseline measurement: query 50 AEO-relevant questions across 4 engines; document current Valeo citation count

**Tuesday-Wednesday:**
- Draft content spec for new root page (universal GCC framing, not country-splash)
- Structure: H1 + TL;DR + "What is Valeo" + Services + How It Works + Pricing + Service Area + FAQ (6-8 pairs) + Trust/Accreditation
- Review with Sundeep: tone, positioning, Arabic parity

**Thursday:**
- Engineering scope review — what's needed to replace the splash with content
- Decision: Is the language/region picker moved to header dropdown? Cookie-based redirect for returning users?
- Scope lock: ship Week 3

**Friday:**
- Week 1 report: audit baseline, target metrics, content spec approved, engineering scope locked

**Deliverables:**
- [ ] Baseline measurement doc (50 queries × 4 engines)
- [ ] Root page content spec (approved by Sundeep)
- [ ] Engineering scope doc (approved by dev lead)

---

### WEEK 2 (May 5-9): Build the New Root Page

**Monday:**
- Verify Week 1 deliverables complete
- Engineering kickoff
- Content team begins writing root page copy (~2,500-3,000 words)

**Tuesday-Thursday:**
- Engineering: Replace splash with universal GCC content page
- Content: Draft + review root page copy (English + Arabic parity)
- Schema engineering: Port MedicalBusiness + LocalBusiness + FAQPage + BreadcrumbList blocks from `/en-ae/dubai` to root
- Add Organization @id fragments + ImageObject wrapping for logo

**Friday:**
- Staging deployment of new root page
- QA: Content review + schema validation (schema.org validator)
- Approval checkpoint with Sundeep before shipping

**Deliverables:**
- [ ] New root page in staging with 2,500+ words of content
- [ ] Enhanced schema @graph with 6+ types (Organization, MedicalBusiness, LocalBusiness, WebPage, FAQPage, BreadcrumbList)
- [ ] Schema passes schema.org validator
- [ ] Arabic (`/ar-ae/`) version parity

---

### WEEK 3 (May 12-16): Ship + Technical Fixes

**Monday:**
- Final review of staging — Sundeep sign-off

**Tuesday:**
- **PRODUCTION DEPLOY: New root page** (highest-impact single action in the program)
- Submit updated URL to Google Search Console → request re-indexing
- Submit to Bing Webmaster Tools

**Wednesday:**
- Technical fixes ship:
  - Add HSTS header (`max-age=63072000; includeSubDomains; preload`)
  - Relax Cache-Control (`public, max-age=0, s-maxage=3600, stale-while-revalidate=86400`)
  - Fix `dateModified` to reflect real content-update timestamp (not render time)

**Thursday:**
- Verify AI bot re-crawl via log analysis
- Manual check: query 10 baseline queries in ChatGPT/Perplexity/Claude — is new content reflected?
- Fix any render regressions

**Friday:**
- Week 3 report: Foundation shipped. Metrics baseline reset. Early indicators of re-indexing.

**Deliverables:**
- [ ] Production root page live with full content + schema
- [ ] HSTS + Cache-Control fixes deployed
- [ ] `dateModified` logic fixed
- [ ] Re-indexing requested in GSC/Bing

**Expected Week 3 impact:**
- Google re-indexes root within 48-72 hours
- AI crawlers re-fetch within 7-14 days
- First signs of improved citation in manual checks

---

### WEEK 4 (May 19-23): Medical Director + Founder Schema

**Monday:**
- Identify Valeo's medical director + founder profiles to feature
- Confirm credentials (DHA license numbers, medical specialties, LinkedIn URLs)
- Content: Draft "About the Team" section copy

**Tuesday-Wednesday:**
- Engineering: Add Person schema for founder + medical director with full hasCredential blocks
- Content: Ship "About" section with bylines, credentials, photos
- Visible DHA license number + authorization statement on root page

**Thursday:**
- Integrate Trustpilot review data into AggregateRating schema
- Ship on MedicalBusiness block
- Add visible "Rated 4.8/5 from X reviews on Trustpilot" on homepage

**Friday:**
- Measure Week 4 appearance rate changes vs Week 0 baseline
- Report: E-E-A-T signals now live

**Deliverables:**
- [ ] Person schema for founder + medical director (with hasCredential)
- [ ] DHA license visible on root page
- [ ] AggregateRating schema with real Trustpilot data
- [ ] "About the Team" section with photos + bylines

---

### WEEK 5 (May 26-30): Schema Depth Expansion to Service Pages

**Monday:**
- Audit top 20 service/city pages for schema quality
- Identify pages needing MedicalBusiness + Service + MedicalTest schema

**Tuesday-Thursday:**
- Engineering: Schema upgrades rolled out to:
  - `/en-ae/dubai` + all UAE city subpages
  - `/en-sa/*` (Saudi Arabia pages)
  - `/en-qa/*` (Qatar)
  - `/en-kw/*` (Kuwait)
- Each location gets: LocalBusiness + MedicalBusiness + BreadcrumbList + (for service pages) MedicalTest / MedicalTherapy / Service
- Port AggregateRating to each location schema

**Friday:**
- Schema audit: validate all schema at schema.org validator
- Report: Schema parity across 20+ top pages

**Deliverables:**
- [ ] 20+ pages with enhanced schema
- [ ] MedicalBusiness + LocalBusiness on all city pages
- [ ] MedicalTest / MedicalTherapy on all service pages
- [ ] All schema validates

---

### WEEK 6 (Jun 2-6): FAQ Content Cluster

**Monday:**
- Harvest PAA (People Also Ask) questions for top 30 queries:
  - "blood test at home Dubai"
  - "home blood test UAE"
  - "IV therapy at home Dubai"
  - "doctor on call UAE"
  - "is at-home blood test accurate"
  - etc.
- Output: 80-100 real user questions

**Tuesday-Thursday:**
- Content team writes FAQ answers (each 40-80 words, direct + authoritative)
- Engineering ships FAQPage schema with 6-8 Q&A pairs per major page
- Deploy to root + top 10 service pages

**Friday:**
- QA: FAQPage schema validation
- Report: 10+ pages now FAQ-rich

**Deliverables:**
- [ ] 80-100 PAA questions harvested
- [ ] 60+ FAQ pairs written + schema-marked
- [ ] Deployed on root + 10 service pages

---

### WEEK 7 (Jun 9-13): Competitor Gap Content — "Valeo vs SKIN111" Style

**Monday:**
- Competitive analysis: What do SKIN111, Onelife, JPR Home Healthcare offer that Valeo doesn't surface well?
- Identify: 5 comparison content opportunities

**Tuesday-Thursday:**
- Write 3 comparison posts:
  - "Valeo Health vs SKIN111: Which At-Home Lab Test Service is Right for You?" (balanced review, not hit-piece)
  - "Home Blood Test Dubai: Complete Comparison Guide 2026" (listicle format with 8 providers)
  - "DHA-Licensed At-Home Healthcare: What to Look For" (category education)

Each post:
- 1,800-2,500 words
- Comparison tables
- FAQPage schema
- Trustpilot quotes (if permitted)
- DHA license prominence
- Internal linking to Valeo service pages

**Friday:**
- Deploy all 3 posts
- Social amplification (LinkedIn — Sundeep's profile if applicable)

**Deliverables:**
- [ ] 3 comparison posts live
- [ ] Each with FAQ + comparison table + internal links
- [ ] LinkedIn posts from founder account

---

### WEEK 8 (Jun 16-20): City Landing Page Optimization

**Monday:**
- Audit top 10 city landing pages (Dubai, Abu Dhabi, Sharjah, Riyadh, Jeddah, Kuwait City, Doha, etc.)
- Identify word-count + schema + FAQ gaps

**Tuesday-Thursday:**
- Content upgrades on each:
  - Ensure 2,000+ words
  - Location-specific intro
  - Local DHA/MOH license acknowledgment
  - City-specific pricing
  - Service availability + delivery times
  - Local FAQ (8-10 pairs)
  - Local testimonials if available

**Friday:**
- QA + deploy
- Measurement: compare Week 1 baseline to Week 8

**Deliverables:**
- [ ] 10 city pages upgraded to 2,000+ words
- [ ] Each with location-specific schema + FAQ

---

### WEEK 9 (Jun 23-27): Blog Content Production Round 1

**Monday:**
- Keyword research for top-of-funnel content:
  - "preventive health screening UAE"
  - "IV therapy benefits"
  - "how often should you get blood tests"
  - "best health checkup Dubai 2026"
  - "at-home nursing services UAE"

**Tuesday-Thursday:**
- Write + ship 5 blog posts (1,200-1,800 words each)
- Each post:
  - TL;DR at top
  - Schema: MedicalWebPage or Article + author (medical director byline)
  - FAQ block
  - Internal links to service + city pages
  - Outbound citations to primary sources (WHO, Ministry of Health, medical journals)

**Friday:**
- Deploy + publish
- Email list + social amplification

**Deliverables:**
- [ ] 5 new blog posts live
- [ ] Each with medical director byline + primary source citations
- [ ] Internal linking strategy executed

---

### WEEK 10 (Jun 30 — Jul 4): Blog Content Production Round 2 + Arabic Content

**Monday:**
- Arabic content audit: which pages are lagging in Arabic version?
- Priority: homepage, top 5 service pages, 3 flagship blog posts

**Tuesday-Thursday:**
- Arabic content team translates + localizes priority pages
- Not straight translation — cultural adaptation (GCC-specific references, Arabic medical terminology)
- Schema: hreflang tags verified, duplicate content avoided
- Additional: 3 more English blog posts (continuing Week 9 momentum)

**Friday:**
- QA Arabic content
- Verify hreflang correctness
- Submit updated sitemap

**Deliverables:**
- [ ] 8 Arabic pages updated
- [ ] 3 more English blog posts shipped (total 8 blog posts by Week 10)
- [ ] Sitemap re-submitted

---

### WEEK 11 (Jul 7-11): Authority Building + Press Outreach

**Monday:**
- Press outreach list: 20 UAE health journalists + 10 GCC tech/wellness publications
- Pitch angle: "Valeo Health reports on GCC at-home healthcare trends" (requires 1 data point — e.g., "X% growth in preventive screening demand")

**Tuesday-Wednesday:**
- Press pitches sent (personalized, not blast)
- Guest post pitches to 5 publications (Gulf News Health, Khaleej Times Wellness, etc.)
- Submit to 10 additional UAE/GCC business directories

**Thursday:**
- Partnership outreach: 5 complementary wellness brands (gyms, nutritionists, wellness apps) for content collaboration

**Friday:**
- Outreach status report
- Early response tracking

**Deliverables:**
- [ ] 20 press pitches sent
- [ ] 5 guest post pitches
- [ ] 10 directory submissions
- [ ] Partnership outreach initiated

---

### WEEK 12 (Jul 14-18): Measurement + Next-Quarter Handoff

**Monday:**
- Comprehensive 12-week measurement audit:
  - AI appearance rate (50 baseline queries × 4 engines)
  - Organic traffic (Google Analytics, GSC)
  - Ranking movements (Ahrefs / Semrush)
  - Referring domains growth
  - AggregateRating shown in SERP
  - Featured snippet captures
  - Trustpilot review count + rating

**Tuesday-Wednesday:**
- Document what worked + what didn't
- Identify top 10 pages by appearance rate improvement
- Identify any regressions

**Thursday:**
- Write quarterly report with:
  - Target achievement status
  - Metrics before/after
  - ROI calculation
  - Q2 recommendations

**Friday:**
- Final presentation to Sundeep + stakeholders
- Handover: measurement dashboard + monthly maintenance plan
- Propose Q2 scope (if engaging continues)

**Deliverables:**
- [ ] 12-week measurement report
- [ ] ROI analysis
- [ ] Q2 scope recommendations
- [ ] Handover documentation

---

## Expected Outcomes by End of Week 12

### Primary metrics

| Metric | Baseline (Apr 14) | Target (Jul 18) |
|---|---|---|
| **AI Appearance Rate** (50 queries × 4 engines) | ~2% | **10-12%** |
| **Citation Rank** (when cited) | N/A | Top 3 |
| **Organic Traffic** | Baseline | **+40-60%** |
| **Page Citation Readiness** | 55% (F) | **85% (B+)** |
| **Brand AI Presence** | 75% (B-) | **85%+ (B+)** |
| **Schema Blocks on root** | 2 | **6+** |
| **FAQ Pairs (sitewide)** | 0 | **80+** |
| **Referring Domains** | Baseline | **+30-50** |
| **Featured Snippets Captured** | Unknown | **5-10** |

### Secondary outcomes
- DHA license + medical director credentials prominently featured (YMYL compliance)
- Arabic content parity on top 10 pages
- 10 blog posts + 3 comparison posts live
- Press outreach pipeline for ongoing coverage
- Measurement dashboard for continuous monitoring

---

## Investment + Scope

### What's included
- Weekly strategy calls with Sundeep (30 min)
- Monday analysis + Friday reporting every week
- Content specs + structural recommendations
- Schema specifications + code snippets
- Competitor monitoring
- Press outreach templates
- Measurement dashboard setup

### What's NOT included (scope boundary)
- Engineering execution (Valeo's dev team or contracted agency)
- Content writing (can be done by Valeo's team or contracted writers — Arun provides specs and reviews)
- Medical content approval (must go through Valeo's medical team for YMYL compliance)
- Paid advertising
- Social media management (beyond founder LinkedIn strategy)

### Resource requirements from Valeo
- **Engineering:** 1 dev for ~15-20 hours/week during Weeks 2-5; ~5-10 hours/week afterward
- **Content:** 1 writer for ~20 hours/week during Weeks 6-10
- **Medical team:** 1-2 hours/week for credential/content approval
- **Sundeep:** 1-2 hours/week for strategic alignment + approvals

### Advisory engagement
- Hourly or retainer (to be discussed)
- Recommendation: retainer model for predictability

---

## Success Criteria + Decision Gates

### Week 4 gate (soft check)
- [ ] Root page shipped + indexed
- [ ] Basic schema enhancements live
- [ ] First improvements visible in manual AI citation checks

**If missed:** Extend Workstream 1 by 1 week. Do not proceed to Workstream 2 until foundation is live.

### Week 8 gate (mid-point)
- [ ] AI appearance rate ≥5% (halfway to 10%)
- [ ] Schema deployed across 20+ pages
- [ ] 60+ FAQ pairs live
- [ ] Organic traffic up 15%+ vs baseline

**If missed:** Diagnose (indexing issues? content quality? measurement error?). Adjust remaining plan.

### Week 12 gate (program completion)
- [ ] AI appearance rate 10-12%
- [ ] Organic traffic +40-60%
- [ ] All 4 workstreams delivered
- [ ] Measurement dashboard live
- [ ] Q2 plan drafted

**If hit:** Continue engagement with Q2 scope (scaling content, Arabic depth, partner integrations).
**If partially hit:** Identify gaps, extend timeline, adjust targets.

---

## Why This Plan Works

### Grounded in actual audit data
Every action in this plan maps to a specific finding in the April 14 audit. No speculation. Fix #1 (root page) alone was quantified to lift Extraction from 5% to 85%.

### Architectural before content
Most agencies start with content production. Without fixing the architectural root cause (splash gateway), content work doesn't compound. This plan fixes foundation first.

### YMYL-aware
Healthcare = Google's highest-trust category. Generic SEO advice doesn't work. Plan explicitly addresses E-E-A-T (medical director, DHA license, credentials) as core requirements, not afterthoughts.

### Measurement-first
Week 1 establishes baseline. Every week has Friday measurement. Week 12 measures against Week 0. No "we'll see how it goes" vagueness.

### Leverages existing strengths
Valeo's brand is strong. Plan amplifies existing brand equity (Trustpilot, SERP position, multi-country presence) rather than rebuilding from zero.

---

## Risks + Mitigations

| Risk | Mitigation |
|---|---|
| Engineering capacity constraint | Week 2-5 is heavy. Scope engineering hours upfront. Consider contractor backfill if needed. |
| Medical content approval bottleneck | Identify medical reviewer + set 48-hour SLA for content approval in Week 1 |
| AI crawler re-indexing delays | Plan assumes 7-14 days for re-crawl. Manual submission to GSC/Bing/IndexNow expedites. |
| Competitor response (SKIN111 counters) | Valeo is ranked #2 with strong brand; catching up is harder than maintaining. |
| Arabic content quality | Use native GCC Arabic writer, not machine translation. Medical terminology matters. |
| Cookie-based root redirect breaks repeat users | Test extensively in Week 2. Fallback to simple header dropdown if issues surface. |

---

## Next Steps

**If approved:**

1. **This week:** Sundeep signs off on scope + pricing
2. **Week 1 (Apr 28):** Kickoff call, baseline measurement, team alignment
3. **Week 3 (May 12):** Ship new root page — single highest-impact milestone
4. **Week 12 (Jul 18):** 12-week review + Q2 scope discussion

### Deliverables to confirm before starting
- [ ] Who is the medical director (name, photo, credentials, DHA license # if disclosable)
- [ ] Who is the founder public profile (Sundeep?)
- [ ] Engineering team availability for Weeks 2-5
- [ ] Content team capacity for Weeks 6-10
- [ ] Brand guidelines / tone preferences
- [ ] Any content topics off-limits

---

## About the Approach

This proposal is built from:
- The full April 14 SEO/AEO/GEO audit of feelvaleo.com
- Sieve-grounded principles on AEO, YMYL healthcare content, and B2B SaaS-to-healthcare-adjacent GTM strategy
- Cross-reference with comparable audits (TRYPS, AnswerMonk) to calibrate expectations
- Direct experience implementing similar programs in B2B SaaS + consumer healthcare contexts

The core insight: **Valeo is one architectural decision away from being the category-leading cited brand in GCC at-home healthcare.** The brand work is done. The measurement gap is the opportunity.

---

**Prepared by:** Arun Sharma
**Contact:** [email]
**Proposal valid through:** 2026-05-15

---

## Appendix A — Audit reference

Full audit document: `feelvaleo-com-SEO.AEO-1-2026-04-14.md`

Key audit scores:
- Overall: 56% (F)
- SEO Score: 73%
- AEO Score: 40%
- Page Citation Readiness: 55% (F)
- Brand AI Presence: 75% (B-)

Top 5 fixes (all addressed in this plan):
1. Serve real content at root (Weeks 1-3)
2. Port schema from `/en-ae/dubai` to root (Weeks 2-5)
3. Fix dynamic `dateModified` (Week 3)
4. Add HSTS + relax Cache-Control (Week 3)
5. AggregateRating + Person schema (Week 4)

## Appendix B — Competitive context

| Brand | SERP Rank | Word count | FAQ | AggregateRating | DHA/License visible |
|---|---|---|---|---|---|
| SKIN111 | #1 | 2,000-2,500 | 5 pairs | 4.9/5 from 1,166 | JCI + ISO + Cambridge |
| **Valeo Health (root)** | **#2** | **106** | **0** | **No (but Trustpilot exists)** | **No (visible only on /en-ae/dubai)** |
| Valeo (/en-ae/dubai) | also indexed | 2,677 | 1 | No | Yes |
| JPR Home Healthcare | #3-4 | ~2,000 | Unknown | Unknown | Yes (DHA) |
| Onelife UAE | #5-6 | — | — | — | Yes (DHA) |

Valeo is competing at #2 with an empty root page. Fixing the root unlocks #1 potential.
