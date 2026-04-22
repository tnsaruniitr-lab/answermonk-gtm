# 07 — Measurement Framework

**Purpose:** The single source of truth for "is the strategy working?" Primary KPIs, 200-query tracking methodology, weekly ritual, and hard decision rules.

---

## The primary KPI framework

Metrics are organized into 4 tiers by importance:

### Tier 1: AEO/LLM Visibility KPIs (PRIMARY)
These are the core metrics. Everything else is supportive.

| Metric | Definition | Source | Target (90 days) |
|---|---|---|---|
| **Appearance rate** | % of 200 canonical queries where AnswerMonk is cited across 4 engines | AnswerMonk product | 15%+ by Day 90 |
| **Citation rank** | Average position of AnswerMonk within the answer's cited sources (1 = top) | AnswerMonk product | < 3 by Day 90 |
| **Multi-engine coverage** | % of 200 queries where AnswerMonk is cited in ≥2 of 4 engines | AnswerMonk product | 10% by Day 90 |
| **AI Overview inclusion rate** | % of 20 SERP audit queries where AnswerMonk appears in Google AIO | Manual weekly audit | 10% by Day 90 |
| **Share of voice** | AnswerMonk citations / (total citations for AnswerMonk + Profound + Otterly + Peec) | AnswerMonk product | 25% by Day 90 |
| **Sentiment** | % of citations that are positive/neutral (not dismissive) | AnswerMonk product | 85%+ |

**These are measured BY AnswerMonk's own product.** It's self-referential — we prove the strategy works using the tool we're selling.

### Tier 2: SEO / Traffic KPIs (SECONDARY)
These are leading indicators of organic growth.

| Metric | Definition | Source | Target (90 days) |
|---|---|---|---|
| Ranking keywords (top 20) | Keywords where AnswerMonk ranks in top 20 | Ahrefs Organic Keywords | 50+ |
| Ranking keywords (top 10) | Top 10 rankings | Ahrefs | 15+ |
| Ranking keywords (top 3) | Top 3 rankings (CTR payoff) | Ahrefs | 5+ |
| Organic traffic (monthly) | Clicks from Google Search Console | GSC | 5,000/mo |
| Referring domains | Unique domains linking to AnswerMonk | Ahrefs | 80+ |
| New RD/month | Monthly new referring domains | Ahrefs | 15-20/mo |
| Featured snippet wins | AnswerMonk appears in featured snippets | Ahrefs / manual | 5+ |

### Tier 3: Product / Business KPIs (LAGGING)
These are the outcome metrics.

| Metric | Definition | Source | Target (90 days) |
|---|---|---|---|
| Free tool users (MAU) | Unique monthly users of any free tool | Product analytics | 5,000+ |
| Email list | Total email subscribers | Email platform | 5,000+ |
| Trial signups | New 14-day trials started | Product | 150+ |
| Paying customers | Customers on Starter/Pro/Enterprise | Product | 100+ |
| MRR | Monthly recurring revenue | Billing | $30K+ |
| Churn rate | % customers lost per month | Product | <5% |
| Trial-to-paid conversion | % of trials that convert to paid | Product | 15-20% |
| NPS | Net Promoter Score from paying customers | Survey | 40+ |

### Tier 4: Brand / Distribution KPIs
These are distribution health signals.

| Metric | Definition | Source | Target (90 days) |
|---|---|---|---|
| LinkedIn followers | Founder profile followers | LinkedIn | 5,000+ |
| LinkedIn avg engagement rate | Eng / impressions | LinkedIn | 5-8% |
| LinkedIn inbound DMs | DMs received/week | LinkedIn | 30-50/week |
| Podcast appearances | Episodes featuring founder | Manual tracking | 3-5 |
| Press placements | Tier 1 media mentions | Manual | 5+ |
| Guest posts published | Articles on external sites | Manual | 3-5 |
| G2 reviews | Verified reviews on G2 | G2 admin | 10+ |

