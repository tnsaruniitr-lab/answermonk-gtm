# Scope Draft: Valeo Health AI Visibility + Organic Growth (16 Weeks / 4 Months)

**For:** Sundeep, Valeo Health (feelvaleo.com)
**Date:** 2026-04-23
**Duration:** 16 weeks (4 months), starting week of 2026-04-28
**Status:** Scope draft for discussion — pricing, resourcing, and final targets to be agreed in kickoff call
**Basis:** SEO + AEO + GEO analysis of feelvaleo.com, 2026-04-14

---

## Opportunity

Valeo ranks in the top results on Google for high-intent at-home healthcare queries in Dubai and has established off-page brand presence (Trustpilot, App Store, Dubai Review, multiple social profiles). The April 14 analysis scored Brand AI Presence in the B- range — directionally above the competitors reviewed in the same session.

The same analysis surfaced a specific architectural constraint: the canonical root page (`feelvaleo.com`) serves ~106 words of language/country splash content, while the substantive service content (~2,677 words) lives at `/en-ae/dubai`. This structure *may limit* what AI engines can extract when they fetch the root URL — which is typically the most-crawled and most-cited URL for a brand. Whether this is the dominant constraint on AI appearance, or one of several, will be validated through the baseline measurement described below.

The intent of this engagement is to close the extraction gap, improve page-level citation readiness, and test whether existing brand authority can be converted into measurable AI citations and incremental organic traffic over a 16-week (4-month) window.

---

## Target Outcome

Two headline outcomes anchor the engagement:

- **AI appearance rate: >10%** across the 50-query × 4-engine canonical set (up from effectively **0%** — Week 1 baseline will confirm, expected near zero).
- **Organic website traffic: +[X]%** — specific range to be aligned against the Week 1 GSC + GA4 baseline and documented in the Week 1 kickoff note.

**Co-ownership:** Outcomes are **co-owned by Ritwik (Valeo)** and Arun (AEO Operator + Build Partner), with Sundeep as approver. Weekly delivery cadence and scope decisions run through Ritwik + Arun; escalations and gate decisions run through Sundeep.

---

## Role: AEO Operator + Build Partner

Arun's role on this engagement is **not passive advisory**. The scope includes scoping, building, and running:

- **Scope:** workstream design, baseline measurement methodology, content frameworks, compliance gates, target-range setting
- **Build:** blog content bot automation, Founder Live Dashboard, Sieve brain integration pipeline, schema drift validators, competitive change detection, content recency triggers — delivered as working infrastructure, not specs handed over
- **Run:** weekly measurement ritual, competitive intel deep-dives, paid efficiency audits, alert curation, content QA against E-E-A-T and YMYL standards

Valeo's engineering team handles production deploys on its own stack. Valeo's content team executes against the frameworks. Arun owns everything between strategy and their execution — including the tooling that makes their execution efficient.

This is why the engagement is priced as a 4-month operator commitment, not an advisor retainer.

---

## Methodology Note

Scores and signals referenced here are drawn from the April 14 analysis (98 checks across technical SEO, schema, AEO extraction, AEO trust, AEO selection, entity consistency, and GEO dimensions). Specific numbers:

- **Page Citation Readiness:** 55% (F) — composite of technical + schema + content extractability checks
- **Brand AI Presence:** ~75% (B-) — *directional* composite of SERP position, indexed URL count, and third-party brand mention signals; **not** a measured AI citation rate
- **AEO Extraction (root page):** 5% of checks passing

**AI citation rate is not currently measured.** Week 1 Task 1 is to run a 50-query baseline across ChatGPT, Claude, Perplexity, and Google AI Mode to establish the measured starting point. Target scenarios in this document are illustrative; specific target ranges will be set against that baseline after Week 1.

---

## Scope: 4 Workstreams

### Workstream 1 — Foundation Fix (Weeks 1-5)
Rebuild the root page so AI engines can extract substantive content from it. Port the existing schema pattern from `/en-ae/dubai` to root. Address technical hygiene items from the analysis (dynamic `dateModified`, missing HSTS, aggressive Cache-Control).

This is the highest-confidence block of work in the engagement: the content, schema, and topical depth already exist on the site and are being relocated, not invented. Extraction checks are expected to move materially upward post-deploy (exact magnitude to be measured). Actual impact on AI citations will depend on AI engine re-crawl cadence (commonly 7-21 days for major engines) and will be assessed in Weeks 5-10.

