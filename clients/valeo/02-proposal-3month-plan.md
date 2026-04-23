# Scope Draft: Valeo Health AI Visibility + Organic Growth (12 Weeks)

**For:** Sundeep, Valeo Health (feelvaleo.com)
**Date:** 2026-04-23
**Duration:** 12 weeks, starting week of 2026-04-28
**Status:** Scope draft for discussion — pricing, resourcing, and final targets to be agreed in kickoff call
**Basis:** SEO + AEO + GEO Audit of feelvaleo.com, 2026-04-14

---

## Opportunity

Valeo ranks in the top results on Google for high-intent at-home healthcare queries in Dubai and has established off-page brand presence (Trustpilot, App Store, Dubai Review, multiple social profiles). The April 14 audit scored Brand AI Presence in the B- range — directionally above the competitors audited in the same session.

The same audit surfaced a specific architectural constraint: the canonical root page (`feelvaleo.com`) serves ~106 words of language/country splash content, while the substantive service content (~2,677 words) lives at `/en-ae/dubai`. This structure *may limit* what AI engines can extract when they fetch the root URL — which is typically the most-crawled and most-cited URL for a brand. Whether this is the dominant constraint on AI appearance, or one of several, will be validated through the baseline measurement described below.

The intent of this engagement is to close the extraction gap, improve page-level citation readiness, and test whether existing brand authority can be converted into measurable AI citations and incremental organic traffic over a 12-week window.

---

## Methodology Note

Scores and signals referenced here are drawn from the April 14 audit (98 checks across technical SEO, schema, AEO extraction, AEO trust, AEO selection, entity consistency, and GEO dimensions). Specific audit numbers:

- **Page Citation Readiness:** 55% (F) — composite of technical + schema + content extractability checks
- **Brand AI Presence:** ~75% (B-) — *directional* composite of SERP position, indexed URL count, and third-party brand mention signals; **not** a measured AI citation rate
- **AEO Extraction (root page):** 5% of checks passing

**AI citation rate is not currently measured.** Week 1 Task 1 is to run a 50-query baseline across ChatGPT, Claude, Perplexity, and Google AI Mode to establish the measured starting point. Target scenarios in this document are illustrative; specific target ranges will be set against that baseline after Week 1.

---

## Scope: 3 Workstreams

### Workstream 1 — Foundation Fix (Weeks 1-4)
Rebuild the root page so AI engines can extract substantive content from it. Port the existing schema pattern from `/en-ae/dubai` to root. Address technical hygiene items from the audit (dynamic `dateModified`, missing HSTS, aggressive Cache-Control).

This is the highest-confidence block of work in the engagement: the content, schema, and topical depth already exist on the site and are being relocated, not invented. The audit's Extraction checks are expected to move materially upward post-deploy (exact magnitude to be measured). Actual impact on AI citations will depend on AI engine re-crawl cadence (commonly 7-21 days for major engines) and will be assessed in Weeks 4-8.

### Workstream 2 — Content + E-E-A-T (Weeks 4-10)
- **Medical authority signals.** Founder and medical director Person schema with DHA credentials; visible DHA license display; medical director byline on health content. Standard E-E-A-T requirements for YMYL healthcare content.
- **AggregateRating integration.** Connect verified Trustpilot review data to Organization + MedicalBusiness schema, consistent with Google's structured data guidelines and Trustpilot's platform TOS. No incentivized generation, no gating, no fabrication.
- **FAQ content clusters.** ~50 FAQ pairs across top pages, each sourced from observed SERP People-Also-Ask data and medical-reviewed. FAQPage schema on priority pages.
- **Top 5 city/service pages upgraded** to competitive depth. (Reduced from 10 to 5 to protect against scope overload — additional pages deferred to Phase 2.)
- **2 balanced comparison posts** (Valeo vs category alternatives). Legal review before publish.

**Deferred to Phase 2 (explicit):** Arabic content parity, press outreach at scale, Reddit/Quora participation, additional city-page depth beyond the top 5. These are material workstreams and should be scoped separately with their own compliance + capacity review.