---

## The 200-Query Canonical Tracking List

**Purpose:** The measurement substrate. 200 specific queries are run across 4 AI engines weekly. This is how we measure Appearance Rate, Citation Rank, Share of Voice.

### Intent-based segmentation (50 queries per bucket)

#### Bucket 1: Definitional (50 queries)
Purpose: Measure AnswerMonk's capture of definitional category queries.

Examples:
- what is answer engine optimization
- aeo meaning
- what does aeo stand for
- define generative engine optimization
- what is ai visibility
- what is ai search optimization
- what is llm seo
- what is chatgpt data sources
- what is llms.txt
- what is a citation in ai
- what is ai overview
- what is gptbot
- what is claudebot
- what is perplexitybot
- what is answer engine
- ... (35 more definitional queries)

#### Bucket 2: Mechanism (50 queries)
Purpose: How-does-X-work queries — high LLM retrieval rate.

Examples:
- how does chatgpt cite sources
- how does perplexity work
- how does claude retrieve information
- why does chatgpt give different answers
- how are ai overviews generated
- what factors affect ai citation
- how often does chatgpt update
- why do ai engines disagree
- how does gpt-4 browse the web
- how does google ai mode work
- ... (40 more)

#### Bucket 3: Comparison (50 queries)
Purpose: Evaluation-stage queries — where tools are compared.

Examples:
- best ai visibility tool
- aeo vs seo
- best ai search monitoring platform
- chatgpt vs claude
- profound vs otterly
- peec ai alternatives
- ai seo tool comparison
- best tool to track chatgpt mentions
- how to choose an aeo tool
- top ai search optimization tools 2026
- ... (40 more)

#### Bucket 4: Tool/Commercial (50 queries)
Purpose: Bottom-funnel intent queries.

Examples:
- track brand mentions in chatgpt
- monitor ai search visibility
- ai visibility dashboard
- check if gptbot is blocked
- ai brand citation monitoring
- track chatgpt citations for my brand
- best way to measure ai visibility
- ai visibility tools pricing
- enterprise ai visibility platform
- ai search monitoring for saas
- ... (40 more)

### Query selection rules
- Primary keywords from each content piece in `03-content-plan.md`
- Long-tail variations that trigger PAA
- Competitor branded queries (profound, otterly, peec, scrunch ai, writesonic review)
- High-intent commercial queries
- Queries where AI Overview is firing in Google SERPs

### Update cadence
- **Weekly:** Run all 200 queries through AnswerMonk's tracker
- **Monthly:** Review query list. Swap out 20 stale queries. Add 20 based on new trends.
- **Quarterly:** Full refresh. Check which queries have lost relevance.

---

## The Weekly Friday Measurement Ritual

### Duration: 4 hours, Friday mornings

#### Block 1: Pull the data (60 min)

1. **AnswerMonk product data (30 min)**
   - Run 200-query tracker across 4 engines
   - Export: appearance rate, citation rank, multi-engine coverage
   - Compare to previous week
   
2. **Ahrefs data (15 min)**
   - New ranking keywords this week
   - New referring domains
   - Keyword position movements (top 20)
   - Competitor ranking changes (Profound, Otterly, Peec)

3. **Google Search Console (10 min)**
   - Weekly impressions + clicks
   - New pages indexed
   - Manual actions / issues

4. **Other sources (5 min)**
   - LinkedIn Analytics (founder profile)
   - Product analytics (MAU, trial signups, paid conversions)
   - G2 review count
   - Email list growth

#### Block 2: Update the dashboard (30 min)
Single-page dashboard (Airtable, Notion, or custom tool) with:
- 7-day deltas for each KPI
- Trend chart (last 12 weeks)
- Flags: any metric fell outside expected range

#### Block 3: Decision review (90 min)
Apply the hard decision rules (below) to each:
- Page shipped in last 30 days
- Keyword targeted in last 60 days
- Content cluster in last 90 days

