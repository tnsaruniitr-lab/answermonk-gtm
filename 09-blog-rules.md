# 09 — Blog Rules (Writer + Auditor Ruleset)

**Purpose:** The exhaustive quality ruleset every piece of content must pass. Drives both the blog writer (generation constraints) and the blog auditor (validation checks).

**Source:** Sieve-grounded + Ahrefs + advisor judgment
**Total rules:** 80+
**Enforcement:** 22 CRITICAL rules block publish; HIGH rules required; MEDIUM/LOW optional

---

## Rule taxonomy

| Severity | Meaning | Enforcement |
|---|---|---|
| **CRITICAL** | Publishing without fixing kills rankings or gets deindexed | Hard block — do not ship |
| **HIGH** | Significantly reduces ranking + citation probability | Required before publish |
| **MEDIUM** | Noticeable quality/performance hit | Required for pillars; optional for micro-posts |
| **LOW** | Marginal improvement | Optional optimization |

---

## SECTION 1 — Pre-Writing Phase

**R-001 | CRITICAL:** Every post has documented: audience, problem, business outcome, differentiation.
**R-002 | CRITICAL:** Topic sourced from keyword data (vol >100, KD <30) OR sales/support feedback.
**R-003 | HIGH:** Primary keyword identified with volume, KD, intent type, SERP features.
**R-004 | HIGH:** Post assigned to topic cluster with 3+ sibling posts.

---

## SECTION 2 — Content Structure

**R-010 | CRITICAL:** TL;DR block above fold, 40-58 words, `<p data-tldr>`, primary keyword in first 8 words.
**R-011 | CRITICAL:** Every H2's first sentence = complete standalone answer. No "as mentioned earlier" phrasing.
**R-012 | HIGH:** 40% of H2 headings phrased as questions.
**R-013 | HIGH:** ≥1 structural element (table, ordered list, or substantive unordered list) per 500 words.
**R-014 | HIGH:** No section >500 words without H3 subsection break.
**R-015 | MEDIUM:** Average sentence length 15-20 words, max 30 any single sentence.
**R-016 | MEDIUM:** Paragraphs 2-4 sentences max, 80 words max.

---

## SECTION 3 — Heading Hierarchy

**R-020 | CRITICAL:** Exactly 1 H1 containing primary keyword.
**R-021 | HIGH:** No heading skips (H1→H2→H3, never H1→H3).
**R-022 | HIGH:** Minimum 3 H2s for 500+ word posts. Max 10 H2s for 2,000-word post.
**R-023 | MEDIUM:** H1: 50-70 chars. H2: 30-70 chars. H3: 20-60 chars.
**R-024 | HIGH:** H1 matches `<title>` tag within 90% similarity. Meta title 50-60 chars.

---

## SECTION 4 — Schema Markup

**R-030 | CRITICAL:** Article schema with headline, author (Person + sameAs LinkedIn), publisher, datePublished, dateModified, description, image.
**R-031 | HIGH:** FAQPage schema required if >3 FAQ questions.
**R-032 | HIGH:** DefinedTerm + DefinedTermSet for glossary entries.
**R-033 | HIGH:** HowTo schema with HowToStep for procedural posts.
**R-034 | MEDIUM:** Table schema or ItemList for comparison posts.
**R-035 | MEDIUM:** Dataset schema for metric/benchmark posts.
**R-036 | HIGH:** BreadcrumbList schema (Home > Blog > Category > Post).

---

## SECTION 5 — Word Count Standards

**R-040 | HIGH:** Word count matches post type:

| Type | Min | Target | Max |
|---|---|---|---|
| Glossary | 500 | 700 | 1,000 |
| How-to | 800 | 1,200 | 1,500 |
| Comparison | 1,200 | 1,800 | 2,500 |
| Pillar | 1,900 | 2,500 | 4,000 |
| Research | 1,500 | 2,500 | 5,000 |
| FAQ | 600 | 900 | 1,200 |
| Listicle | 1,500 | 2,500 | 3,500 |
| Mechanism | 1,200 | 1,800 | 2,500 |

---

## SECTION 6 — Readability

**R-050 | HIGH:** Flesch Reading Ease 60-70; Flesch-Kincaid Grade 8-10.
**R-051 | MEDIUM:** Passive voice <10% of sentences.
**R-052 | MEDIUM:** All acronyms expanded on first use with `<abbr>` or inline.
**R-053 | LOW:** Active voice + imperative mood for how-tos; present tense for definitions.