### Workstream 3 — Measurement + Competitive Intel + Paid Efficiency Audit (Ongoing)
- **AI citation tracking.** 50 canonical queries × 4 engines, weekly measurement, Valeo + 3-4 competitors.
- **SERP + AI Overview monitoring** on ~30 priority queries, weekly.
- **Competitive gap analysis.** Where competitors are cited and Valeo is not; what content or schema appears to drive the gap.
- **AI-assisted keyword discovery.** Use ChatGPT/Claude/Perplexity to surface real user phrasing that classical keyword tools underweight.
- **Alert infrastructure.** Automated notifications (email or Telegram) on material changes — competitor rank shifts, new AI Overview triggers, review volume movements.
- **Paid efficiency audit (advisory only — no execution).** Monthly audit of Google Ads / Meta campaigns run by Valeo's marketing team, covering: keyword-to-landing-page alignment, Quality Score drivers, attribution gaps, organic cannibalization, conversion tracking accuracy, negative keyword coverage, ad-copy vs landing-page consistency. Deliverable: efficiency report + recommendations. Marketing team owns execution.
- **Weekly dashboard** (Airtable or Notion): single view of AI appearance signals, SERP rank, organic traffic, referring domains, and paid metrics shared by the marketing team.

---

## Compliance & Governance

Healthcare content carries regulatory and platform obligations. These are built into the engagement, not afterthoughts.

### Medical review workflow
- All health-related content passes Valeo's medical team before publish
- Target SLA: 48-hour turnaround per piece (dependent on Valeo reviewer capacity)
- Medical reviewer must be DHA-licensed
- Content making therapeutic or diagnostic claims requires a physician byline with credentials

### Claim restrictions
- No unverified treatment outcome claims
- No comparative clinical efficacy claims without clinical evidence
- No health advice not authored or reviewed by a licensed physician
- All claims adhere to Google Search Quality Evaluator YMYL guidelines (author expertise surfaced, physician review documented, primary-source citations)

### DHA / MOH regulatory adherence
Service descriptions, outcome statements, pricing, and clinical procedure references comply with UAE Dubai Health Authority (DHA) and, where applicable, Saudi Ministry of Health (MOH) advertising and claims policies. License numbers and authorizations visible where required.

### Testimonial / review usage
- Patient testimonials require documented consent + attribution
- Review collection follows Trustpilot's own TOS: post-service invitation email only; no incentivization; no gating of service on review completion
- AggregateRating schema reflects only real, verifiable Trustpilot data
- No schema inflation

### Competitor comparison content
Valeo vs competitor content goes through legal review before publish. Claims are factual, sourced, and balanced (pros + cons for each entity). No hit-piece framing (Google actively deindexes these in healthcare contexts).

### Community engagement (Reddit / Quora / forums)
Explicitly deferred to Phase 2. Healthcare brands face disclosure obligations and reputational exposure on these surfaces. Not in scope for this engagement.

### Approval ownership
Sundeep (or delegated approver) is the single point of approval for: final content publish, schema deploys touching medical claims, comparison content, review collection campaigns, and any public statement referencing clinical outcomes.

---

## 12-Week Calendar

Cadence: Monday analysis → Tuesday-Thursday execution → Friday measurement + report.

### Weeks 1-2 — Baseline + Foundation Scope
- **W1:** Kickoff. Run baseline measurement (50 queries × 4 engines). Set up intel dashboard. Lock content spec for new root page. Identify medical director for Person schema. **Pricing + target ranges finalized after baseline lands.**
- **W2:** Build new root page in staging. Content team drafts ~2,500 words with medical team review. Schema @graph drafted.

### Weeks 3-4 — Ship Foundation + Credentials
- **W3:** Production deploy of new root page. Technical fixes ship (HSTS, Cache-Control, `dateModified`). GSC + Bing re-indexing requested.
- **W4:** Founder + medical director Person schema live with DHA credentials. Visible DHA license on root. AggregateRating connected to real Trustpilot data.

### Weeks 5-6 — Schema Depth + FAQ
- **W5:** Schema upgrades across top 10 city/service pages (LocalBusiness + MedicalBusiness + BreadcrumbList).
- **W6:** ~50 FAQ pairs written (PAA-sourced), medical-reviewed, deployed with FAQPage schema across priority pages.

### Weeks 7-8 — Content Depth + Comparison
- **W7:** Top 5 city pages upgraded to competitive depth. **First paid ads audit report** delivered to marketing team.
- **W8:** 2 comparison posts (legal-reviewed) shipped.