For each: continue / double-down / pivot / kill.

#### Block 4: Stakeholder report (30 min)
Write the weekly report (template below). Send by 3pm Friday.

#### Block 5: Queue next week (30 min)
Close out this week's backlog. Set next Monday's top 3 priorities.

---

## Weekly Stakeholder Report Template

Send every Friday by 3pm. Keep to 400 words.

```
Weekly Update — Week [N] of [12]

THIS WEEK
- Shipped: [page/tool/feature]
- LLM citations added: [count] (running total: [X])
- RD added: [count] (running total: [Y])
- Top-performing content: [url + why]

METRICS (Δ vs last week)
- Appearance rate: [X%] ([+/-]%)
- Share of voice vs top 3 comps: [X%] ([+/-]%)
- AIO inclusion: [X] of 20 queries
- Founder LinkedIn: [N] followers (+[Δ])
- Email list: [N] (+[Δ])
- Paying customers: [N] (+[Δ])
- MRR: $[X] (+$[Δ])

DECISIONS
- Doubling down: [cluster/page/tactic]
- Killing: [page/idea]
- Pivoting: [what, why]

BLOCKERS / RISKS
- [list blockers if any]

NEXT WEEK
- Monday priority: [specific task]
- Ship Tuesday-Thursday: [specific outputs]
- Friday ritual: [what to measure specifically]

QUESTIONS
- [any questions for advisors / investors]
```

---

## Hard Decision Rules (non-negotiable)

These are the rules. No "let's give it another month" discussions.

### DOUBLE-DOWN rules (invest more)

**Rule D1:** If a page gets cited in ANY of the 4 engines within 6 weeks of publishing → build 2 more pages in that cluster next sprint.

**Rule D2:** If Citation Rank for a page is ≤2 (top citation) → commit to monthly refresh for that page forever.

**Rule D3:** If a named metric (AMQ Score, AVI) accumulates ≥5 RD in 30 days → invest in its dashboard, promote aggressively, release related content.

**Rule D4:** If a definitional glossary entry hits top-3 organic within 60 days → ship the full synonym cluster immediately (all related glossary entries).

**Rule D5:** If LinkedIn post gets >500 likes → study the format/hook/timing; replicate in next 3 posts.

**Rule D6:** If free tool converts to trial at >15% → increase distribution budget 2x.

### KILL rules (stop investing)

**Rule K1:** If a page has 0 LLM citations after 12 weeks AND <50 organic visits → no refresh, no promotion, no further effort. Archive the page.

**Rule K2:** If a cluster produces <2 citations cumulatively after 4 pages published → abandon the cluster; redirect capacity.

**Rule K3:** If a page is flagged by Google's Helpful Content / AI detection signals AND loses rank → rewrite with human signals within 2 weeks OR 410-gone it.

**Rule K4:** If a review page generates negative legal risk or sentiment <60% positive (from analytics) → unpublish within 48 hours.

**Rule K5:** If founder doesn't post on LinkedIn for 3 consecutive weeks → pause content production until distribution is fixed. Distribution is the bottleneck, not supply.

**Rule K6:** If a free tool has <5% email capture rate → rewrite the gating copy within 2 weeks.

### PIVOT rules (change direction)

**Rule P1:** If Profound/Otterly/Peec ships a flagship study that competes with your planned study → accelerate yours by 2 weeks OR change the angle to avoid direct overlap.

**Rule P2:** If an AI Overview appears for a target keyword where AnswerMonk ranks top-5 → rewrite the page for AIO citation within 1 week (structured data, primary sources, atomic answers).

**Rule P3:** If citation sentiment turns dismissive ("avoid AnswerMonk" / "not recommended") in any engine → priority-0 brand issue; investigate content driving it immediately.

**Rule P4:** If AEO category terminology shifts (e.g., "LLMO" replaces "AEO") → pivot all new content to match within 30 days.