---

## SECTION 7 — Author / E-E-A-T

**R-060 | CRITICAL:** Named author byline visible, bio 50-100 words, author page link, Person schema with sameAs (LinkedIn URL that resolves).
**R-061 | HIGH:** LinkedIn profile real + resolves; role aligned with content topic.
**R-062 | HIGH:** All claims have source + date + method cited inline or footnote.
**R-063 | MEDIUM:** Reviewer byline for pillar posts (>1,900 words).

---

## SECTION 8 — Internal Linking

**R-070 | HIGH:** First mention of any concept with dedicated page is linked (Wikipedia-style).
**R-071 | HIGH:** 3-12 internal links per 1,500 words.
**R-072 | MEDIUM:** Descriptive anchor text (no "click here").
**R-073 | MEDIUM:** 2+ sibling cluster links. 3+ inbound sibling links after cluster matures.
**R-074 | HIGH:** "Related" section with 3-5 contextually relevant links.

---

## SECTION 9 — External Linking

**R-080 | CRITICAL:** Minimum 3 outbound links to primary sources per post. Priority:
1. Official docs (OpenAI, Google, MDN)
2. Academic papers (arXiv, ACM, IEEE)
3. Industry reports (Gartner, Forrester)
4. First-party data from authoritative companies
5. Wikipedia (entity disambiguation only)

Do NOT link to: competitor marketing content as sources, generic "what is X" blogs, paywalled content without summary, SEO-stuffed listicles.

**R-081 | HIGH:** External links open in new tab (`target="_blank" rel="noopener"`).
**R-082 | MEDIUM:** Nofollow untrusted sources; DoFollow primary sources (citation reciprocity).
**R-083 | HIGH:** Anchor text accurately represents linked content (no keyword stuffing).

---

## SECTION 10 — Featured Snippet Optimization

**R-090 | HIGH:** Paragraph snippets: 40-58 words, directly after H2 with query term, query phrase in first 8 words, ends complete sentence.
**R-091 | HIGH:** List snippets: 3-10 items, each 6-24 words, ordered for steps, unordered for features.
**R-092 | HIGH:** Table snippets: 2-4 cols, 3-7 rows, `<th scope="col">` markup (not CSS divs).
**R-093 | MEDIUM:** Odd-numbered step lists (7 or 9) prefered for citation.

---

## SECTION 11 — AEO / LLM Citation

**R-100 | CRITICAL:** Server-side rendered. Primary answer content visible with JS disabled.
**R-101 | CRITICAL:** Written for extraction, not keyword ranking. Every section standalone-quotable, factually specific, verifiable. Zero vague marketing language ("revolutionary," "game-changing," "cutting-edge").
**R-102 | HIGH:** Entity naming consistent site-wide ("AnswerMonk" always, "Answer Engine Optimization (AEO)" on first use).
**R-103 | HIGH:** First-party data required for ranking/benchmark/comparison posts ("We tested X," "Our data shows Y").
**R-104 | HIGH:** FAQ questions harvested from live SERP PAA. Minimum 5 questions with 1-sentence direct answer + 2-sentence elaboration.
**R-105 | HIGH:** Long-form content (>1,500 words) includes `<nav aria-label="Table of contents">`.

---

## SECTION 12 — Freshness

**R-110 | CRITICAL:** datePublished + dateModified in schema + visible "Last updated" on page.
**R-111 | HIGH:** Refresh cadence:

| Type | Cadence | What to update |
|---|---|---|
| Glossary | 6 months | Synonyms, use cases |
| Comparison | 3 months | Pricing, features |
| Reference tables | Monthly | Core data |
| Listicles | Annually | Re-rank entries |
| Mechanism | 6 months | New model versions |
| Research | Annually | Re-run with new data |
| Pillars | 6 months | Major updates |

**R-112 | MEDIUM:** Refresh updates both dateModified + visible "Last updated" + publication year in title.
**R-113 | HIGH:** Perplexity targets: dateModified <180 days. ChatGPT: <365 days.

---

## SECTION 13 — Images and Visuals

**R-120 | CRITICAL:** No AI-generated imagery as hero. Prefer: original product screenshots, custom diagrams, original charts, real people photos.
**R-121 | HIGH:** Every image has descriptive alt text (5-15 words), descriptive filename, lazy-loading (except hero), optimized file size (<200KB most, <500KB hero).
**R-122 | HIGH:** ≥1 visual per 500 words.
**R-123 | MEDIUM:** Original diagrams include subtle AnswerMonk branding for attribution backlinks.
**R-124 | MEDIUM:** ImageObject schema for hero image.