### Weeks 9-10 — Blog + Authority
- **W9:** 3-5 blog posts shipped (medical-reviewed, primary-source citations).
- **W10:** 2-3 more blog posts. **Second paid ads audit report.**

### Weeks 11-12 — Measurement + Handover
- **W11:** Trustpilot review invitation (compliant — post-service email, no incentivization).
- **W12:** 12-week measurement audit. Results review. Q2 scope recommendations. Dashboard + intel handover.

---

## Target Scenarios (not commitments)

All outcomes are **target scenarios** — illustrative ranges, subject to (a) baseline validation in Week 1 and (b) the execution and external dependencies listed in the next section. These are not guarantees.

| Dimension | Week 0 | Scenario: Conservative | Scenario: Upside |
|---|---|---|---|
| AI citation rate (50 queries × 4 engines) | Measured Week 1 | +2-3x baseline | +5-10x baseline |
| Page Citation Readiness (audit score) | 55% | 75-80% | 85%+ |
| Organic traffic (total sessions) | Measured Week 1 | +20-30% | +40-60% |
| Branded search trend (GSC brand-term impressions) | Measured Week 1 | Trending up | Clear step-change |
| Featured snippets captured | Not measured | 2-5 new | 5-10 new |
| Schema depth (pages with MedicalBusiness + FAQPage) | Low | 15+ pages | 20+ pages |
| FAQ pairs live | 0 | 40-50 pairs | 50+ pairs |
| Referring domains | Measured Week 1 | +5-15 new | +15-30 new |
| Competitive intel dashboard | None | Live + weekly refresh | Live + alerts operational |
| Paid ads audit reports | None | 2 reports delivered | 2 reports + adopted changes |

Concrete target ranges (replacing "conservative / upside") will be set after Week 1 baseline.

---

## Assumptions

Targets assume these conditions hold:

- Engineering capacity as committed (20-25 hrs/week Weeks 2-5; 10-15 hrs/week after)
- Medical reviewer availability at a 48-hour content-approval SLA
- Legal review availability for comparison + regulatory-adjacent content (3-5 hrs total)
- Content team capacity (~20 hrs/week) during Weeks 6-10
- Sundeep availability: ~3 hrs/week for strategic alignment + approvals
- Marketing team willingness to share paid ad account access for the audit layer
- No major Google or AI engine algorithm changes during engagement
- Review invitation response rates within industry norms for healthcare

If any of these change materially, scope and targets are renegotiated.

---

## Risks

- **Re-crawl lag.** AI engines may not re-crawl the new root page within the engagement window. Citation impact could land in Weeks 13-20 rather than Weeks 4-12.
- **Schema alone is insufficient.** Schema + content improvements increase *extractability* but do not guarantee *selection* by AI engines. Selection depends on authority signals outside our direct control.
- **Regulatory review latency.** If medical or legal review SLAs slip, content workstream compresses or slips.
- **Competitive response.** If SKIN111 or Onelife materially upgrades their content during this window, relative position may not improve despite absolute gains.
- **Attribution ambiguity.** Organic traffic gains in this period may reflect seasonality or paid-channel spillover; clean attribution requires the baseline + control groups already defined in the measurement plan.

---

## Resource Commitments (Valeo side)

| Role | Weeks 1-5 | Weeks 6-12 |
|---|---|---|
| Engineering | 20-25 hrs/week | 10-15 hrs/week |
| Content team | 5 hrs/week | 20 hrs/week |
| Medical reviewer | 3-5 hrs/week | 3-5 hrs/week |
| Legal reviewer | 2-3 hrs total | 2-3 hrs total |
| Sundeep (founder) | 3-4 hrs/week | 2-3 hrs/week |

If capacity is lower than the table, scope reduces proportionally. This is a meaningful client-side commitment and should be confirmed before kickoff.

---

## Advisor Effort Estimates

Below are **advisor (Arun) hours only** — the contracted scope. Valeo-side hours are separate (see Resource Commitments above). A **30% buffer** is applied per workstream to cover review cycles, regulatory-review latency, re-crawl diagnostics, prompt tuning iterations, and scope ambiguities typical in healthcare delivery.

The plan includes material **analysis and automation build-out** — not just strategy. The blog writer automation and competitive intel infrastructure are significant engineering efforts in their own right and are called out explicitly below.

