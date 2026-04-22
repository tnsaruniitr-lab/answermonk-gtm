# 03 — Content Plan (15 Canonical Pages with Full Briefs)

**Purpose:** Every page AnswerMonk ships in the first 90 days. Full briefs with URLs, titles, keywords, word counts, schema, and publish dates.

**Cadence:** 2 canonical pages per week for Weeks 1-6, then 1 per week for Weeks 7-12. Total: 15 pages by end of Week 12.

---

## Content Tier Hierarchy

```
Tier A — Pillars (5,000+ words, category-defining)
  - Canonical reference for major category terms
  - Update quarterly
  - Internal linking hub

Tier B — Supporting posts (1,500-2,500 words)
  - Deep-dive on specific sub-topics
  - Cluster around pillars
  - Update semi-annually

Tier C — Glossary entries (500-1,000 words)
  - Single term definitions
  - Lightweight but essential
  - Update annually

Tier D — Tool pages (varies)
  - Landing + educational content for free tools
  - Update as tool evolves
```

---

## The 15 Canonical Pages

### PAGE 1 — Category Pillar (Tier A)

**URL:** `/glossary/answer-engine-optimization`

**Title:** What Is Answer Engine Optimization (AEO)? The Complete 2026 Guide

**Primary keyword:** answer engine optimization (3,400/mo, KD 38)
**Secondary keywords:** what is aeo, aeo meaning, what does aeo stand for, aeo definition

**Publish date:** Week 1, Thursday

**Template:** A (Definitional) + F (FAQ) + pillar structure

**Word count target:** 2,500-3,000

**Structure:**
- H1: "What Is Answer Engine Optimization (AEO)? The Complete 2026 Guide"
- TL;DR block: 50-word definition with `<dfn>` on AEO
- H2: What is Answer Engine Optimization? (core definition + 3-paragraph explanation)
- H2: AEO vs SEO vs GEO: Key Differences (5-col comparison table)
- H2: Why AEO Matters in 2026 (market stats, specific AI engine share)
- H2: How AEO Works: The 4 Key Mechanisms (retrieval, citation selection, ranking, freshness)
- H2: AEO Signals: What AI Engines Actually Look For (entity density, schema, primary sources, freshness)
- H2: How to Implement AEO: A 7-Step Framework (numbered ordered list)
- H2: Common AEO Mistakes (anti-patterns)
- H2: AEO Tools Comparison (table with AnswerMonk, Profound, Otterly, Peec)
- H2: Measuring AEO Success (link to AMQ Score)
- H2: The Future of AEO (predictions, 2027 outlook)
- H2: FAQ (10 questions harvested from live SERP PAA)

**Schema required:**
- Article / BlogPosting
- DefinedTerm + DefinedTermSet (for AEO term)
- FAQPage (for FAQ block)
- BreadcrumbList

**Required elements:**
- 40-word TL;DR in `<p data-tldr>`
- Comparison table (AEO vs SEO vs GEO)
- Numbered 7-step framework
- 8-10 FAQ questions with direct answers
- Author byline (founder: Arun Sharma with LinkedIn sameAs)
- 5+ outbound primary citations (OpenAI docs, Google Search Central, arXiv, Gartner)
- Visible "Last updated: [date]" + `dateModified` in schema
- Original hero image/diagram (NOT AI-generated)

**Success criteria:**
- Top-10 ranking within 90 days on primary keyword
- First LLM citation observed within 60 days
- 10+ internal links pointing to this page from other content

---

### PAGE 2 — Glossary Foundation (Tier C, multi-entry)

**URL base:** `/glossary/aeo` `/glossary/geo` `/glossary/llmo` `/glossary/ai-visibility` `/glossary/ai-citation` `/glossary/aieo` `/glossary/ai-search` `/glossary/answer-engine`

**Publish date:** Week 1 (ship 4), Week 3 (ship 4 more) — 8 glossary entries total