---

## SECTION 14 — CTAs

**R-130 | HIGH:** Hero soft CTA + mid-article contextual + footer hard CTA.
**R-131 | HIGH:** CTAs relevant to post topic (not generic "Book a demo").
**R-132 | MEDIUM:** Max 4 CTAs per post.
**R-133 | MEDIUM:** Mid-article content upgrade for pillar posts (>1,900 words).

---

## SECTION 15 — Meta Tags

**R-140 | CRITICAL:** Meta title 50-60 chars, primary keyword included, unique across site. Format: "Primary Keyword | Secondary Context | Brand"
**R-141 | CRITICAL:** Meta description 140-160 chars, primary keyword, CTA/value prop, unique.
**R-142 | HIGH:** Open Graph tags: og:title, og:description, og:image (1200x630), og:url, og:type=article.
**R-143 | HIGH:** Twitter Card: twitter:card=summary_large_image, twitter:title, twitter:description, twitter:image.
**R-144 | CRITICAL:** Canonical tag self-referential, absolute URL.

---

## SECTION 16 — Technical SEO

**R-150 | CRITICAL:** Core Web Vitals pass: LCP <2.5s, INP <200ms, CLS <0.1.
**R-151 | CRITICAL:** robots.txt allows: GPTBot, ClaudeBot, PerplexityBot, Google-Extended, CCBot.
**R-152 | HIGH:** Internal links HTTPS, absolute URLs.
**R-153 | HIGH:** URL in sitemap, submitted to Google Search Console.
**R-154 | HIGH:** URL: lowercase, hyphens (not underscores), max 5 segments deep, keyword in slug, no dates (unless time-bound).
**R-155 | HIGH:** Mobile-responsive, readable without zoom, tap targets >44px.

---

## SECTION 17 — Originality / AI-Flag Prevention

**R-160 | CRITICAL:** ≥4 human signals present:
1. First-person byline with LinkedIn sameAs schema
2. ≥1 first-party data point ("We tested," "Our product data shows")
3. ≥1 original screenshot or custom diagram (NOT AI-generated)
4. ≥3 outbound citations to primary sources

**R-161 | CRITICAL:** Zero AI-generated imagery anywhere.
**R-162 | HIGH:** ≥2 opinions/points of view ("We believe," "Our view," "This is why we cut X").
**R-163 | HIGH:** No banned AI-stylistic phrases:
- "In today's fast-paced world"
- "It's important to note"
- "In this comprehensive guide"
- "Whether you're a [A] or a [B]"
- "The key to success is"
- "In summary"
- "Let's dive in"
- "By the end of this article"

---

## SECTION 18 — Anti-Patterns (Hard Kills)

**R-170 | CRITICAL:** No hit-piece competitor reviews. Balanced 5-pros + 5-cons required.
**R-171 | CRITICAL:** No announcement without evergreen twin page (/awards, /news, /updates).
**R-172 | CRITICAL:** Never target "aeo" raw keyword (American Eagle Outfitters contamination).
**R-173 | HIGH:** No listicles without testing methodology, no geo-modifier SEO keywords, no commercial "alternative" pages as primary content, no shopping-engine long-tails, no generic B2B marketing-engineering content.
**R-174 | HIGH:** Keyword density 0.5%-2.5%. Above = stuffing; below = weak relevance.
**R-175 | MEDIUM:** No exact-duplicate content. Similar topics differentiated by angle.

---

## SECTION 19 — Pre-Publish QA Checklist

Copy into CMS for every post. All CRITICAL must pass.

```
CRITICAL (22 rules — all must pass):
□ R-001 Brief complete (audience, problem, outcome, differentiation)
□ R-002 Topic sourced (keyword data or sales feedback)
□ R-010 TL;DR 40-58 words, data-tldr, keyword in first 8 words
□ R-011 Every H2 first sentence = standalone answer
□ R-020 Exactly 1 H1 with primary keyword
□ R-030 Article schema validated (author + sameAs + dates)
□ R-060 Named author with LinkedIn sameAs + bio
□ R-080 ≥3 outbound primary source citations
□ R-100 SSR verified (content visible with JS disabled)
□ R-101 Zero vague marketing language
□ R-110 datePublished + dateModified + visible "Last updated"
□ R-120 No AI-generated hero imagery
□ R-140 Meta title 50-60 chars with keyword
□ R-141 Meta description 140-160 chars
□ R-144 Self-referential canonical tag
□ R-150 Core Web Vitals pass
□ R-151 All AI crawlers allowed in robots.txt
□ R-160 ≥4 human signals present
□ R-161 Zero AI-generated imagery site-wide
□ R-170 No hit-piece competitor framing
□ R-171 Announcement content has evergreen twin
□ R-172 Not targeting raw "aeo" keyword

HIGH (45 rules — pre-publish required):
[Full checklist — see sections 1-17 above]

POST-PUBLISH (within 24h):
□ Submit to Google Search Console + request indexing
□ Submit to Bing Webmaster Tools
□ Founder LinkedIn post
□ Cross-link from ≥2 existing pages
□ Monitor indexing for 7 days
```