### Workstream 1 — Foundation Fix (Weeks 1-4)

| Activity | Base hrs |
|---|---|
| Root page content spec + structure (2,500 words, medical-reviewed brief) | 10 |
| Schema @graph design (port + enhance from /en-ae/dubai) | 8 |
| Technical fix spec + engineering handoff (HSTS, Cache-Control, dateModified) | 4 |
| Staging review + pre-deploy QA across AI crawler user agents | 6 |
| Post-deploy AI crawl validation + re-index tracking | 4 |
| Person schema spec (founder + medical director, DHA credential display) | 4 |
| AggregateRating ↔ Trustpilot integration spec + TOS compliance review | 5 |
| Strategy calls + iteration | 6 |
| **Base subtotal** | **47** |
| **+ 30% buffer** | **14** |
| **Buffered total** | **~61 hrs** |

### Workstream 2 — Content + E-E-A-T + Brand-Aware Blog Writer Automation (Weeks 4-10)

| Activity | Base hrs |
|---|---|
| **Content strategy + briefs** | |
| FAQ sourcing methodology + PAA harvesting approach | 6 |
| 50 FAQ briefs (groups of 5-10) + editorial QA | 16 |
| Top-5 city-page content briefs + competitive-depth framework | 20 |
| 2 comparison post frameworks + legal gate spec | 8 |
| 5-8 blog post briefs + editorial standards | 15 |
| E-E-A-T audit (medical authority surfacing across site) | 8 |
| Schema consistency QA across 10+ pages | 10 |
| Content iteration + medical-review coordination | 10 |
| **Brand-aware blog writer automation (custom build)** | |
| Brand voice + guardrail spec (ingest Valeo tone, YMYL compliance rules, DHA constraints) | 10 |
| Pipeline build: intake → draft → medical-review handoff → schema injection → publish-ready export | 20 |
| Prompt library + few-shot examples for healthcare YMYL (per content type: FAQ, blog, city page) | 10 |
| Testing + tuning on 3-5 sample pieces against medical reviewer feedback | 10 |
| Medical-review integration flow (diff view, approval tracking) | 4 |
| Handover docs + content-team training | 4 |
| **Base subtotal** | **151** |
| **+ 30% buffer** | **45** |
| **Buffered total** | **~196 hrs** |

### Workstream 3 — Measurement Infrastructure + Competitive Intel + Paid Audit (Weeks 1-12)

Split into a one-time **Build phase** (Weeks 1-3) and **Run phase** (Weeks 2-12).

#### Build phase (one-time)

| Activity | Base hrs |
|---|---|
| Baseline measurement harness (50 queries × 4 engines × scripted runs) | 8 |
| Competitive intel automation (SERP + AI Overview scrapers, 4 competitors) | 14 |
| AI citation tracking pipeline (per-engine parsers, attribution logic) | 12 |
| Competitor comparison layer + normalization + scoring | 10 |
| Telegram alert infrastructure (bot, threshold rules, routing) | 10 |
| Dashboard build (Airtable / Notion, views, rollups, data sync) | 12 |
| **Build subtotal** | **66** |

#### Run phase (ongoing, 12 weeks)

| Activity | Base hrs |
|---|---|
| Weekly AI citation measurement ritual (2.5 hrs × 12) | 30 |
| Weekly competitor SERP + AI Overview tracking (2 hrs × 12) | 24 |
| Competitive gap deep-dive analyses (3 iterations × 5 hrs) | 15 |
| AI-assisted keyword discovery (ChatGPT/Claude/Perplexity probing) | 10 |
| Paid efficiency audit reports (2 × 10 hrs, full review of Google Ads + Meta) | 20 |
| Week 12 measurement audit + ROI write-up + Q2 scope | 15 |
| Cross-workstream strategy alignment + Friday reports | 10 |
| **Run subtotal** | **124** |

| Rollup | Hrs |
|---|---|
| Build + Run base | 190 |
| + 30% buffer | 57 |
| **Buffered total** | **~247 hrs** |

### Advisor engagement total

| Workstream | Base | +30% buffer | Buffered total |
|---|---|---|---|
| WS1 — Foundation Fix | 47 | 14 | **~61** |
| WS2 — Content + Blog Writer Automation | 151 | 45 | **~196** |
| WS3 — Measurement Infra + Intel + Paid Audit | 190 | 57 | **~247** |
| **Advisor total (Arun)** | **388** | **116** | **~504 hrs** |