**Template:** A (Definitional)

**Word count target:** 600-900 each

**Structure (standard for all glossary entries):**
- H1: What Is [Term]?
- TL;DR: 40-word complete definition
- H2: Definition (formal 50-word definition with synonyms)
- H2: [Term] vs Related Concepts (short comparison)
- H2: How [Term] Works (mechanism, 2-3 paragraphs)
- H2: [Term] in Practice (concrete example with named brand)
- H2: Tools for [Term] (brief mention + link to AnswerMonk)
- H2: FAQ (5 questions from PAA)

**Schema required:**
- DefinedTerm (primary)
- DefinedTermSet (link all glossary entries)
- FAQPage
- Article

**Required elements:**
- `<dfn>` tag around term on first use
- `<abbr title="[full form]">` for acronyms
- "Also known as" block listing synonyms
- Link to parent pillar (`/glossary/answer-engine-optimization`)
- 3+ primary source citations
- Author byline

**Example: /glossary/aeo**

- H1: What Is AEO? (Answer Engine Optimization Explained)
- TL;DR: "Answer Engine Optimization (AEO) is the practice of optimizing content so that AI chatbots like ChatGPT, Claude, and Perplexity cite your brand when answering user questions. Unlike SEO, which targets search engine rankings, AEO targets AI-generated answer boxes."
- Sections on: definition, synonyms (AIEO, GEO), how it works, examples, tools, FAQ

---

### PAGE 3 — Comparison Post (Tier B)

**URL:** `/blog/aeo-vs-seo-geo`

**Title:** AEO vs SEO vs GEO: The 2026 Comparison (Which Should You Optimize For?)

**Primary keyword:** aeo vs seo (1,500/mo, KD 12)
**Secondary keywords:** aeo vs geo, seo for ai, ai search seo, what is aeo vs seo

**Publish date:** Week 1, Friday

**Template:** B (Comparison) + F (FAQ)

**Word count target:** 1,800-2,200

**Structure:**
- H1: AEO vs SEO vs GEO: The 2026 Comparison
- TL;DR: 1-sentence verdict + who should care
- H2: Quick Comparison: AEO vs SEO vs GEO (4-column × 8-row table)
- H2: What Is SEO? (150-word section)
- H2: What Is AEO? (150-word section)
- H2: What Is GEO? (150-word section)
- H2: Side-by-Side: Key Differences
  - H3: Primary Goal
  - H3: Target Surface
  - H3: Success Metric
  - H3: Optimization Unit
  - H3: Content Style
- H2: Can You Do All Three? (yes, with examples)
- H2: Decision Framework: Which to Prioritize (flowchart / decision tree)
- H2: Tools for Each (listing with brief descriptions)
- H2: The Future: Will AEO Replace SEO? (contrarian POV)
- H2: FAQ (6 PAA questions)

**Schema:** Article + FAQPage + BreadcrumbList

**Required elements:**
- Comparison table as first visual element
- Each table row has "verdict" column (LLMs cite verdicts)
- Decision tree diagram (original SVG, not AI-generated)
- 5+ primary citations
- Author POV section ("Our view on the AEO vs SEO debate")

**Success criteria:**
- Rank top-5 for "aeo vs seo" within 60 days (KD 12 = achievable)
- 5+ RD from comparison-content backlinks within 90 days

---

### PAGE 4 — AI Overview Displacement (Tier B)

**URL:** `/blog/chatgpt-data-sources`

**Title:** ChatGPT Data Sources: The Complete Reference (Updated 2026)