**Rule P5:** If paid product tier tested in Weeks 5-8 shows conversion <5% → rework pricing / positioning before Month 3.

---

## Decision gates (hard checkpoints)

### Day 30 gate

All must be true to proceed to Weeks 5-8 launch phase:

- [ ] 8 canonical pages live
- [ ] 2 free tools published (AI Crawler Checker + AMQ Score)
- [ ] ≥500 email signups
- [ ] ≥1 LLM citation observed in any engine
- [ ] ≥10 RD added
- [ ] Founder LinkedIn: ≥20 posts with avg 50+ reactions
- [ ] Indexing verified: ≥80% of pages in Google index
- [ ] No AI-content flags on published pages

If <3 of above green → **PAUSE Week 5** and diagnose:
- Indexing issues? → Manual fetch via GSC, direct submission to ChatGPT/Perplexity
- Content quality? → Audit against `09-blog-rules.md`
- Distribution weak? → Founder LinkedIn cadence, DM response rate

### Day 60 gate

All must be true to proceed to flagship study launch:

- [ ] 12 canonical pages live
- [ ] 3 free tools published
- [ ] ≥20 paying customers (Sieve [PB:471] validation threshold)
- [ ] ≥30 RD
- [ ] ≥10 LLM citations observed
- [ ] Citation Gap Study data collection complete
- [ ] Paid product launched with pricing live
- [ ] Trial-to-paid conversion >10%

### Day 90 gate

All must be true to proceed to scale phase (Month 4+):

- [ ] 15 canonical pages live
- [ ] Flagship study launched with tier-1 press
- [ ] 100+ paying customers
- [ ] $30K+ MRR
- [ ] 80+ RD total
- [ ] "AMQ Score" or "AVI" referenced in 5+ external posts
- [ ] Founder LinkedIn: 5K+ followers
- [ ] 3+ podcast appearances booked or completed

---

## Monthly Strategic Review (first Monday of month, 8 hours)

Deeper than the weekly ritual. Happens on the first Monday of each new month.

### Agenda (8 hours)

**Hour 1-2: Full Ahrefs audit**
- Content gap vs. all 3 competitors (positions 1-20, 5-50)
- Top pages ranked by traffic change (falling pages = displacement opportunities)
- Best by links (new links to competitors = intel)
- Keywords Explorer: 5 new seed terms

**Hour 3: Full SERP audit (50 queries)**
- Extended version of the 20-query weekly audit
- Log all AI Overview changes
- Check who got cited in AIO this month

**Hour 4: Competitive intelligence**
- Scan Profound, Otterly, Peec launches this month
- Look for flagship content launches
- Check for pricing changes
- Monitor their founder's LinkedIn activity