Implied weekly load: **~42 hrs/week** across 12 weeks. This is a near-full-time commitment. If the scope needs to run alongside other advisor commitments, the blog-writer automation and/or top-5 city page upgrades are the natural deferral candidates — those two items together represent ~60 hrs of buffered scope.

Notes:
- Buffer is drawn down only as consumed; unused buffer rolls into Phase 2 scope discussions.
- If Week 1 baseline reveals different starting conditions than the audit implies, estimates are re-baselined before Week 3.
- Automation build hours (blog writer + intel infra) are front-loaded in Weeks 1-4 — the heaviest advisor weeks are Weeks 1-4, tapering in Weeks 9-12 to run ops + audit.

---

## Pricing

Pricing is intentionally deferred to the kickoff discussion. Three structures are possible:

- **Phased fee** — Foundation / Content+Authority / Measurement+Handover, each with a decision gate before the next unlocks
- **12-week retainer** — single monthly fee × 3 months, all deliverables included
- **Milestone-based** — payment tied to specific deliverables

Final structure + figures are a conversation, not a quote in this document. **This is a scope draft, not a priced proposal.**

**Not included under any structure:**
- Engineering execution (Valeo's dev team)
- Content writing (Valeo's content team)
- Medical / legal reviewer time (Valeo's team)
- Paid ad spend (owned by marketing team)
- Tool subscriptions (Ahrefs, Airtable, etc.)

---

## Decision Gates

### Week 4 gate — foundation complete
- New root page live in production
- Schema depth materially increased at root (specific block count set in Week 1 plan)
- Technical fixes shipped (HSTS, Cache-Control, `dateModified`)
- Indexing confirmed in GSC + Bing
- Medical director Person schema live with credentials

If foundation is not substantially complete, Workstream 2 pauses and the delay is diagnosed before expansion.

### Week 8 gate — content + authority mid-point
- Schema depth live on 15+ pages
- 40+ FAQ pairs deployed
- Top 5 city pages upgraded
- 2 comparison posts shipped (legal-reviewed)
- First paid ads audit report delivered
- AI citation rate direction vs Week 1 baseline assessed (direction, not absolute threshold)

If mid-point is materially behind, remaining scope is renegotiated before Weeks 9-10.

### Week 12 gate — engagement close
- Measured AI citation rate vs Week 1 baseline (range agreed in Week 1)
- Organic traffic vs Week 1 baseline (range agreed in Week 1)
- Competitive intel dashboard live + operational
- 2 paid ads audit reports delivered
- Q2 scope recommendations documented

Outcome scenarios:
- **Base case:** core foundation + schema shipped; citation direction positive; traffic gains within conservative range → reasonable success, extend if aligned.
- **Upside:** full scope shipped; citation gains at higher end of range → strong result, scale engagement.
- **Downside:** foundation slipped or citation direction unclear → honest debrief, diagnose gaps, adjust approach.

---

## Why This Scope Is Credible

1. **Baseline-first.** Week 1 measures before Week 3 ships. Targets anchor to measured starting points, not estimates.
2. **Audit-grounded.** Every fix traces to a specific finding in the April 14 audit.
3. **Compliance-native.** Medical review, DHA adherence, YMYL standards, and review-collection TOS are in the workflow, not added after.
4. **Conditional framing.** Outcomes are target scenarios with explicit dependencies — not commitments.
5. **Focused scope.** 3 workstreams. Arabic, press at scale, Reddit/Quora explicitly deferred to Phase 2.
6. **Paid ads stays with marketing team.** We audit efficiency; we do not duplicate execution.
7. **Evidence over assertion.** Directional claims labeled as directional. Unmeasured values labeled as unmeasured.

---

## Next Steps

1. Sundeep reviews this scope draft
2. Discussion call: resource commitment confirmation, pricing structure selection, question resolution
3. Kickoff week of April 28 (if aligned)
4. Week 1 Task 1: measure baseline (50 queries × 4 engines) → target ranges locked
5. First decision gate: Week 4

---

**Prepared by:** Arun Sharma
**Contact:** [email]
**Document status:** Scope draft v4 — supersedes prior drafts