### Workstream 2 — Content + E-E-A-T (Weeks 5-13)
- **Medical authority signals.** Founder and medical director Person schema with DHA credentials; visible DHA license display; medical director byline on health content. Standard E-E-A-T requirements for YMYL healthcare content.
- **AggregateRating integration.** Connect verified Trustpilot review data to Organization + MedicalBusiness schema, consistent with Google's structured data guidelines and Trustpilot's platform TOS. No incentivized generation, no gating, no fabrication.
- **FAQ content clusters.** ~50 FAQ pairs across top pages, each sourced from observed SERP People-Also-Ask data and medical-reviewed. FAQPage schema on priority pages.
- **Top 5 city/service pages upgraded** to competitive depth. (Reduced from 10 to 5 to protect against scope overload — additional pages deferred to Phase 2.)
- **2 balanced comparison posts** (Valeo vs category alternatives). Legal review before publish.
- **Founder-led community authority (compliance-native):**
  - **Compliance playbook first** — Valeo-specific, medical + legal reviewed: what founders can say, what they can't, how to redirect medical-advice asks, disclosure templates. All community activity gated on this landing.
  - **Quora.** Topic map of 15-20 high-intent UAE at-home healthcare questions. Founder-byline answer framework. Arun drafts and edits for AEO + compliance; Sundeep or Ritwik post under their real identity.
  - **Reddit.** Subreddit map (r/Dubai, r/UAE, r/UAE_Expats, r/DubaiLife + 2-3 relevant health/wellness subs). ~2 founder posts/month under identified handles. Operational and category content (pricing transparency, logistics, patient experience) — **no medical advice in replies**; those redirect to consult booking.
  - **Review expansion.** Google Business Profile + App Store review invitation campaigns, extending the Trustpilot invitation flow. Same compliance rules: post-service email, no incentivization, no gating.
  - **Monthly community footprint audit** — mentions, sentiment, response coordination (Ritwik owns responses; Arun coordinates).

**Deferred to Phase 2 (explicit):** brand-aware blog writer automation (full pipeline build), Arabic content parity, press outreach at scale, additional city-page depth beyond the top 5, Telegram alerts. These are material workstreams and should be scoped separately with their own compliance + capacity review.

### Workstream 3 — Measurement + Competitive Intel + Paid Efficiency Audit (Weeks 1-16)
- **AI citation tracking.** 50 canonical queries × 4 engines. Weekly in Weeks 1-5 (to catch re-crawl impact after foundation ship), bi-weekly Weeks 6-16.
- **SERP + AI Overview monitoring** on ~30 priority queries, same cadence.
- **Competitive gap analysis.** 3 deep-dives during the engagement — where competitors are cited that Valeo isn't, and what content/schema appears to drive the gap.
- **AI-assisted keyword discovery.** Surface real user phrasing via ChatGPT/Claude/Perplexity probing (passes at Weeks 4, 10, and 15).
- **Email alert infrastructure** on material changes — competitor rank shifts, new AI Overview triggers, review volume movements. (Telegram deferred to Phase 2.)
- **Paid efficiency audit (advisory only — no execution).** 2 audit reports (Week 10, Week 16) of Google Ads / Meta campaigns run by Valeo's marketing team: keyword-to-landing-page alignment, Quality Score drivers, attribution gaps, organic cannibalization, conversion tracking, negative keyword coverage, ad-copy vs landing-page consistency. Marketing team owns execution.
- **Measurement dashboard** surfaces into the Founder Live View built in WS4 (shared single source of truth).

### Workstream 4 — Always-On Intelligence (Weeks 2-16)

Continuous intelligence layer — the single source of truth Ritwik and Sundeep open any day of the week. Turns the engagement from periodic reports into a living system.