---

## SECTION 20 — Post-Publish Obligations

**R-180 | HIGH:** Within 24 hours: GSC submit + indexing, Bing Webmaster, founder LinkedIn share, cross-links from 2+ existing pages.
**R-181 | HIGH:** Within 7 days: Indexing status check, impressions/clicks tracked, manual LLM citation test, initial position benchmark.
**R-182 | MEDIUM:** Within 30 days: Ranking check, outbound links audit, diagnose if <100 impressions.

---

## SECTION 21 — Refresh Workflow

When refresh due (per R-111):
1. Re-research target keyword (volume/KD/SERP changes?)
2. Re-run featured snippet audit
3. Update data points with fresh numbers
4. Replace outdated references
5. Re-verify outbound sources (no broken links)
6. Update dateModified schema + visible date
7. Update year in title if present
8. Add "Updated [Month Year]" edit note at top
9. Re-submit to Google Search Console
10. Re-share on LinkedIn with "We refreshed this" framing

---

## SECTION 22 — Top 10 Rules (if you only enforce these, catches 80% of quality failures)

1. **R-010** — 40-word TL;DR with keyword in first 8 words
2. **R-011** — Every H2 first sentence = standalone answer
3. **R-030** — Validated Article schema with author + dates
4. **R-060** — Named author with LinkedIn sameAs
5. **R-080** — ≥3 outbound primary-source citations
6. **R-100** — SSR validated (JS-off test)
7. **R-110** — datePublished + dateModified + visible "Last updated"
8. **R-160** — 4+ human signals (byline, first-party data, original visual, citations)
9. **R-151** — AI crawlers allowed in robots.txt
10. **R-170-173** — Anti-pattern kills (hit-pieces, raw AEO keyword, press without twin)

---

## Integration with writer + auditor

### Writer generation constraints (critical rules in system prompt)
```
YOU MUST:
- Start with <p data-tldr> containing 40-58 words, keyword in first 8 words
- Every H2's first sentence = complete standalone answer
- 40% of H2s as questions
- ≥1 table or ordered list per 500 words
- ≥3 outbound primary source citations
- End with FAQ block of 5+ questions
- Include ≥2 points of view ("We believe", "Our view")

YOU MUST NOT:
- Write hit-piece reviews (balanced only)
- Use AI-generated imagery
- Use vague marketing language
- Skip heading levels
- Use banned AI-stylistic phrases
```

### Auditor validation (automatable rules become checks)
```
Fully automatable (40+ rules):
- Word counts, heading hierarchy, schema validation, link counts, character counts, canonical presence, banned phrases, URL patterns

Semi-automatable (25 rules):
- Readability scoring, passive voice, entity naming consistency, first-party data presence

Human-only (15 rules):
- POV/opinion presence, outbound source quality tier, intent match, original visual quality
```

---

## The governance rule

**One source of truth:** This file (`09-blog-rules.md`) is canonical. If the writer or auditor drifts from these rules, update this file first, then propagate.

**Review cadence:** Monthly. Add new rules as failures emerge in production. Remove rules that consistently pass (not worth auditing).

**Version control:** Every change commit'd with changelog. Major rule changes require written rationale.

---

## Summary

**80+ rules across 21 sections.** 22 are CRITICAL and block publishing. The rest are HIGH priority for pre-publish approval.

**Key enforcement mechanism:**
- Writer uses rules as generation constraints (baked into system prompt)
- Auditor uses rules as validation checks (automated + LLM judge + human review)
- Both consume this file as source of truth

**Top 10 rules catch 80% of failures.** If you can't enforce all 80, enforce these.

**When in doubt:** "Would a competent editor be proud to publish this under their real name?" If no, don't ship.