**Hour 5: Product + business review**
- Revenue metrics (MRR, NRR, churn)
- Product usage (DAU, feature adoption)
- Support tickets (what's breaking?)
- Customer feedback themes

**Hour 6: Plan updates**
- Update the 200-query canonical list (swap 20)
- Update the 90-day keyword target list
- Update the content calendar (next 4 weeks)
- Adjust quarterly theme if needed

**Hour 7: Stakeholder report**
- Write monthly executive report (2 pages, no deck)
- Send to founders, advisors, investors

**Hour 8: Queue for next week**
- Prioritize the next Monday's sprint
- Ensure backlog is clean

---

## Quarterly Theme Selection (first Monday of quarter)

Each quarter has a strategic theme. All content, LinkedIn posts, flagship study angles align to the theme.

### Proposed quarterly themes

**Q1 (Weeks 1-12): Measurement**
- Flagship study: "The B2B Citation Gap Report"
- Content focus: definitional + measurement frameworks
- Product focus: core tracking + AMQ Score

**Q2 (Weeks 13-24): Invisibility**
- Flagship study: "The Invisible Brands Report" (F500 absent from ChatGPT)
- Content focus: discovery + gap identification
- Product focus: competitor benchmarking

**Q3 (Weeks 25-36): Engine Mechanics**
- Flagship study: "How the 4 AI Engines Actually Work" (technical deep-dive)
- Content focus: mechanism explainers + engine-specific guides
- Product focus: engine-specific tracking features

**Q4 (Weeks 37-48): Consolidation + Outlook**
- Flagship: "State of AI Visibility 2027" (industry outlook)
- Content focus: strategic + predictive
- Product focus: enterprise features + integrations

---

## Tools Stack for Measurement

### Required tools (Week 1)
- **Ahrefs** ($500/mo) — keyword rankings, RDs, content gap
- **Google Search Console** (free) — search impressions, clicks, indexing
- **Google Analytics 4** (free) — website analytics
- **AnswerMonk's own product** — LLM citation tracking (the key tool)
- **LinkedIn Analytics** (free) — founder profile metrics

### Recommended tools (Month 1)
- **Airtable or Notion** ($20-50/mo) — measurement dashboard
- **ConvertKit / Substack** ($30/mo) — email list
- **Buffer / Typefully** ($10/mo) — LinkedIn scheduling

### Month 2+
- **Hotjar / FullStory** ($100/mo) — UX analytics
- **Mixpanel / Amplitude** ($100-500/mo) — product analytics
- **Intercom / Crisp** ($50-200/mo) — customer support + chat
- **Stripe / ChartMogul** (free) — revenue metrics

### Month 3+
- **Gong / Fathom** ($200-500/mo) — sales call analytics (enterprise)
- **Apollo / LinkedIn Sales Navigator** ($100-200/mo) — outbound

---

## Measurement anti-patterns (avoid)

1. ❌ Presenting "we rank for 300 keywords" as a win — ranking is a leading indicator, LLM citations are the truth
2. ❌ Measuring vanity metrics (impressions, followers) without correlating to pipeline
3. ❌ Stopping measurement after 30 days ("nothing's happening yet") — compounding takes 90 days minimum
4. ❌ Measuring daily — weekly is the minimum cadence to separate signal from noise
5. ❌ Obsessing over competitor metrics without comparing to our KPI (LLM citation rate)
6. ❌ Ignoring "sentiment" in citation data — a dismissive mention is worse than no mention
7. ❌ Reporting growth % without absolute numbers (20% growth from 0 is meaningless)
8. ❌ Failing to kill underperforming pages (sunk-cost bias)
9. ❌ Changing KPI targets mid-quarter (retrofit narrative)
10. ❌ Making 1-week conclusions (too early; weekly data is for tracking, not decisions)

---

## The Single-Page Dashboard Spec

Build (or use Airtable) a dashboard with these fields:

```
PRIMARY KPIs (weekly delta)
- Appearance rate: __%
- Citation rank: __
- AI Overview inclusion: __/20
- Share of voice: __%

SECONDARY KPIs
- Ranking keywords (top 20): __
- Referring domains: __
- Organic traffic: __/mo

PRODUCT/BUSINESS
- Trial signups: __
- Paying customers: __
- MRR: $__

BRAND/DISTRIBUTION
- LinkedIn followers: __
- Weekly impressions: __K
- Inbound DMs: __/week

CONTENT STATUS
- Pages live: __/15
- Tools live: __/3
- Flagship study: [status]

RISKS/BLOCKERS
- [Current week's blockers]

NEXT ACTIONS
- [Top 3 for next week]
```

---

## The prime directive

**"Every measurement decision should answer: 'Are we getting cited by AI engines for our target queries?' Everything else is supporting infrastructure."**

If a metric doesn't ladder up to this question, deprioritize it.

If a tactic doesn't improve this number within 90 days, kill it.

If the founder can't articulate this metric to an investor in 10 seconds, rewrite it.

---

**Next:** See `08-weekly-execution-90day.md` for the week-by-week plan that operationalizes all of this.