- **Founder Live Dashboard.** Single view (Airtable or Retool) of AI appearance rate, SERP rank, organic traffic, Valeo vs competitor citation gap, content health (freshness + schema coverage), paid metrics. Always-current; no waiting for Friday reports.
- **Sieve brain integration.** Valeo pages continuously re-audited against the latest extracted rules in Sieve's brain (principles, playbooks, anti-patterns). When LLM / SEO / AEO rules shift (Google docs, OpenAI guidance, Perplexity changes), Valeo's pages get re-checked against the new standard and drift is flagged.
- **Schema drift + validator automation.** Weekly scan across top 20+ pages. Alerts when Trustpilot schema breaks, medical director credentials desync, FAQPage schema drops, or dateModified goes stale.
- **Content recency triggers.** Pages flagged when (a) unreviewed >90 days, (b) primary-source citations go dead, (c) E-E-A-T signals (author credential, med review byline) missing, (d) internal links break. Queue feeds directly into Ritwik's weekly review.
- **Competitive change detection.** Weekly competitor page-diff + schema-diff + new-page detection. AI Overview trigger changes tracked per query. Alerts surface the specific deltas, not aggregate scores.

**Why this deserves its own workstream:** the deliverable is not a report; it is infrastructure. Once live, it keeps checking the site forever against evolving LLM/SEO standards. This is the compounding layer — everything else is one-off.

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
In scope, **compliance-native**. Governed by a dedicated Valeo community playbook (medical + legal reviewed) before any posting. Non-negotiables:
- Founders (Sundeep / Ritwik) post under their real identified accounts. No anonymous accounts, no astroturfing, no incentivized third-party posting.
- No medical, diagnostic, or therapeutic advice in free-form replies. Those get redirected to consult booking.
- Operational / category / patient-experience content only (pricing transparency, logistics, service quality, UAE healthcare context).
- All Quora and Reddit content flows through the same medical + legal review gate as on-site content.
- Weekly monitoring for user-generated health questions addressed to Valeo; responses coordinated with the medical team.

### Approval ownership
Sundeep (or delegated approver) is the single point of approval for: final content publish, schema deploys touching medical claims, comparison content, review collection campaigns, and any public statement referencing clinical outcomes.

---

## 16-Week Calendar

Cadence: Monday analysis → Tuesday-Thursday execution → Friday measurement + report.

### Weeks 1-2 — Baseline + Foundation Scope + Intel Groundwork
- **W1:** Kickoff. Run baseline measurement (50 queries × 4 engines). Lock content spec for new root page. Identify medical director for Person schema. Founder Live Dashboard wireframe + data-source inventory (WS4 begins). **Pricing + target ranges finalized after baseline lands.**
- **W2:** Build new root page in staging. Content team drafts ~2,500 words with medical team review. Schema @graph drafted. Sieve brain integration scoped (rules to continuously check Valeo against).

### Weeks 3-5 — Ship Foundation + Credentials + Dashboard v1
- **W3:** Production deploy of new root page. Technical fixes ship (HSTS, Cache-Control, `dateModified`). GSC + Bing re-indexing requested. Founder Dashboard v1 live (read-only).
- **W4:** Founder + medical director Person schema live with DHA credentials. Visible DHA license on root. AggregateRating connected to real Trustpilot data. Sieve brain integration hooked — first automated re-audit of Valeo pages against current rules.
- **W5:** Sieve-driven drift alerts operational. Competitive change detection live (weekly competitor page-diff). **Week 5 decision gate.**

### Weeks 6-8 — Schema Depth + FAQ + Content Automation + Community Playbook
- **W6:** Schema upgrades across top 10 city/service pages (LocalBusiness + MedicalBusiness + BreadcrumbList). Schema drift validator running. **Community compliance playbook drafted + legal/medical reviewed.**
- **W7:** ~50 FAQ pairs written (PAA-sourced), medical-reviewed, deployed with FAQPage schema across priority pages. Content recency triggers live. **Quora topic map + first 5 founder-byline answer frameworks drafted.**
- **W8:** First competitive gap deep-dive. **First 5 Quora answers posted (Sundeep/Ritwik byline). Reddit subreddit map + first founder post framework ready.**

### Weeks 9-11 — Content Depth + Comparison + Community Cadence + First Audit
- **W9:** Top 5 city pages upgraded to competitive depth. **First Reddit post live (founder-identified). 5 more Quora answers posted. Google Business Profile review invitation flow live.**
- **W10:** 2 comparison posts (legal-reviewed) shipped. **First paid ads audit report** delivered to marketing team. **First monthly community footprint audit.** **Week 10 decision gate.**
- **W11:** 2-3 blog posts shipped (medical-reviewed, primary-source citations). Second competitive gap deep-dive. **Second Reddit post. 5 more Quora answers. App Store review invitation flow live.**