**Primary keyword:** chatgpt data sources (target Ahrefs didn't expose volume; Profound dropped 1→10 when AIO launched)
**Secondary keywords:** chatgpt training data, what data does chatgpt use, gpt-4 training sources

**Publish date:** Week 2, Tuesday

**Template:** A + E (Definitional + Dataset)

**Word count target:** 1,800-2,500

**Structure:**
- H1: ChatGPT Data Sources: Complete Reference
- TL;DR: 40-word summary of the 4 main source categories
- H2: ChatGPT's Training Data (pre-training corpus)
- H2: ChatGPT's Retrieval Sources (browsing mode / RAG)
- H2: Publisher Partnerships (OpenAI deals with AP, FT, etc.)
- H2: User-Generated Content Sources (Reddit, forums)
- H2: **The Complete ChatGPT Source Table** (10+ rows: Source type | Dataset | Size | Confirmed by | Date | Evidence URL)
- H2: What's NOT in ChatGPT's Training Data (explicitly excluded content)
- H2: How to Check if Your Site Is Being Crawled (practical how-to with code samples)
- H2: Optimizing for ChatGPT Retrieval (5 actionable tips)
- H2: FAQ (5 PAA questions)

**Schema:** Article + Dataset + FAQPage + HowTo

**Required elements:**
- **The source table** — 10+ rows with evidence URLs (this is what AIO will cite)
- Primary citations: OpenAI model system card, GPT-4 technical report (arXiv), 3 Reddit threads, official partnership press releases
- DefinedTerm for "training data" and "RAG"
- Last-updated stamp with commitment to quarterly refresh

**AI Overview displacement requirements:**
- Static HTML only (no JS rendering for the table)
- Table must use proper `<table>` with `<th scope="col">`
- First sentence under each H2 = complete answer
- 40-word TL;DR extractable as paragraph

**Success criteria:**
- AI Overview citation within 12 weeks
- Position 1-5 on Google within 90 days

---

### PAGE 5 — Canonical Reference (Link Magnet, Tier B)

**URL:** `/blog/llms-txt`

**Title:** llms.txt: The Complete Technical Reference (Updated [Month] 2026)

**Primary keyword:** llms.txt
**Secondary keywords:** llms.txt specification, llms txt adoption, ai crawler directive

**Publish date:** Week 2, Thursday

**Template:** Custom (canonical technical reference)

**Word count target:** 2,000-2,500

**Structure:**
- H1: llms.txt: The Complete Technical Reference
- TL;DR: "llms.txt is a proposed standard for informing LLM crawlers which content to index. As of [Month Year]: [X] sites have adopted, [Y] engines honor it."
- H2: What Is llms.txt?
- H2: **Adoption Tracker** (live-updated table: Engine | Status | Last Tested | Evidence URL)
  - Rows: ChatGPT / GPT-4, Claude, Gemini, Perplexity, Grok, DeepSeek, Mistral, Cohere, Google-Extended, CCBot
- H2: How llms.txt Differs from robots.txt
- H2: Writing Your llms.txt (code samples)
- H2: How to Test Adoption (test methodology)
- H2: Should You Add llms.txt to Your Site? (decision criteria)
- H2: The Future of llms.txt (speculation, next steps)
- H2: FAQ

**Schema:** TechArticle + HowTo + FAQPage

**Required elements:**
- **The adoption tracker table** (THIS IS THE PAGE'S PURPOSE)
- Code examples with syntax highlighting
- Test methodology documented
- Monthly refresh commitment (dateModified updates)
- Submit to Hacker News on first monthly refresh (not launch — timing matters)

**Success criteria:**
- 30-80 RD in 6 months (Peec's abandoned post had similar potential)
- Top-3 Google ranking within 60 days
- Hacker News front page potential

---

### PAGE 6 — Named Metric Launch (Tier A equivalent — Tool + Content)

**URL:** `/amq-score` (also acts as free tool page — see `04-free-tools.md`)

**Title:** AMQ Score: Measure Your Brand's AI Visibility (Free Score)

**Primary keyword:** search visibility score (450, KD 20)
**Secondary keywords:** ai visibility score, measure ai visibility, brand ai citation rate

**Publish date:** Week 3, Wednesday

**Template:** E (Metric/formula) + Tool page

**Word count target:** 2,000-3,000

**Structure:**
- H1: AMQ Score: The Industry Standard for AI Visibility Measurement
- TL;DR: "AMQ Score (AnswerMonk Visibility Score) measures how often your brand is cited by ChatGPT, Claude, Perplexity, and Google AI Mode. Average for B2B SaaS: [X]. Top 10%: [Y]+."
- **Interactive calculator widget** (paste domain → get AMQ Score)
- H2: What Is AMQ Score?
- H2: How AMQ Score Is Calculated (the formula)
  - Formula: `AMQ = (Citation Frequency × Position Weight × Engine Coverage × Sentiment) × 100`
- H2: Industry Benchmarks (table by vertical)
- H2: How to Interpret Your Score (ranges + meaning)
- H2: How to Improve Your AMQ Score (7 actionable steps)
- H2: AMQ Score vs. Other Metrics (comparison with Domain Authority, Share of Voice)
- H2: The Research Behind AMQ (methodology, sample size)
- H2: FAQ

**Schema:** SoftwareApplication + Dataset + DefinedTerm + Article + FAQPage

**Required elements:**
- Functional calculator widget (JS is fine on tool itself, but core content + benchmarks must be SSR)
- Named formula with variables defined
- Industry benchmark table (from AnswerMonk's product data across 500+ brands)
- Email gate for "full report" (Starter tier conversion path)
- Day-1 distribution: DM 15 influencers on LinkedIn

**Success criteria:**
- 15-30 RD within 6 months (from writers/consultants forced to reference metric)
- 500+ calculator uses in first month
- First public mention of "AMQ Score" by external writer within 90 days

---

### PAGE 7 — Procedural (Tier B)

**URL:** `/blog/how-to-rank-in-ai-overviews`

**Title:** How to Rank in Google AI Overviews: 7 Steps That Actually Work (2026)

**Primary keyword:** how to rank in ai overviews (600, KD 12)
**Secondary keywords:** how to show up in ai overviews seo (700, KD 3), how to get in ai overview

**Publish date:** Week 3, Friday

**Template:** C (Procedural / HowTo)

**Word count target:** 1,500-2,000

**Structure:**
- H1: How to Rank in Google AI Overviews: 7 Steps (2026)
- TL;DR: The 7-step framework in 40 words
- H2: What Is a Google AI Overview?
- H2: Why Ranking in AI Overviews Matters (stats on AIO frequency)
- H2: **The 7-Step Framework**
  - H3: Step 1: Structure content for extraction (structured data, schema)
  - H3: Step 2: Own the TL;DR slot (40-word extractable answers)
  - H3: Step 3: Build entity authority (author byline, E-E-A-T)
  - H3: Step 4: Cite primary sources (reciprocity effect)
  - H3: Step 5: Maintain freshness (dateModified, quarterly refresh)
  - H3: Step 6: Target the right queries (question-format keywords)
  - H3: Step 7: Measure and iterate (with AnswerMonk)
- H2: Common Mistakes That Get You Excluded from AIO
- H2: AI Overview Ranking Factors (what research shows)
- H2: Tools to Monitor Your AIO Presence (AnswerMonk CTA)
- H2: FAQ

**Schema:** HowTo + HowToStep + FAQPage + Article

**Required elements:**
- Odd number of steps (7 cites better than 6 or 8)
- Each step 25-40 words
- Real SERP screenshots showing AIO examples
- Embedded AMQ Score CTA mid-article
- Original data: "We analyzed N AI Overviews, X% of cited pages had schema"

**Success criteria:**
- Top-5 ranking within 60 days
- Co-ranks or outranks Otterly's current #1 post

---

### PAGE 8 — Monitoring Guide (Product-Led, Tier B)

**URL:** `/blog/how-to-monitor-ai-search-visibility`

**Title:** How to Monitor AI Search Visibility: The 2026 Playbook

**Primary keyword:** how to monitor ai search visibility (300, KD 6)
**Secondary keywords:** why should i track ai brand visibility (350, KD 1), track ai brand mentions, monitor chatgpt brand mentions

**Publish date:** Week 4, Tuesday

**Template:** C (Procedural) + product-adjacent

**Word count target:** 1,500-2,000

**Structure:**
- H1: How to Monitor AI Search Visibility: The 2026 Playbook
- TL;DR: 40-word 5-step framework
- H2: Why Monitor AI Search Visibility?
  - Market shift stats
  - Cost of ignoring
- H2: What to Monitor (the 5 core metrics)
- H2: **How to Track Brand Mentions in ChatGPT** (manual + automated)
- H2: How to Track Claude Citations
- H2: How to Track Perplexity Mentions
- H2: How to Track Google AI Overviews
- H2: Setting Up a Multi-Engine Tracking System (here's where AnswerMonk fits)
- H2: Frequency: Daily vs Weekly vs Monthly
- H2: The AMQ Score: Unified AI Visibility Metric
- H2: FAQ

**Schema:** HowTo + HowToStep + SoftwareApplication (for AnswerMonk mention)

**Required elements:**
- Product screenshots of AnswerMonk naturally embedded
- AMQ Score CTA
- Comparison of manual vs automated tracking
- Free 14-day trial CTA at end

---

### PAGE 9 — Mechanism Research (AEO-High, Tier B)

**URL:** `/blog/why-chatgpt-different-answers`

**Title:** Why Does ChatGPT Give Different Answers to the Same Question? (We Ran It 10,000 Times)

**Primary keyword:** why does chatgpt provide different answers (Otterly currently ranks #1, weak content)
**Secondary keywords:** does chatgpt give same answer to everyone, does chat gpt generate same responses, chatgpt answer variance

**Publish date:** Week 4, Thursday

**Template:** Original research + mechanism explainer

**Word count target:** 2,000-2,500

**Structure:**
- H1: Why Does ChatGPT Give Different Answers to the Same Question? (Original Research)
- TL;DR: The 4 mechanisms + our experiment findings
- H2: The Experiment: 10,000 Queries, 4 Models (methodology)
- H2: **Variance Stats** (table with: Model | Avg. Agreement Rate | Top Variance Query | Confidence Score)
- H2: Mechanism 1: Temperature (explanation + data)
- H2: Mechanism 2: RAG Freshness (explanation + data)
- H2: Mechanism 3: User Context (explanation + data)
- H2: Mechanism 4: Model Version Drift (explanation + data)
- H2: How to Reduce Answer Variance (for marketers)
- H2: What This Means for Brand Monitoring
- H2: FAQ

**Schema:** Article + Dataset + FAQPage

**Required elements:**
- Original experiment data (AnswerMonk runs this)
- Charts showing variance distribution
- Primary citations: OpenAI temperature docs, academic papers on LLM determinism
- Author byline + methodology section

**Success criteria:**
- Outrank Otterly's current #1 post within 90 days
- First-party data establishes AnswerMonk as research authority
- 20+ RD from researchers/writers citing the variance data

---

### PAGE 10 — Review (Commercial, Tier B)

**URL:** `/reviews/profound`

**Title:** Profound AI Review (2026): Honest Take from an AI Visibility Competitor

**Primary keyword:** profound ai, profound review
**Secondary keywords:** profound alternative, profound pricing, tryprofound review

**Publish date:** Week 5, Tuesday

**Template:** Balanced review (D-adjusted — NOT hit-piece)

**Word count target:** 1,800-2,200

**Structure:**
- H1: Profound AI Review (2026): Honest Take from a Competitor
- **Transparency disclosure at top:** "We're AnswerMonk, a competing tool. We've tried to make this review as honest as possible."
- TL;DR: Neutral 1-sentence verdict + who it's for + who it isn't
- H2: What Is Profound AI?
- H2: Pricing (accurate table from Profound's public pricing page)
- H2: **5 Pros** (genuine strengths, each 30-50 words)
- H2: **5 Cons** (genuine limitations, each 30-50 words)
- H2: Who Should Use Profound (2-3 use cases where they're genuinely best)
- H2: Who Shouldn't Use Profound (honest limitations)
- H2: Profound Alternatives
  - Otterly.ai (1 sentence)
  - Peec AI (1 sentence)
  - Scrunch AI (1 sentence)
  - AnswerMonk (1 sentence, fair)
- H2: AnswerMonk vs Profound: When to Choose Which (collapsible section at BOTTOM, not top)
- H2: FAQ

**Schema:** Review + SoftwareApplication + FAQPage + Rating

**Required elements:**
- 5 pros = 5 cons (equal weight, balanced review)
- Real screenshots of Profound UI
- Honest pricing (don't misrepresent)
- Author byline with disclosure
- Update `dateModified` quarterly (pricing refresh)

**Success criteria:**
- Rank top-10 for "profound review" within 60 days
- Don't get deindexed (this is the risk — maintain balance)
- Conversion: 2-5% of readers who click "Start AnswerMonk free trial"

---

### PAGE 11 — Mechanism Cluster (Tier B)

**URL:** `/blog/how-chatgpt-retrieves-sources`

**Title:** How ChatGPT Retrieves Sources: The Complete Mechanism Guide

**Primary keyword:** how chatgpt retrieves sources, chatgpt source selection
**Secondary keywords:** chatgpt browsing mode, gpt-4 retrieval, chatgpt bing integration

**Publish date:** Week 6, Tuesday

**Template:** Mechanism explainer (A + E)

**Word count target:** 2,000-2,500

**Structure:**
- H1: How ChatGPT Retrieves Sources: The Complete Mechanism
- TL;DR: 40-word summary of the 5-step retrieval process
- H2: ChatGPT Retrieval: Training Data vs Browsing Mode
- H2: Step 1: Query Interpretation
- H2: Step 2: Bing Search Integration
- H2: Step 3: Source Ranking Factors
- H2: Step 4: Citation Selection
- H2: Step 5: Answer Synthesis
- H2: What This Means for Your Content
- H2: How to Optimize for ChatGPT Retrieval
- H2: FAQ

**Schema:** TechArticle + HowTo + FAQPage

---

### PAGE 12 — Evergreen Reference Table

**URL:** `/ai-engine-feature-matrix`

**Title:** AI Engine Feature Matrix: ChatGPT vs Claude vs Gemini vs Perplexity (Updated Monthly)

**Primary keyword:** compare ai engines, ai engine comparison
**Secondary keywords:** chatgpt vs claude vs gemini, ai search engines compared

**Publish date:** Week 6, Thursday

**Template:** Reference table (custom)

**Word count target:** 1,500

**Structure:**
- H1: AI Engine Feature Matrix: Updated Monthly
- TL;DR: 40-word summary + last updated date
- H2: **The Complete Feature Matrix**
  - Columns: Engine | Cites Sources | Follows llms.txt | Browsing Mode | API Available | Knowledge Cutoff | Context Window | Custom Instructions | Last Tested
  - Rows: ChatGPT, GPT-4, Claude 3.5, Claude 4, Gemini 1.5, Gemini 2.0, Perplexity, Grok, DeepSeek, Mistral Le Chat, Cohere Coral
- H2: How to Read This Matrix
- H2: Methodology (how we test, refresh cadence)
- H2: What Changed This Month (changelog)
- H2: FAQ

**Schema:** Dataset + Article + FAQPage

**Required elements:**
- The feature matrix (THIS is the page's purpose)
- Monthly refresh commitment + changelog
- Evidence URLs for each cell
- Shareable/embeddable via HTML snippet

**Success criteria:**
- 50-120 RD in 12 months (permanent reference)
- Monthly LinkedIn announcement of updates drives fresh engagement

---

### PAGE 13 — AVI Dashboard (Named Metric #2)

**URL:** `/ai-volatility-index`

**Title:** AI Volatility Index (AVI): Track Weekly AI Search Instability

**Primary keyword:** ai search volatility
**Secondary keywords:** search volatility, chatgpt answer volatility, ai citation stability

**Publish date:** Week 7, Tuesday

**Template:** Dashboard + named metric (E)

**Word count target:** 1,500 + live data

**Structure:**
- H1: AI Volatility Index (AVI): Weekly Tracker
- TL;DR: What AVI is + current week's reading
- **Live chart** (SVG, weekly data points)
- H2: What Is the AVI?
- H2: AVI Formula (explained)
- H2: This Week's Reading (current value + interpretation)
- H2: Historical Trend (last 52 weeks)
- H2: By Industry (benchmark breakdown)
- H2: How to Use the AVI
- H2: Methodology
- H2: Subscribe to Weekly Updates

**Schema:** Dataset + Article + DefinedTerm

**Required elements:**
- Live weekly-updated data (AnswerMonk pulls this from product)
- Original SVG chart (not screenshot, not AI-generated image)
- First-person byline with author schema
- Weekly publication cadence committed

---

### PAGE 14 — Tier 1 Quick Win (Tier B)

**URL:** `/blog/why-track-ai-visibility`

**Title:** Why You Should Track AI Brand Visibility in 2026 (And How to Start)

**Primary keyword:** why should i track ai brand visibility (350, KD 1)
**Secondary keywords:** why monitor chatgpt, ai brand visibility importance

**Publish date:** Week 7, Thursday

**Template:** Informational + conversion

**Word count target:** 1,500-2,000

**Structure:**
- H1: Why You Should Track AI Brand Visibility in 2026
- TL;DR: Summary of 5 reasons
- H2: The Shift: From SEO to AEO
- H2: 5 Reasons to Track AI Visibility
  - Reason 1: AI is already driving research (stats)
  - Reason 2: Your competitors are already being cited
  - Reason 3: Citations decay monthly (50% churn)
  - Reason 4: Traditional SEO tools miss this
  - Reason 5: Category leadership is time-sensitive
- H2: How to Get Started (3 steps)
- H2: Tools for AI Visibility Tracking (AnswerMonk CTA)
- H2: FAQ

---

### PAGE 15 — Final Glossary Expansion

**URL:** `/glossary/ai-visibility`

**Title:** What Is AI Visibility? (Definition, Measurement, and Why It Matters)

**Primary keyword:** ai visibility (1,500, KD 49)
**Secondary keywords:** what is ai visibility, ai search visibility

**Publish date:** Week 8, Tuesday

**Template:** A (Definitional) + comprehensive

**Word count target:** 1,500-2,000

**Structure:**
- H1: What Is AI Visibility? The Complete Guide
- TL;DR: 50-word definition
- H2: Definition (formal)
- H2: AI Visibility vs. Other Visibility Metrics
- H2: How AI Visibility Is Measured (link to AMQ Score)
- H2: Why AI Visibility Matters Now
- H2: How to Improve AI Visibility
- H2: AI Visibility Tools
- H2: FAQ

---

## Publish Schedule Summary

| Week | Day | Page # | URL | Type |
|---|---|---|---|---|
| 1 | Thu | 1 | /glossary/answer-engine-optimization | Pillar |
| 1 | Thu | 2a-d | /glossary/aeo, /geo, /llmo, /aieo | Glossary |
| 1 | Fri | 3 | /blog/aeo-vs-seo-geo | Comparison |
| 2 | Tue | 4 | /blog/chatgpt-data-sources | AIO displacement |
| 2 | Thu | 5 | /blog/llms-txt | Canonical reference |
| 3 | Tue | 2e-h | /glossary/ai-visibility, /ai-citation, /answer-engine, /ai-search | Glossary |
| 3 | Wed | 6 | /amq-score | Named metric + tool |
| 3 | Fri | 7 | /blog/how-to-rank-in-ai-overviews | Procedural |
| 4 | Tue | 8 | /blog/how-to-monitor-ai-search-visibility | Product-led |
| 4 | Thu | 9 | /blog/why-chatgpt-different-answers | Original research |
| 5 | Tue | 10 | /reviews/profound | Competitor review |
| 5 | Thu | — | /reviews/otterly | Competitor review |
| 6 | Tue | 11 | /blog/how-chatgpt-retrieves-sources | Mechanism |
| 6 | Thu | 12 | /ai-engine-feature-matrix | Reference table |
| 7 | Tue | 13 | /ai-volatility-index | Named metric + dashboard |
| 7 | Thu | 14 | /blog/why-track-ai-visibility | Tier 1 quick win |
| 8 | Tue | 15 | /glossary/ai-visibility | Tier 2 glossary |
| 8 | Thu | — | /reviews/peec-ai | Competitor review |

**Total by end of Week 8: 15 canonical pages (plus glossary entries + 3 reviews)**

---

## Content Refresh Schedule

| Page type | Refresh cadence | What to update |
|---|---|---|
| Glossary | Every 6 months | New synonyms, new use cases |
| Comparison | Every 3 months | Pricing, features (verify against competitor sites) |
| Reference tables (Feature Matrix, llms.txt) | **Monthly** | Core data |
| AVI | **Weekly** | Data point |
| Reviews | Every 3 months | Pricing, new features |
| Pillars | Every 6 months | Major updates |
| Mechanism pages | Every 6 months | New model versions |
| Original research | Annually | Re-run with new data |

---

## Quality Standards (all 15 pages)

Every page must pass the QA checklist from `09-blog-rules.md`. Key mandatory elements:

- 40-word TL;DR above fold
- Author byline with LinkedIn `sameAs`
- Article schema + domain-specific schema (DefinedTerm / HowTo / Dataset / Review)
- FAQPage schema with 5+ harvested PAA questions
- 3+ outbound citations to primary sources
- `dateModified` in schema + visible
- 1+ original visual (not AI-generated)
- First-party data for benchmark/research content
- Meta title 50-60 chars
- Meta description 140-160 chars
- Canonical tag
- OG + Twitter Card tags
- BreadcrumbList schema
- SSR-rendered (content visible with JS disabled)

---

## Content NOT in this plan (explicit exclusions)

- General SEO how-tos ("how to rank on Google")
- Listicles without methodology (e.g., "10 best SEO tools")
- Geo-modifier content (local SEO, city+SEO)
- Press releases / announcements (unless paired with evergreen page)
- Thin landing pages (<500 words)
- Case studies (defer to Month 4+ when customers have data)
- Generic marketing content
- Content about our team / culture (not founder brand building)

---

## Post-publish obligations (within 24 hours)

For every page:
1. Submit URL to Google Search Console → Request indexing
2. Submit URL to Bing Webmaster Tools
3. Add to XML sitemap
4. Cross-link from at least 2 existing pages
5. Founder LinkedIn post announcing the page
6. Internal team Slack: "New page live → [URL]"
7. Monitor indexing status in GSC for 7 days

---

## Measurement per page

Track weekly for each page:
- Impressions (Google Search Console)
- Clicks (GSC)
- Average position
- LLM citation rate (AnswerMonk's own product — is this page being cited?)
- Referring domains (Ahrefs)
- Conversion events (email signup, trial start)

After 30 days: diagnose any page with < 100 impressions.
After 60 days: diagnose any page with no LLM citations.
After 90 days: kill any page that fails both.

---

**Next:** See `04-free-tools.md` for tool specs or `08-weekly-execution-90day.md` for day-by-day execution.