### Weeks 12-14 — Blog Velocity + Authority Signals + Community Cadence
- **W12:** 3 blog posts. Dashboard refinement based on Ritwik + founder feedback (3-week usage). **Third Reddit post. Second monthly community footprint audit.**
- **W13:** 2-3 blog posts. Trustpilot review invitation wave (compliant). **5 more Quora answers.**
- **W14:** 2 blog posts. Third competitive gap deep-dive. Content recency queue cleared. **Fourth Reddit post.**

### Weeks 15-16 — Measurement + Handover
- **W15:** Full re-audit via Sieve brain against latest rules (captures any rule drift during engagement). AI-assisted keyword discovery pass 3 — input to Q2 scope.
- **W16:** 16-week measurement audit. **Second paid ads audit report.** Results review. Q2 scope recommendations. Dashboard + intel fully handed over to Ritwik as ongoing owner. **Week 16 decision gate.**

---

## Target Scenarios (not commitments)

All outcomes are **target scenarios** — illustrative ranges, subject to (a) baseline validation in Week 1 and (b) the execution and external dependencies listed in the next section. These are not guarantees.

| Dimension | Week 0 | Scenario: Conservative (Week 16) | Scenario: Upside (Week 16) |
|---|---|---|---|
| AI citation rate (50 queries × 4 engines) | Measured Week 1 | +3-5x baseline | +7-12x baseline |
| Page Citation Readiness (analysis score) | 55% | 80-85% | 88%+ |
| Organic traffic (total sessions) | Measured Week 1 | +30-40% | +50-70% |
| Branded search trend (GSC brand-term impressions) | Measured Week 1 | Trending up | Clear step-change |
| Featured snippets captured | Not measured | 3-7 new | 7-12 new |
| Schema depth (pages with MedicalBusiness + FAQPage) | Low | 15+ pages | 20+ pages |
| FAQ pairs live | 0 | 40-50 pairs | 50+ pairs |
| Referring domains | Measured Week 1 | +8-18 new | +18-35 new |
| Founder Live Dashboard + Sieve re-audit | None | Live + weekly re-audit | Live + alert loop operational |
| Paid ads audit reports | None | 2 reports delivered | 2 reports + adopted changes |

Concrete target ranges (replacing "conservative / upside") will be set after Week 1 baseline.

---

## Assumptions

Targets assume these conditions hold:

- Engineering capacity as committed (10-14 hrs/week across the engagement)
- Medical reviewer availability at a 48-hour content-approval SLA
- Legal review availability for comparison + regulatory-adjacent content (3-5 hrs total)
- Content team capacity (~20 hrs/week) during Weeks 7-14
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

| Role | Weeks 1-6 | Weeks 7-16 |
|---|---|---|
| Engineering | 10-14 hrs/week | 10-14 hrs/week |
| Content team | 5 hrs/week | 18-22 hrs/week |
| Medical reviewer | 3-5 hrs/week | 3-5 hrs/week |
| Legal reviewer | 2-3 hrs total | 2-3 hrs total |
| Ritwik (co-owner) | 4-6 hrs/week | 4-6 hrs/week |
| Sundeep (founder) | 3-4 hrs/week | 2-3 hrs/week |

If capacity is lower than the table, scope reduces proportionally. This is a meaningful client-side commitment and should be confirmed before kickoff.

---

## Operator Effort Estimates

**Arun's hours only** (scope + build + run) — the contracted commitment. Valeo-side hours are separate (see Resource Commitments). All totals include a **30% buffer** for review cycles, regulatory-review latency, re-crawl diagnostics, and healthcare-specific rework.

### Workstream 1 — Foundation Fix (Weeks 1-4)

| Activity |
|---|
| Root page content spec + structure (~2,500 words, medical-reviewed brief) |
| Schema @graph design (port + enhance from /en-ae/dubai) |
| Technical fix spec + engineering handoff (HSTS, Cache-Control, dateModified) |
| Staging review + pre-deploy QA across AI crawler user agents |
| Post-deploy AI crawl validation + re-index tracking |
| Person schema spec (founder + medical director, DHA credential display) |
| AggregateRating ↔ Trustpilot integration spec + TOS compliance review |
| Strategy calls + iteration |
| **Total: ~61 hrs (with 30% buffer)** |

### Workstream 2 — Content + E-E-A-T + Founder Community Authority (Weeks 4-14)

Frameworks + templates approach for on-site content. Founder-led, compliance-native community engagement for off-site authority. Brand-aware blog writer automation (full pipeline) deferred to Phase 2.

**On-site content + E-E-A-T:**

| Activity |
|---|
| FAQ sourcing methodology + PAA harvesting approach |
| FAQ editorial template + QA framework (50 pairs, batch review) |
| Top-5 city-page framework + page-level briefs |
| 2 comparison post frameworks + legal gate spec |
| Blog post editorial standards + brief templates (5-8 pieces) |
| E-E-A-T audit (medical authority surfacing across site) |
| Schema consistency QA across 10+ pages |
| Content iteration + medical-review coordination |

**Founder-led community authority:**

| Activity |
|---|
| Community compliance playbook (Valeo-specific, medical + legal reviewed) |
| Quora topic map + 15-20 founder-byline answer frameworks + editing pass |
| Reddit subreddit map + monthly post frameworks (~2 posts/month × 4 months) + editing pass |
| Google Business Profile + App Store review invitation flows (extend Trustpilot pattern) |
| Monthly community footprint audits + response coordination |

**Total: ~118 hrs (with 30% buffer)**

### Workstream 3 — Measurement + Competitive Intel + Paid Audit (Weeks 1-16)

Lightweight measurement ops feeding into the WS4 Founder Live Dashboard. Full Telegram alerts + full scraper pipeline deferred to Phase 2.

**Build phase (Weeks 1-3):**

| Activity |
|---|
| Baseline measurement harness (50 queries × 4 engines, scripted) |
| Lightweight competitive intel setup (4 competitors, semi-manual weekly check) |
| AI citation tracking (spreadsheet + prompts, not full pipeline) |
| Email alert rules + routing |

**Run phase (Weeks 2-16):**

| Activity |
|---|
| Weekly measurement Weeks 1-5, bi-weekly Weeks 6-16 |
| Competitor SERP + AI Overview tracking (same cadence) |
| 3 competitive gap deep-dives (Weeks 8, 11, 14) |
| AI-assisted keyword discovery (passes at W4, W10, W15) |
| 2 paid efficiency audit reports (W10, W16) |
| W16 measurement audit + ROI write-up + Q2 scope |
| Cross-workstream strategy alignment + Friday reports |

**Total: ~140 hrs (with 30% buffer)**

### Workstream 4 — Always-On Intelligence (Weeks 2-16)

Founder Live Dashboard, Sieve brain integration, schema drift + content recency automation, competitive change detection. The compounding infrastructure layer.

| Activity |
|---|
| Founder Live Dashboard build (multi-panel: appearance, rank, traffic, competitor gap, content health) |
| Sieve brain integration (API hookup, continuous Valeo page re-audit pipeline, rule-change ingestion from official docs) |
| Schema drift + validator automation (weekly scan across top 20+ pages) |
| Content recency triggers (page age, dead-link scan, E-E-A-T signal audit, citation rot detection) |
| Competitive page-diff + schema-diff + new-page detection + AI Overview trigger tracking |
| Dashboard iteration + founder/Ritwik feedback loop (W6, W10, W14) |
| Ongoing alert curation + tuning (~0.5 hrs × 14 weeks) |

**Total: ~95 hrs (with 30% buffer)**

### Operator engagement total

| Workstream | Total hrs (with 30% buffer) |
|---|---|
| WS1 — Foundation Fix | ~61 |
| WS2 — Content + E-E-A-T + Founder Community Authority | ~118 |
| WS3 — Measurement + Intel + Paid Audit | ~140 |
| WS4 — Always-On Intelligence (Dashboard + Sieve + automation) | ~95 |
| **Operator total (Arun)** | **~414 hrs** |

**Weekly load profile** (~26 hrs/week average over 16 weeks):

| Phase | Weeks | Avg hrs/week |
|---|---|---|
| Foundation + dashboard + Sieve integration build | W1-5 | ~28 |
| Schema + FAQ + community playbook + automation operational | W6-8 | ~27 |
| Content depth + community posting + first paid audit | W9-11 | ~26 |
| Content velocity + dashboard refinement + community cadence | W12-14 | ~24 |
| Close + re-audit + handover | W15-16 | ~21 |

Notes:
- Buffer is drawn down only as consumed; unused buffer rolls into Phase 2 scope discussions.
- If Week 1 baseline reveals materially different starting conditions, estimates are re-baselined before Week 3.
- WS4 infrastructure is built to outlive the engagement — Ritwik owns it post-W16 with the alert loop continuing to surface content + competitor + rule-change drift.
- **Deferred to Phase 2** (explicit, scoped separately): brand-aware blog writer pipeline build, Telegram alert infrastructure, Arabic content parity, press outreach at scale, additional city pages beyond top 5.

---

## Pricing

Pricing is intentionally deferred to the kickoff discussion. Three structures are possible:

- **Phased fee** — Foundation / Content+Authority / Measurement+Handover, each with a decision gate before the next unlocks
- **16-week retainer** — single monthly fee × 4 months, all deliverables included
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

### Week 5 gate — foundation complete
- New root page live in production
- Schema depth materially increased at root (specific block count set in Week 1 plan)
- Technical fixes shipped (HSTS, Cache-Control, `dateModified`)
- Indexing confirmed in GSC + Bing
- Medical director Person schema live with credentials
- Founder Live Dashboard v1 live; Sieve brain integration operational

If foundation is not substantially complete, Workstream 2 pauses and the delay is diagnosed before expansion.

### Week 10 gate — content + authority mid-point
- Schema depth live on 15+ pages
- 40+ FAQ pairs deployed
- Top 5 city pages upgraded
- 2 comparison posts shipped (legal-reviewed)
- First paid ads audit report delivered
- Sieve-driven drift alerts + schema drift detection operational
- AI citation rate direction vs Week 1 baseline assessed (direction, not absolute threshold)

If mid-point is materially behind, remaining scope is renegotiated before Weeks 11-14.

### Week 16 gate — engagement close
- Measured AI citation rate: **target >10%** across 50-query × 4-engine set (vs Week 1 baseline near 0%)
- Organic traffic vs Week 1 baseline (range agreed in Week 1)
- Founder Live Dashboard + Sieve re-audit loop fully operational and handed to Ritwik
- 2 paid ads audit reports delivered
- Full Sieve re-audit against latest rules completed
- Q2 scope recommendations documented

Outcome scenarios:
- **Base case:** core foundation + schema shipped; AI appearance rate crosses 5-10%; traffic gains within conservative range → reasonable success, extend if aligned.
- **Upside:** full scope shipped; AI appearance rate >10%; traffic gains at higher end → strong result, scale engagement.
- **Downside:** foundation slipped or citation direction unclear → honest debrief, diagnose gaps, adjust approach.

---

## Why This Scope Is Credible

1. **Baseline-first.** Week 1 measures before Week 3 ships. Targets anchor to measured starting points, not estimates.
2. **Analysis-grounded.** Every fix traces to a specific finding in the April 14 analysis.
3. **Compliance-native.** Medical review, DHA adherence, YMYL standards, and review-collection TOS are in the workflow, not added after.
4. **Conditional framing.** Outcomes are target scenarios with explicit dependencies — not commitments.
5. **Focused scope.** 4 workstreams. Arabic, press at scale, and the full blog writer automation pipeline explicitly deferred to Phase 2. Community engagement is in scope but gated by a compliance playbook, not ad-hoc.
6. **Paid ads stays with marketing team.** We audit efficiency; we do not duplicate execution.
7. **Compounding infrastructure.** WS4 (dashboard + Sieve integration + drift detection) outlives the engagement — Valeo keeps re-auditing against evolving LLM/SEO rules without continued operator time.
8. **Evidence over assertion.** Directional claims labeled as directional. Unmeasured values labeled as unmeasured.

---

## Next Steps

1. Sundeep reviews this scope draft
2. Discussion call: resource commitment confirmation, pricing structure selection, question resolution
3. Kickoff week of April 28 (if aligned)
4. Week 1 Task 1: measure baseline (50 queries × 4 engines) → target ranges locked
5. First decision gate: Week 5

---

**Prepared by:** Arun Sharma
**Contact:** [email]
**Document status:** Scope draft v4 — supersedes prior drafts
