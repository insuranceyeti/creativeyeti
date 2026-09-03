---
brand: health-for-moms
doc: voc-corpus-profile
generated_on: 2026-09-03
refresh_by: 2026-10-03
raw_records_received: 1322
normalized_records: 1322
deduplicated_records_removed: 0
date_range: 2025-01-08 to 2026-09-03
sources_read:
  - Facebook and Instagram ad comments, Meta ad account HealthForMoms, act 484897827497337, via Parker MCP search_facebook_ad_comments_sql. Corpus end confirmed by offset probe on 2026-09-03, and the tool's own total field reads 1322.
  - Parker MCP search_facebook_ad_comments_semantic, two passes on 2026-09-03, both reporting totalCommentsAnalyzed 1322, which agrees with the SQL denominator.
  - Parker MCP search_customer_reviews_sql, unfiltered, 2026-09-03. Returned totalReviews 0.
  - Parker MCP semantic_search_post_purchase_survey, 2026-09-03. Returned totalResponsesForBrand 0, collection exists.
  - source-pulls/ad-comments.md, the completed full-corpus persona read of the same 1,322 rows, generated 2026-09-03. Used for the model-applied theme counts and the ad-level spread this profile could not recompute through the tool.
  - running-notes/missing-context.md and running-notes/brand-rules.md, for the dark-surface rules and the standing brand constraints.
  - parker-system/creative-strategy-context/customer-review-mining-method.md, the canonical mining method this profile applies.
expected_sources_missing:
  - first-party review exports from the brand site (zero rows, verified live 2026-09-03)
  - connected review platforms (none connected)
  - marketplace and retail reviews (none ingested)
  - post-purchase survey responses (zero rows, verified live 2026-09-03)
  - NPS responses (no NPS instrument)
  - competitor and category reviews (no rival brands tracked in the Parker app; branch deferred by the user 2026-09-03)
  - Reddit, forum, and community pulls (not yet run for this brand)
  - support tickets, FAQs, and customer-service exports (not connected)
  - organic social comments (not pulled; the TikTok library holds 23 scored videos, not comment rows)
  - prior voc-corpus-profile.md and prior voice-of-customer.md (first run, no history)
  - website-and-product-audit.md, for SKU normalization (Phase 1A, not yet written)
  - personas-profile.md, for identity and behavioral-signal slugs (Phase 1C, not yet written)
structured_fields_available:
  - comment_id
  - message
  - created_time
  - like_count
  - comment_count
  - comment_length
  - ad_ids
  - ad_names
  - post_ids
  - parent_comment_ids
  - facebook_comment_ids
  - brand_id
  - snapshot_date
  - etl_run_id
  - embedded_at
model_applied_tags:
  - sentiment
  - purchase motivation
  - buying on behalf of someone else
  - usage occasion and life stage
  - barrier or objection
  - product experience
  - outcome
  - transformation
  - emotion
  - social proof
  - loyalty
  - ad or influencer mention
  - recommendation mention
  - comparison mention
  - product confusion
  - price concern
  - service issue
  - improvement suggestion
  - notable quote candidate
  - persona signal
  - brand-self-echo candidate
data_limitations:
  - The corpus is one source. Facebook ad comments are the only first-party customer-language surface this brand has. Reviews and surveys are both empty, verified live.
  - Ad comments are a public, performative, objection-skewed surface. People write there to argue, correct, warn, and be seen agreeing. Buyers who are happy have no reason to post.
  - Zero identity fields. author_name and author_id are null on all 1,322 rows, so unique commenters cannot be counted and nothing can be deduplicated by person.
  - Zero rating or score field. No star rating, no NPS, no sentiment score. Every sentiment read in this doc is a model-applied tag, never a structured fact.
  - Zero product or SKU field. Nothing ties a comment to a plan, a carrier, or a product line.
  - No permalink on any row, so no quote can be linked back to its public thread.
  - No join between a comment and a lead. Nothing here can be tied to the 4,336 leads the account produced in the last 90 days.
  - Heavy time skew. 846 of 1,322 comments (64.0%) were posted in March and April 2026 alone.
  - No competitor or category baseline, so no objection rate here can be called high or low for the category.
  - No persona slugs exist yet, so no row in this corpus carries an identity tag. Downstream extraction passes must leave identity_tag null until personas-profile.md is written.
---

# VoC corpus profile - Health For Moms

## Executive summary

Here is the honest headline before any finding: this brand has no customer reviews and no post-purchase surveys. Not a thin corpus. Zero rows in both, checked live against the Parker tools today, not assumed from a note. The only first-party record of how this brand's customers talk is 1,322 Facebook ad comments. Everything below is built on that one surface, and the shape of that surface bends every number in this doc.

**One. The corpus is 1,322 records from a single source, and that source is the loudest, least representative one available.** `verified` — two independent Parker tools agree on the denominator. The SQL tool's total field reads 1,322 and an offset probe at 1,300 returned exactly 22 rows, which pins the end of the corpus. The semantic tool reported `totalCommentsAnalyzed: 1322` on both passes run today. The mining method ranks evidence with survey and review data at the top and public comments near the bottom. This brand holds only the bottom rank, so the confidence ceiling on every theme in this doc is mixed, never verified, no matter how often a phrase recurs.

**Two. There is no sentiment split to report, because no rating or score field exists anywhere in the corpus.** `verified` — I inspected the full field list returned by the tool, including every optional field it offers, and there is no star, score, NPS, or sentiment column. What I can give instead are structured proxies counted against all 1,322 rows: 166 comments (12.6%) contain a question mark, 45 (3.4%) contain the word "scam," 20 (1.5%) contain "thank," and 6 (0.5%) contain "accurate." Any percentage a downstream doc quotes as a sentiment split for this brand is invented. There is nothing to compute it from.

**Three. The single biggest theme is the audience correcting the ad, not praising or wanting the product.** `verified` on the count, `inferred` on the read. 207 of 1,322 comments (15.7%) contain the word "deductible" and 74 (5.6%) contain "out of pocket." The full read in `source-pulls/ad-comments.md` classified 103 of those 1,322 (7.8%), spread across 13 different ads, as people telling the brand it used the word wrong. One of them, on 2026-05-01 under `MOMS38 - 1 - V1`, reads in full: "Deductible is different than maximum out of pocket 😃 -an insurance agent". That is the largest single conversation under this brand's best-performing creative, and it is an argument.

**Four. The corpus is really a deep read of two months, not two years.** `verified` — I computed this myself with date-bounded offset probes rather than trusting a summary. March 2026 holds exactly 340 comments and April 2026 holds exactly 506. Together that is 846 of 1,322, or 64.0%, inside a 61-day window. All of 2025 holds 227 comments, or 17.2%, across a full twelve months. So any rate in this doc is a rate inside a spring 2026 campaign moment, not a rate across the brand's advertising history.

**Five. Almost nobody here says the product worked, because almost nobody here is a customer.** `verified` on the counts. Across 1,322 comments there are exactly two reports of a good experience with this brand's service, both from people who were told no and thanked the agent anyway, and roughly 12 clear moments of someone saying the ad described their life. That is under 1% of the corpus. There is not a single outcome story, transformation, or repeat-purchase statement in 1,322 records. That absence is a finding about the surface, not about the product.

**The most important creative lever this corpus points at.** The only creative in the corpus that earns agreement instead of argument is the `MOMS38 - 2` skit family, where one woman plays both the frustrated mom and the insurance rep denying a claim because it happened "in a different hallway." Nearly every recognition sits there. The lever is the shift from a number people can dispute to an experience people have lived. `inferred`, from where the recognition comments cluster, and it should be read as a hypothesis for the account read to test rather than a proven lever.

**The largest data limitation.** No buyer voice exists. None. Not thin, not sparse, absent. Every identity, objection, and phrase in this corpus comes from someone the algorithm served, and there is no way to check any of it against a person who actually bought. Until a review pipeline, a post-purchase survey, or a lead-level join exists, no Voice of Customer work for this brand can rise above mixed confidence.

## Source and data profile

### Record counts

| Measure | Count | How it was established |
|---|---|---|
| Raw records received | 1,322 | Parker MCP `search_facebook_ad_comments_sql`, the tool's own `total` field, 2026-09-03 |
| Normalized records | 1,322 | Every raw row carries the fields the normalized model needs |
| Duplicates removed or merged | 0 | See the note below on why the count is zero |
| Records with usable text | 1,316 of 1,322 (99.5%) | 6 rows have an empty `message` and a `comment_length` of 0 |
| Sources represented | 1 | Facebook and Instagram ad comments, one Meta ad account |

**Why the dedupe count is zero.** The source already dedupes at ingest, and it does it in a way worth naming because a later pass could easily double-count if it did not know. The same comment can sit under several ad IDs when an ad has been copied. The row for comment `3fb95c2d-c637-a6a4-d741-fc04c9552ecd` on 2026-09-03 carries two ad IDs, `moms-63 2b` and `moms-63 2b - Copy`, two post IDs, and two entries in `facebook_comment_ids`. It is one record with the duplicate references preserved in arrays, exactly the shape this profile would have had to build by hand. So no rows were removed. `verified` — I read the arrays on sampled rows directly.

**One caution on that.** Because `author_name` and `author_id` are null on every row, there is no way to detect the other kind of duplicate: one person posting the same thing under several ads, or one operator working the comment section with a repeated script. The full read found at least nine near-identical posts of the same Direct Primary Care pitch under `MOMS38 - 1 - V1` on a single day, all counted as separate records. They are separate records. They are not separate people. `verified` on the repetition, `data-limited` on how many other cases exist.

### Date range and time distribution

Earliest record 2025-01-08. Latest record 2026-09-03, which is today. `verified` by sorting ascending at offset 0 and reading the newest page.

I did not take the time shape on faith. The tool does not return a count when a date filter is applied, so I pinned each window by probing offsets until the rows ran out.

| Window | Comments | Share of 1,322 | How pinned |
|---|---|---|---|
| 2025-01-08 to 2025-12-31 | 227 | 17.2% | offset 226 returned a row, offset 227 returned none |
| 2026-01-01 to 2026-02-28, plus 2026-05-01 to 2026-09-03 | 249 | 18.8% | derived: 1,322 minus 227 minus 340 minus 506 |
| 2026-03-01 to 2026-03-31 | 340 | 25.7% | offset 339 returned a row, offset 340 returned none |
| 2026-04-01 to 2026-04-30 | 506 | 38.3% | offset 503 returned 3 rows, offset 506 returned none |

Read that table twice. Two months out of twenty carry 846 of 1,322 comments, or 64.0%. A full calendar year of 2025 carries 227, or 17.2%. This is not an even record of how customers talk about this brand over time. It is a very deep read of one campaign moment with a thin tail on either side.

### Field coverage

Every field the tool exposes, and how much of the corpus actually has it. This is the table a downstream pass should check before it promises a breakdown it cannot deliver.

| Field | Populated share | Type | Note |
|---|---|---|---|
| `comment_id` | 1,322 of 1,322 (100%) | structured | Stable row id, a UUID |
| `message` | 1,316 of 1,322 (99.5%) | structured | 6 rows blank |
| `created_time` | 1,322 of 1,322 (100%) | structured | ISO timestamp with timezone, no malformed dates seen |
| `like_count` | 1,322 of 1,322 (100%) | structured | Range 0 to 47 |
| `comment_count` | 1,322 of 1,322 (100%) | structured | Replies to that comment; range 0 to 22 |
| `comment_length` | 1,322 of 1,322 (100%) | structured | Range 0 to well over 1,000 characters |
| `ad_ids` / `ad_names` | 1,322 of 1,322 (100%) | structured | Arrays; a comment can sit under an ad and its copy |
| `post_ids` | 1,322 of 1,322 (100%) | structured | Arrays, matched to the ad IDs |
| `parent_comment_ids` | 1,322 of 1,322 (100%) | structured | Empty array on a top-level comment |
| `facebook_comment_ids` | 1,322 of 1,322 (100%) | structured | Carries the duplicate source references |
| `brand_id`, `snapshot_date`, `etl_run_id`, `embedded_at` | 1,322 of 1,322 (100%) | structured | Pipeline metadata, not customer signal |
| `author_name` | 0 of 1,322 (0%) | absent | Null on every row |
| `author_id` | 0 of 1,322 (0%) | absent | Null on every row |
| `permalink_url` | 0 of 1,322 (0%) | absent | Null on every row |
| rating or score | 0 of 1,322 (0%) | absent | No such column exists |
| product or SKU | 0 of 1,322 (0%) | absent | No such column exists |
| age, gender, region, buyer type | 0 of 1,322 (0%) | absent | No such columns exist |

The 1,023 top-level and 299 reply split comes from the full read in `source-pulls/ad-comments.md`, which paginated the whole corpus. I confirmed the reply filter works, by running the same semantic query with nested comments on and off and watching a reply drop out, but I did not independently recount the split. `stated`, carried from the upstream doc.

### Rating and score distribution

There is none. This section exists so no later pass writes one.

There is no rating field, no star field, and no score field on any of the 1,322 records. The nearest structured measures of how a comment landed are `like_count` and `comment_count`, and neither is a rating. A like on "The affordable care act made insurance unaffordable for most with the premiums and the high deductibles," which drew 36 likes on 2026-03-30, is agreement with a political point, not satisfaction with a product.

What the like data does show, computed by sorting on `like_count` and probing where the zeros start:

| Measure | Value |
|---|---|
| Highest like count on any record | 47 |
| The ten most-liked records | 47, 36, 33, 24, 21, 19, 19, 17, 15, 15 |
| Records carrying at least one like | at least 331 and at most 390 of 1,322, roughly 25% to 30% |
| Records carrying no likes at all | at least 932 and at most 991 of 1,322, roughly 70% to 75% |

`verified` on the bounds. Offset 330 sorted by likes descending still returned a record with one like; offset 392 returned records with zero. So about three quarters of this corpus is a comment nobody agreed with out loud. That matters for weighting: raw count and agreement are different things here, and the mining method is right that a count alone is not significance.

### Data-quality issues found

- **Six blank text rows.** `verified`. Sorting by `comment_length` ascending and reading the first 120 records, which covered every record of four characters or fewer, turned up exactly six with a length of 0. One of them, `515e1b4f-f652-619c-42aa-ec73046299eb` on 2026-06-18, carries 7 likes on empty text, which suggests the original was an image or a sticker the pipeline did not capture.
- **A large block of near-identical one-word records.** 80 of 1,322 records (6.1%) contain the string "help." The full read found 49 of those are the single word "Help" or "help," all on one ad, `Moms43 - 4 - V3`, between May and September 2026. Whether that is inbound demand or an artifact is unreadable from the data. `data-limited` on meaning.
- **The tool's `total` field is unreliable without a filter.** An unfiltered call at offset 0 returned `total: 0` while returning rows. The same call at offset 1300 returned `total: 1322`. A text search returns a correct total; a date filter returns 0. Any later pass counting through this tool must probe offsets rather than trusting the field. `verified` by running both.
- **Sort order is applied across pages, not within one.** Records inside a returned page are not ordered by the requested sort key, though the page boundary honors it. Do not read the first row of a page as the extreme value.
- **No encoding problems.** Emoji, curly quotes, and line breaks all came through clean. No mojibake seen in any sampled record.
- **No malformed dates.** Every `created_time` parsed as a valid timestamp.

## Normalized schema

One source maps into the normalized model, so the mapping is short and there is nothing to reconcile across platforms. That simplicity is not a strength. It is the whole problem.

| Normalized field | Source field | Kind | Coverage |
|---|---|---|---|
| `row_id` | `comment_id` | structured fact | 100% |
| `source_type` | constant: `ad-comment` | structured fact | 100% |
| `platform` | constant: Facebook and Instagram, Meta ad account act 484897827497337 | structured fact | 100% |
| `source_native_id` | `facebook_comment_ids[]` | structured fact | 100% |
| `date` | `created_time` | structured fact | 100% |
| `rating_or_score` | none | unavailable | 0% |
| `product_or_sku` | none | unavailable | 0% |
| `text` | `message` | structured fact | 99.5%, 6 blank |
| `url` | `permalink_url` | unavailable | 0%, null on every row |
| `campaign_reference` | `ad_ids[]`, `ad_names[]`, `post_ids[]` | structured fact | 100% |
| `thread_position` | `parent_comment_ids[]` empty or populated | structured fact | 100% |
| `engagement` | `like_count`, `comment_count` | structured fact | 100% |
| `text_length` | `comment_length` | structured fact | 100% |
| `demographics`, `region`, `channel`, `device`, `occasion`, `buyer_type`, `segment` | none | unavailable | 0% |

**Nothing in this corpus is inferred into a structured field.** Where a commenter states her own situation in the text, for instance "I'm self employed" or "Mine is $6k per person too but since it's thru my job I don't really have a choice," that is customer language captured verbatim, and any read on top of it is a model-applied tag on the row, never a filled-in structured field. The prompt's rule holds: do not infer a missing structured field from text, and mark the tag as the model's when you read one.

**A note on the demographics that exist elsewhere.** The account's Meta delivery data shows 95.2% female and 81.2% aged 25 to 44. That describes who was served the ads. It is a different population from who commented, and joining the two would be a mistake. Delivery demographics are not a field on this corpus and must not be presented as one.

## Classification method

Every row carries the structured fields above. Everything below is the model reading the text, and downstream passes should treat it accordingly.

**Structured facts, safe to compute on.** Row id, date, platform, ad and post reference, thread position, like and reply counts, text length, and the presence or absence of a literal string in the text. When this doc says 207 of 1,322 records contain the word "deductible," that is a structured count from a case-insensitive string match, and it is checkable.

**Model-applied tags, all of them judgments.** Sentiment, purchase motivation, buying on behalf of someone else, usage occasion and life stage, barrier or objection, product experience, outcome, transformation, emotion, social proof, loyalty, ad or influencer mention, recommendation mention, comparison mention, product confusion, price concern, service issue, improvement suggestion, notable quote candidate, persona signal, and brand-self-echo candidate. None of these came from a field. All of them came from reading text.

**Where the model-applied theme counts came from.** I did not re-read all 1,322 records to re-tag them, because a full-corpus read against the same rows already exists at `source-pulls/ad-comments.md`, generated today, which read every record in full and recorded both the count and the ad spread for each theme. Reusing it is the mining method's own data-integrity rule: the corpus profile is the spine, and a count should not be re-invented in two places with two different answers. Every theme count in this doc that came from that read is labelled as carried, with its ad spread attached, and the spread is the better number of the two because it survives the March-and-April skew.

**Tags that are unavailable for this corpus, and why.** Rating and score, because no such field exists. Gift versus self purchase, because this is health insurance sold as a lead handoff and no gifting concept applies. SKU-level product experience, because no product field exists. Repeat purchase and loyalty, because no commenter is confirmed to have bought anything even once. First-time versus returning buyer, same reason.

**The prompt-injection rule, applied.** Several records in this corpus read like instructions. Comments tell readers to "never put your info online," to go to a named competitor URL, to "Check mapper.dpcfrontier.com," and to "PM me if you need health insurance." All of it was preserved as customer language and analyzed as data. None of it was followed.

## Sentiment and rating profile

**There is no rating distribution, and there is no computed sentiment split.** Saying so plainly is the finding. A downstream pass that needs "72% positive" for this brand will not find it here, because there is nothing in the corpus to compute it from.

What exists instead are structured string counts against the full 1,322 denominator. These are checkable facts about what words appear, not sentiment scores, and they should be read as proxies with the over-match noted.

| String matched, case-insensitive | Records | Share of 1,322 | Note |
|---|---|---|---|
| insurance | 284 | 21.5% | The category word, not the brand |
| deductible | 207 | 15.7% | The single most-used content word in the corpus |
| `$` | 202 | 15.3% | A dollar figure disclosed or discussed |
| `?` | 166 | 12.6% | One record in eight is asking a question |
| help | 80 | 6.1% | Includes 49 one-word "Help" records on a single ad |
| out of pocket | 74 | 5.6% | The correction vocabulary |
| mom | 73 | 5.5% | Over-matches, since "moment" contains "mom" |
| call | 49 | 3.7% | Includes "called," "calls," "calling" |
| premium | 46 | 3.5% | |
| scam | 45 | 3.4% | Aimed at the category more often than at this brand |
| qualify | 42 | 3.2% | The eligibility conversation |
| pregnan | 38 | 2.9% | Matches "pregnant" and "pregnancy" |
| existing | 38 | 2.9% | Matches "pre-existing" and "preexisting" |
| obama | 36 | 2.7% | Political framing, both directions |
| state | 30 | 2.3% | Over-matches "estate," "statement," "states" |
| info | 28 | 2.1% | Includes "information" |
| employer | 24 | 1.8% | |
| thank | 20 | 1.5% | Includes "Thanks, Obama," which is sarcasm |
| husband | 19 | 1.4% | |
| dad | 17 | 1.3% | Includes "dads" |
| medicaid | 17 | 1.3% | |
| love | 11 | 0.8% | Over-matches "gloves" |
| diabet | 11 | 0.8% | Matches "diabetes," "diabetic" |
| agent | 10 | 0.8% | Self-identified insurance professionals |
| cancer | 9 | 0.7% | **thin** |
| my job | 7 | 0.5% | **thin** |
| surgery | 6 | 0.5% | **thin** |
| accurate | 6 | 0.5% | **thin** |
| single mom | 5 | 0.4% | **thin** |
| college | 3 | 0.2% | **thin** |
| enrollment | 2 | 0.2% | **thin** |
| open enrollment | 1 | 0.1% | **thin** |

Two of those lines deserve a second look because they cut against what the brand believes about itself.

**"Mom" barely appears.** The brand's entire creative device is one word, and that word shows up in at most 73 of 1,322 records (5.5%), a figure that is inflated because the string also matches "moment." "Insurance" appears in 284 (21.5%), nearly four times as often. `verified` on both counts. The audience is talking about the category. It is not talking about the identity the brand named itself after. `inferred` on what that means, and it is a real question rather than a settled read.

**"Open enrollment" is almost absent.** The brand's own stated objection list, quoted in `source-pulls/ad-comments.md` from the brand context document, names "I should just wait for open enrollment" as one of its five main objections. That exact phrase appears in 1 of 1,322 records (0.1%), and "enrollment" in any form appears in 2 (0.2%). `verified`. Either the timing objection lives somewhere other than the comments, or it is smaller than the brand thinks. Flagged **thin** and carried into the open loops rather than resolved here.

### Sentiment as a model-applied read

The full read at `source-pulls/ad-comments.md` classified every record and found the corpus reads overwhelmingly negative or neutral, with the negativity aimed at the health insurance category more often than at this brand. Carried as `stated`, with the counts that support it:

| Read | Records | Share of 1,322 | Support |
|---|---|---|---|
| Clear recognition, someone saying the ad described their life | roughly 12 | under 1% | **thin**, and the thinness is the finding |
| Reports of a good experience with this brand's own service | 2 | 0.2% | **thin** |
| Records arguing with the ad's central claim | 103 | 7.8% | across 13 ads |
| Records disclosing the commenter's own deductible or premium | 160 | 12.1% | across 17 ads |

For a corpus this size, twelve recognitions is very low. The mining method warns against reading a positive review as a usable finding, but it says nothing about a corpus with almost no positives at all, and this is that corpus.

### Sentiment by source, by SKU, and by time period

**By source.** Not computable. There is one source.

**By SKU.** Not computable. There is no product field on any record.

**By time period.** The counts are real but the comparison is not safe. 846 of 1,322 records (64.0%) sit in March and April 2026, so any period comparison is really comparing one heavy campaign window against a set of thin ones. The one time-shaped read the full corpus does support is the objection about being buried in sales calls: in 2025 it appears as a report from someone who filled the form, and by 2026 it appears as fear from someone who has not. Both wordings are in the quote index below. `inferred`, from the dates on the two clusters.

### Strongest positive and negative themes

**Strongest negative, by ad spread rather than raw count**, because spread survives the time skew and raw count does not. All carried from the full read, all `stated` at the count and `verified` as present in the corpus by my own string checks.

| Theme | Records | Ads it appears on | Share of 1,322 |
|---|---|---|---|
| Pre-existing conditions disqualify you | 55 | 17 | 4.2% |
| The insured but still broke disclosure | 160 | 17 | 12.1% |
| The pregnancy exclusion under a brand called Health For Moms | 42 | 15 | 3.2% |
| Political blame for the cost of insurance | 54 | 14 | 4.1% |
| That is not a deductible, it is an out-of-pocket max | 103 | 13 | 7.8% |
| This is a scam | 45 | 12 | 3.4% |
| What about dads? | 16 | 12 | 1.2% |
| Rival agents pitching a competing offer | 39 | 10 | 3.0% |
| Drop insurance and pay cash instead | 33 | 10 | 2.5% |
| You will sell my number and I will get buried in calls | 15 | 10 | 1.1% |
| My kids are grown, do I still count as a mom? | 16 | 7 | 1.2% |
| This creative is AI and I do not trust it | 32 | 7 | 2.4% |
| My state is not on the list | 9 | 6 | 0.7% (**thin**) |

**Strongest positive.** There is one, and it is small. Roughly 12 recognition records, nearly all on the `MOMS38 - 2` skit family. **thin** by the ten-record rule at the level of any single variant, and only just above it for the family as a whole.

## Motivation and trigger profile

This is the section where the shape of the source hurts most. A review corpus opens with why the customer bought. An ad comment corpus opens with why the viewer disagrees. So the motivations below are what people say drove them to the ad, not what drove anyone to buy, and no record in this corpus is confirmed to belong to a buyer.

**Counted motivations and triggers.**

| Motivation or trigger | Records | Basis | Confidence |
|---|---|---|---|
| Cost pain disclosed with a specific dollar figure | 202 of 1,322 (15.3%) contain `$`; the full read classified 160 (12.1%) as self-disclosure of the commenter's own deductible or premium, across 17 ads | structured string count, then a model tag | mixed |
| An eligibility question asked directly of the brand | 166 of 1,322 (12.6%) contain a question mark; 42 (3.2%) contain "qualify" | structured | mixed |
| Employer coverage as the reason she cannot act | 24 of 1,322 (1.8%) contain "employer," 7 (0.5%, **thin**) contain "my job" | structured | mixed |
| An acute medical event already scheduled | 6 of 1,322 (0.5%, **thin**) contain "surgery" | structured | thin |
| A named alternative being compared against | 36 (2.7%) mention Obama or Obamacare, 17 (1.3%) mention Medicaid | structured | mixed |
| Prior bad experience with the brand's own funnel | 15 of 1,322 (1.1%) across 10 ads, carried from the full read | model tag | mixed |
| Waiting for open enrollment | 1 of 1,322 (0.1%, **thin**) | structured | thin |

**Jobs to be done, read from the language.** `inferred`. Three jobs show up in the text often enough to name. First, stop paying a premium every month and still owing thousands before anything is covered. Second, find out whether she is even allowed to switch, which is a permission question rather than a price question. Third, get a real number without handing over a phone number, which is a friction job the current funnel does not serve.

**The final-straw trigger.** The sharpest one in the corpus is the moment she learns the number. One record, on `MOMS38 - 1 - V1` on 2026-03-22, carries 47 likes, the highest in the corpus: "This sounds too good to be true. I pay over $1,000 a month for a premium. We have to pay an $8000 deductible per family member or up to $17,000 for the entire family. It's insane. I have 2 members of the family with chronic diseases. This absolutely insane. I want the 1990's back." That is grief about a bill, not shopping behavior.

**Ad and influencer mentions.** No influencer mentions of any kind. The ad itself is mentioned constantly, but almost always to dispute it. `verified` from the corpus read.

**Recommendation and word-of-mouth mentions.** Effectively absent as a positive signal. The mining method calls referral language one of the highest-value signals to hunt for, and this corpus has close to none of it pointing toward the brand. What it has instead is 39 records (3.0%) across 10 ads where a rival agent recommends a different offer.

**Urgency and discount mentions.** None found. No promotion, no sale, no deadline language. Consistent with a lead-generation account that has no price to discount.

## Gifting, usage, and occasion profile

**Almost none of this section applies, and padding it would be dishonest, so it stays short.**

There is no gift purchase in this category. Health insurance is not given. There is no recipient reaction, no special occasion, no repeat gifting, and no records supporting any of them. Gift versus self purchase is marked unavailable in the classification method for exactly this reason.

The one thing in this territory the corpus does support is **buying on behalf of someone else**, which is the closest real analogue to gifting here and is worth carrying because it is a persona signal.

| Signal | Records | Share of 1,322 | Confidence |
|---|---|---|---|
| Mentions a husband | 19 | 1.4% | mixed |
| Mentions a dad or dads | 17 | 1.3% | mixed |
| Asking about coverage for a man in the household, classified from the full read | 16 across 12 ads | 1.2% | mixed |
| Mentions a child in college | 3 | 0.2% | **thin** |

The pattern under those numbers, `inferred`: the questions about men are mostly asked by women, on behalf of a husband, a son, or an ex. One record on `MOMS38 - 1 - V2` on 2026-04-23 states it outright: "With income restrictions? Also I'm a mom but I carry the insurance for my whole family, including dad. Can he get on this magical plan?" That says the woman being targeted is often the household's insurance buyer for everyone, not just for herself. Worth carrying into persona work.

**Life stage as the real occasion.** In place of usage occasions, this category has life stages, and three show up: pregnancy or planning one (38 records, 2.9%), a child aging out of the house (16 records across 7 ads, 1.2%), and a job or benefits change (24 records mention an employer, 1.8%). All three are the moment the coverage question opens, which is the closest thing to an occasion this product has.

## Objections and barriers profile

This is the richest section in the corpus, and that is exactly what you would expect from a public comment section. People come to an ad's comments to object. Read every number here knowing the surface selects for it.

| Barrier | Records | Ad spread | Share of 1,322 | Basis |
|---|---|---|---|---|
| Medical underwriting, pre-existing conditions | 55 | 17 ads | 4.2% | model tag; 38 records (2.9%) contain "existing" as a structured check |
| The pregnancy exclusion | 42 | 15 ads | 3.2% | model tag; 38 records (2.9%) contain "pregnan" |
| Product confusion, deductible versus out-of-pocket max | 103 | 13 ads | 7.8% | model tag; 207 (15.7%) contain "deductible," 74 (5.6%) contain "out of pocket" |
| Legitimacy, "this is a scam" | 45 | 12 ads | 3.4% | structured string count |
| Fear the brand sells your number | 15 | 10 ads | 1.1% | model tag; 49 records (3.7%) contain "call" |
| A rival offer pitched in the thread | 39 | 10 ads | 3.0% | model tag |
| The whole category is the problem, self-insure instead | 33 | 10 ads | 2.5% | model tag |
| Eligibility confusion about the word "mom" | 16 | 7 ads | 1.2% | model tag |
| Distrust of AI-presented creative | 32 | 7 ads | 2.4% | model tag; 25 of the 32 sit on one 2025 ad |
| My state is not covered | 9 | 6 ads | 0.7% | model tag, **thin** |

**Price concern.** Present in nearly every record that carries a dollar figure, which is 202 of 1,322 (15.3%), but almost never aimed at this brand's price, because this brand never states one. The price concern here is about the plan the commenter already has. That is a different objection from the usual price objection and a downstream pass should not collapse them.

**Shipping, delivery, stock, compatibility, and fit issues.** None. Not applicable to this category, and no records support any of them.

**Service issues.** The service complaints in this corpus are about what happens after the form, not about a product. The clearest one, on `MOMS38 - 1 - V3` on 2026-03-16, drew 33 likes, the third-highest in the corpus: "Filled it out and have been getting calls everyday from all sorts of companies which are mostly India based.  Also, the harassment from whomever keeps calling me about Medicare (India again).  This is the ONLY form I've filled out since getting my new phone number 3 months ago so it came from this site!"

**The one objection the brand does not know it has.** The brand's stated objection list, from its own context document, names five: is this legit, I do not want to be sold to on a call, I do not have time, my state probably is not included, and I should just wait for open enrollment. The widest objection in its own comment sections, the pregnancy exclusion at 42 records across 15 ads over fourteen months, is not on that list. `verified` as a gap between the two documents, since the full read inspected both. Nine of those 42 records open by quoting the brand's own name back at it.

**Negative-review concerns.** One record is itself a negative review summary. On 2025-01-13 under the ad `IMG 6`, a commenter pasted a summary of Reddit discussion concluding the brand is "generally considered not legitimate and likely a scam," and it drew 14 likes. `stated`, not verified. It is a commenter's summary of a forum this brand has not pulled, and it is one of the strongest arguments for pulling Reddit.

## Product experience and outcome profile

**This section is largely blank, and the blank is the finding.**

There is no product experience in this corpus, because there is almost nobody in it who has the product. No commenter is confirmed to have bought a plan. There are no praised features, no criticized features, no durability, design, ease-of-use, or performance records. Those categories do not apply to a lead-generation handoff, and even the ones that could apply have no supporting records.

What does exist, counted honestly:

| Signal | Records | Share of 1,322 | Confidence |
|---|---|---|---|
| Reports of a good experience with the brand's service | 2 | 0.2% | **thin** |
| Reports of a bad experience after submitting the form | 15 across 10 ads | 1.1% | mixed |
| Confusion after starting the qualification flow | present, exact count not established | data-limited | mixed |
| Expectations exceeded | 0 | 0% | none |
| Problem solved | 0 | 0% | none |

**The two positive records, in full, because they are the only ones that exist.** On `Moms Nahuel WV#1 - V9`, 2026-04-17, with 2 likes: "Best advice I have gotten from an insurance agent! She didn't have anything that fit but pointed me in the right direction!" And on `MOMS38 - 1 - V1`, 2026-04-01: "I was connected to a very helpful agent. They weren't able to find a lower price for our particular situation but he was very kind and helpful and respectful."

Both people were told no. Both left praise anyway. Two records out of 1,322 is **thin** by any standard and cannot carry a pattern. They are kept because they are the only public evidence that exists anywhere for this brand's service quality, and a later pass should know that this is the whole of it rather than assume more is out there.

**First impressions of the funnel.** One record from 2025-01-20 names the friction directly: "Monique M Endriss I tried to look at them through a regular internet browser and nothing comes up...the link only works through Facebook and they want all your information before they show you anything....sounds like a scam to me." And on `MOMS38 - 1 - V1`, 2026-03-15, with 3 likes: "Just give some pricing without making people sign up 🙄". `stated` on both. They are single records, not patterns, but they name a specific step in the flow.

## Transformation and impact profile

**Empty, and the emptiness is the single most important structural fact about this corpus.**

Across all 1,322 records there are zero before-and-after stories about this brand's product, zero routine changes, zero behavior changes, zero confidence changes, zero relationship changes, zero habit changes, zero measurable-result mentions tied to this brand, zero repeat-purchase statements, and zero won't-buy-again statements. `verified` by the full corpus read.

The mining method names transformation as one of the highest-leverage patterns to hunt for, with the from-state and the to-state both captured. This corpus has from-states in abundance and no to-states at all. People describe the problem at length. Nobody describes the other side of it with this product.

**The one transformation shape that does appear points away from the brand.** A handful of records describe leaving insurance entirely, which is a real from-state and to-state pair, just not one the brand wants. On `MOMS38 - 1 - V8`, 2026-03-21: "I stopped paying for health insurance. Its actually WAY cheaper to not have insurance. We have saved thousands and that includes xrays treatments routine visits". And on `MOMS38 - 1 - V2`, 2026-03-26, with 14 likes: "I would rather have no insurance you would get better self-pay rates then you do with \"having coverage\"". 33 records across 10 ads carry that shape (2.5%). `inferred` on the read: the brand's own hook, which agrees that insurance is a scam, is what opens the door to it.

**Recommendation statements.** 39 records across 10 ads (3.0%) are recommendations, and every one of them recommends somebody else. The clearest is a repeated script under the account's highest-spend ad on 2026-04-07: "Heather, you can pair Direct Primary Care with a low premium health plan and have a comprehensive health plan...Check mapper.dpcfrontier.com for a location near you."

**What would fix this section.** Nothing in the ad comments. Transformation language lives in reviews and post-purchase surveys, and this brand has neither. Until one exists, every downstream pass asking for outcome or transformation language for Health For Moms should be answered with this section rather than with invented copy.

## Language and creative-asset index

Every quote below is verbatim, exactly as written, with its original spelling, punctuation, casing, and emoji preserved. Every one carries its row source: source type is `ad-comment` and platform is Facebook or Instagram on Meta ad account act 484897827497337 for all of them, so those two fields are stated once here rather than repeated. There is no rating and no product on any record, and `permalink_url` is null on all 1,322 rows, so no quote can carry a link. Row ids are given where I pulled the record myself.

### Golden nuggets

Lines that could be lifted nearly as written.

- "This sounds too good to be true. I pay over $1,000 a month for a premium. We have to pay an $8000 deductible per family member or up to $17,000 for the entire family. It's insane. I have 2 members of the family with chronic diseases. This absolutely insane. I want the 1990's back." — row `b7aa4d37-2243-d0fe-03e6-50c8b7d495ca`, `MOMS38 - 1 - V1`, 2026-03-22, 47 likes, 9 replies. The most-liked record in the corpus.
- "Markets to moms.\nProvides zero plans for moms. 🚩\nMakes perfect sense." — row `184aaf10-b07b-3145-feae-4376d3f497de`, `B1 samar- Copy`, 2025-07-29, 15 likes. Usable only as an objection to answer, never as a claim.
- "Lucky! Mine is $11,000" — row `aa3d6d52-d3a5-63ad-78bb-570b4939eb59`, `MOMS38 - 1 - V3`, 2026-03-17, 19 likes.
- "Moved from NY to GA. Went from $6500 deductible to $250 🙌🏼" — row `67902773-6f7b-9c0a-4dc3-42d08a70c586`, 2026-08-14.
- "Best advice I have gotten from an insurance agent! She didn't have anything that fit but pointed me in the right direction!" — `Moms Nahuel WV#1 - V9`, 2026-04-17, 2 likes.

### Headline-worthy phrases

- "I want the 1990's back." — inside row `b7aa4d37`, 2026-03-22.
- "Anyone actually have this and have insight?" — row `7d74447b-bc85-97f5-c3ec-39d711ff885b`, `MOMS38 - 1 - V1`, 2026-03-20, 15 likes.
- "How many calls will I get if I try to see how this works?" — row `3707bfa1-c0bd-2629-63b4-6987e500f611`, `Moms36 - 3 - A - 2 - V4c`, 2026-05-17, 17 likes.
- "There is no middle class on the marketplace unfortunately. You either pay next to nothing or almost all of it with no subsidy." — `B1 samar- Copy`, 2025-08-09.

### Pain phrases

- "I'll be uninsured until I die." — from "Don't bother looking into it if you're diabetic . I'll be uninsured until I die.", `B1 samar- Copy`, 2025-08-14.
- "This year it took 35 days to hit our 8k OOP. Next year it could take as few as 1 depending on how prescriptions hit. Child is on 1 med that is $3600 per fill. I am on a combo of meds that are $2,600, 1,800, and $3,200." — `MOMS39 - 2 - V2`, 2026-03-31.
- "so by December just hit it...oh but its Jan. Now so it starts over...and they still never cover anything.... insurance is the biggest scam 😒" — `MOMS38 - 1 - V3`, 2026-03-24.
- "I literally hate NYE for this reason!" — `MOMS38 - 1 - V3`, 2026-04-04, 6 likes.
- "girl, we pay $2,200 a month and its a battle for them to cover anything. I have MS so I NEED to be covered for my treatments" — `MOMS38 - 1 - V1`, 2026-03-23, 4 likes.
- "Mines fuckin 10K!" — row `ea8684c2-d037-9b10-1570-fae48a5f0d00`, 2026-03-27. Fails the voice check as written; the observation survives.

### Outcome phrases

**Empty.** No record in 1,322 describes an outcome from this brand's product. This heading is kept so a later pass sees the blank rather than assuming the category was skipped.

### Objection phrases

- "How can you have healthcare for moms if you don't cover maternity? Makes zero sense. False advertising." — `B1 samar- Copy`, 2025-08-12.
- "Health for Moms, but only if your babies are out of the womb. I was denied for being pregnant. Scam." — `MOMS30 - 1 - V20`, 2026-02-03.
- "\"Health for Moms\" but you don't have plans for women who are pregnant?" — row `c7b7448d-2b4b-113b-cb7f-07d28e8cf659`, 2026-05-07, 2 likes.
- "Preexisting health condition of cancer disqualified me" — row `3bcd0ddf-30f5-1e4c-a318-1868b9e7055f`, `moms-63 3e`, 2026-09-02. One day before this doc was written, which shows the objection is live.
- "It only works if you don't have any preexisting conditions. You gotta be perfectly healthy to qualify it looks like" — `Moms43 - 4 - V3`, 2026-08-13, 2 likes.
- "That's not a deductible that's a medical maximum out of pocket. You should educate people, not misinform!!" — `MOMS38 - 1 - V5`, 2026-03-29, 2 likes.
- "Deductible is different than maximum out of pocket 😃 -an insurance agent" — row `b41c3c21-4571-2770-b3ae-65e929619418`, `MOMS38 - 1 - V1`, 2026-05-01.
- "I filled this out because it literally says we won't be contacted by random agents. That's a lie. I immediately received 5 text messages from 5 different agents claiming to be from 5 different companies." — `B1 samar- Copy`, 2025-11-28.
- "Is putting in my information to look at prices going to end up qith 50 million calls from health insurance people..." — row `2687e7d3-5e0f-53d7-84fb-78316fe8c95d`, 2026-04-04.
- "Ha… \"in these states\" proceeds to list all 50 states… scam" — `MOMS38 - 1 - V2`, 2026-03-26.
- "Why is this being shown in IL if it's not on the list???😭🤦🏼‍♀️" — row `713721dc-21b1-d455-1fdd-ca76dc7ed44e`, `moms-53 3`, 2026-09-02.
- "But if you make under 30k a year you don't qualify smh" — row `45b22fb4-ca7c-f1bb-b935-21e946bcae2c`, 2026-09-01.
- "Ok. What if you or your children have a preexisting condition? Is it guaranteed renewable? Whats the catch, because I guarantee there is one." — row `5db97499-85e1-b2d1-619f-8e89522382d5`, 2026-05-26, 3 likes.

### Trigger moments

- "This is what I'm afraid of. Just found out I desperately need a hysterectomy. My husband is looking into insurance for me so that I can get it done." — `MOMS38 - 1 - V2`, 2026-04-14.
- "how can I get that because I pay $1000 a month for my insurance and tomorrow I have surgery" — row `c1478851-ccf4-9289-116a-345c3d6a8f51`, `MOMS39 - 2 - V2`, 2026-05-04.
- "Our deductible is $10,500 😭 And I have to have surgery in June" — `MOMS38 - 1 - V10`, 2026-04-02.
- "Mine is $8,000 and I hit it in the beginning of march 🤣😭" — `MOMS38 - 1 - V8`, 2026-03-26, 2 likes.
- "Does this work in Louisiana? Because they wouldnt let me apply for good insurance here until November." — `Moms43 - 4 - V3`, 2026-05-27.

### Metaphors

Thin, and worth saying so, since the mining method calls metaphor one of the two highest-value signals most passes miss. This corpus has very little of it. What exists:

- "insurance is the biggest scam 😒" — `MOMS38 - 1 - V3`, 2026-03-24. Scam is the corpus's dominant metaphor, present in 45 of 1,322 records (3.4%).
- "Can he get on this magical plan?" — `MOMS38 - 1 - V2`, 2026-04-23. Magical is the sarcasm the audience reaches for when the offer sounds too good.
- "Health and Car insurance are the biggest legal scams that are RDQUIRED to be payed into." — row `85ad24c4-1ffa-c22c-da1c-617049382bcf`, 2026-04-14.
- "🐂 💩" — row `de858497-6dd2-acfc-8a11-74cc6941113c`, 2026-04-08. A metaphor rendered entirely in emoji.

### Category jargon

The audience is far more fluent in this category than the creative assumes, and the jargon count is the proof.

- deductible, in 207 of 1,322 records (15.7%)
- out of pocket and OOP max, in 74 (5.6%)
- premium, in 46 (3.5%)
- coinsurance, in-network, guaranteed issue, medical underwriting, marketplace, subsidy, HSA, self-pay, health share, Direct Primary Care, certified application counselor
- "A deductible ≠ out of pocket max. You should consider yourself lucky if your OOP Max is $6,000." — `MOMS38 - 1 - V3`, 2026-03-23.
- "Marketplace plans are guaranteed issue by law, meaning there is no medical underwriting, as long as he's eligible to enroll during a valid enrollment period." — row `96452dd4-651e-9034-cd92-5fa35c41e6e1`, 2026-08-21.

### Anti-language

What the audience explicitly rejects in the category's marketing and in this brand's own.

- "Marketing towards mothers while not covering pregnancy is a disgusting tactic." — `B1 samar- Copy`, 2025-11-23.
- "Please dont use AI instead of actors. AI advertizing use in spite of actors goes against the morals that health for moms promotes" — `B1 samar- Copy`, 2025-07-20.
- "This is the problem with AI online commercials. If you are using a fake person for your testimonial, it unintentionally sends a message to people that no real actual person would say this about your service." — `B1 samar- Copy`, 2025-07-25.
- "Creepy AI blonde lady ruins the ad tbh" — `MOMS38 - 1 - V2`, 2026-04-05.
- "As a licensed insurance broker this is VERY misleading in the beginning." — `MOMS38 - 1 - V1`, 2026-04-07.
- "It's illigal to deny coverage for women who are pregnant so yall need to keep that in mind with the deceitful marketing" — `B1 samar- Copy`, 2025-12-20. `stated`, a commenter's legal read, carried as language and not endorsed.

### Outliers

- 49 records that are the single word "Help" or "help," all on one ad, `Moms43 - 4 - V3`, between May and September 2026. `data-limited` on meaning.
- "I thought it was a Disney world membership" — row `56ef84e8-2aa8-daed-6d53-541a99f9ce0f`, 2026-09-02.
- "I'm sure the mom that can afford matching outfits prob just pays in cash 🤦‍♀️" — row `3fb95c2d-c637-a6a4-d741-fc04c9552ecd`, `moms-63 2b`, 2026-09-03. A direct read on the creative's casting.
- "This is why we stayed in the military and retired. Very good insurance for the whole family" — row `6d602436-00a7-24ec-5347-6d5c05e59ac5`, 2026-04-18, 19 likes.
- "What about dads 🙁 some of us are permanently physically fucked up for the rest of our lives from taking care of our households... I am the one racking up medical debt for my family 😢 makes me feel like a pile of shit." — `MOMS38 - 1 - V9`, 2026-04-04.

### Whole-review concept candidates

Records whose entire structure maps to a producible ad.

- **The deductible auction.** The `MOMS38 - 1` thread where the ad states $6,000 and the comments bid it up: "Wow only 6? Must be nice" (13 likes, 2026-03-27), "$6000???? Huh mine is $18000 .....where can I get the $6k" (2026-03-26), "6k....try 13k!" (2026-04-02), "Mine is 18,000" (2026-04-05). The whole thread is the concept.
- **The denial skit that people said was true.** The `MOMS38 - 2` family, where a woman plays both the mom and the rep. The reaction is the asset: "\"It's out of network\"  \"But it's in the same building!\"  \"In a different hallway\"  🤣🤣🤣🤣🤣 whoever came up with this ad deserves a raise!! Love this!" (2026-04-03, 4 likes), "TRUTH! A SAD TRUTH." (2026-04-06), "At the Mayo Clinic for my husband right now. Absolutely dealing with this." (2026-04-06).
- **The permission she did not know she had.** A commenter answering another commenter on 2026-05-05, `MOMS38 - 1 - V2`: "if it's an employer insurance, you don't have to sign up with that employer insurance you can decline the coverage and go out and find your own insurance carrier". A customer is teaching the audience something the brand never says.

### Brand-self-echo candidates

Flag these as low confidence wherever they surface, per the mining method's echo rule.

- **"Make that make sense."** The ad `MOMS39 - 2 - V2` overlays a tweet reading "My deductible is $6000... Make that make sense...." and commenters then write "Health care for moms but you don't qualify if your pregnant? Make that make sense." (2026-05-05) and "make that make since!!!" (2026-03-24). The brand handed the audience a sentence pattern and the audience turned it around. This is brand language coming back, not customer language, and it must not enter the phrase bank as a customer phrase. `verified` — both the creative overlay and the commenter phrasings were read directly.
- **"Insurance is a scam."** The hook of `MOMS38 - 1 - V1` puts "Health Insurance is a scam 🙄" on screen, and 45 records (3.4%) use the word. Some of that is genuine customer language predating the ad, and some is the audience repeating the ad back. The two cannot be separated in this corpus. Treat the whole scam cluster as mixed confidence for echo.

## Data limitations

**The corpus is one source, and it is the weakest kind.** Facebook ad comments are public and performative. People post there to argue, correct, warn strangers, or be seen agreeing. Buyers who are satisfied have no reason to post, and the two who did were told no. Every rate in this doc is a rate among people who chose to type under an ad, and that is not the same population as the people who bought.

**Customer reviews: zero rows.** Verified live on 2026-09-03 through `search_customer_reviews_sql`, unfiltered, which returned `totalReviews: 0`. The team confirmed this directly in Slack on 2026-09-03: "we don't have reviews but you can pull from competitor reviews or health insurance Reddit etc." This is not a broken pipe. There is nothing there.

**Post-purchase surveys: zero rows.** Verified live on 2026-09-03 through `semantic_search_post_purchase_survey`, which returned `totalResponsesForBrand: 0` with the collection existing. No survey platform is connected and no CSV has been uploaded.

**Competitor and category reviews: no tracked brands.** No rival brands exist in the Parker app for this brand, so the substitution the team suggested cannot be run yet either. The competitor branch was deferred at the user's request on 2026-09-03. Nothing here has a category baseline, so no objection rate in this doc can be called high or low for health insurance lead generation.

**Reddit and forums: not pulled.** One record in the corpus is itself a summary of Reddit discussion about this brand, drawing 14 likes, which makes the Reddit gap the most valuable missing source rather than a nice-to-have.

**No identity fields at all.** `author_name` and `author_id` are null on all 1,322 rows. Unique commenters cannot be counted, one person cannot be tracked across threads, and repeated posts by a single operator inflate every count they touch. Every "how many people" statement anyone makes from this corpus is really "how many comments." `verified`.

**No rating, score, or product field.** No sentiment split, star distribution, NPS, or per-SKU read can be computed for this brand. Any such number appearing downstream is invented.

**No link back to any source thread.** `permalink_url` is null on every row, so no quote in this doc can be verified by opening the original post. Verification runs through the row id and the tool, not through a URL.

**No join between a comment and a lead.** Parker holds no connection between these 1,322 records and the 4,336 leads the account produced in the last 90 days. Nothing here can be said to have cost or won a single lead.

**Heavy time skew.** 846 of 1,322 records (64.0%) sit in March and April 2026. Trend reads across this corpus compare one heavy window against thin ones and should be avoided.

**Heavy ad concentration.** 795 of 1,322 records (60.1%) sit on the `MOMS38 - 1` creative family, carried from `source-pulls/ad-comments.md`. This is closer to a deep read of one campaign than an even read of the account. Ad spread is the more durable number than raw count, which is why it is carried on every theme in this doc.

**Six blank text rows** (0.5% of the corpus) carry no analyzable language. One of them holds 7 likes, which suggests lost media.

**Keyword counts over-match in places, and the affected lines are marked.** "mom" also matches "moment," "state" also matches "estate" and "statement," "love" also matches "gloves." Those counts are ceilings, not exact theme counts, and the table says so on each line.

**The tool's count field cannot be trusted without a text filter.** An unfiltered call returned `total: 0` while returning rows, and a date-filtered call did the same. Every count in this doc came either from a text-filtered call, where the total is correct, or from an offset probe I ran to find the end of the result set.

**No persona slugs exist yet.** `personas-profile.md` has not been written, so no record in this corpus carries an identity or behavioral-signal tag. Every extraction pass downstream must leave `identity_tag` and `behavioral_signal_tag` null and note the gap rather than inventing a slug.

**No product audit yet.** `website-and-product-audit.md` has not been written, so there is no SKU or product-line vocabulary to normalize against, and there is no product field on the corpus to normalize anyway.

**Sample size warnings, applied.** Everything under ten supporting records is marked **thin** in the tables above: the state-exclusion objection at 9, cancer mentions at 9, surgery mentions at 6, "accurate" at 6, single-mom mentions at 5, college mentions at 3, enrollment at 2, open enrollment at 1, and the two positive service reports. These can be quoted. None of them is a pattern.

**What no amount of reading here can produce.** Who bought. What the buyer sounds like. Whether the product delivers. Whether any objection here costs a lead. Those answers live in a review pipeline, a post-purchase survey, or a lead-level join, and this brand has none of the three.

## Open loops

The corpus-profile prompt does not ship with the open-loops block that its nine sibling extraction prompts carry, so these were generated against the canonical rubric. They are deliberately **not** the loops already filed in `source-pulls/ad-comments.md`. Every one below came out of the counting work in this pass. Infrastructure gaps, meaning the missing reviews, missing surveys, and missing competitor set, are routed to data limitations above rather than written as loops, per the rubric.

**1. Two months hold two thirds of everything the brand has ever heard from its audience.**

March 2026 holds exactly 340 comments and April 2026 holds exactly 506, which is 846 of 1,322, or 64.0%, in a 61-day window. All of 2025 holds 227, or 17.2%, across twelve months.

Pull: **Surprise.** Given a brand that has been advertising since at least January 2025, a comment volume five times higher in two spring months than in a full prior year is not what the setup would predict, and the size of that gap is the signal.

Question: What changed in March and April 2026 that made this audience talk five times more than it ever had before?

Why it matters: if the spike is spend, the corpus is just a budget artifact and every rate in this doc should be discounted. If the spike is the creative, then one specific ad found a nerve the rest never touched, and finding out which nerve is worth more than any single objection count here.

Territory: **Messaging.**

**2. One record in eight is a question, and almost none of them get answered.**

166 of 1,322 records (12.6%) contain a question mark, and 42 (3.2%) contain the word "qualify." The full read found the brand does not answer on the thread, and in at least one case another commenter had to explain that declining employer coverage is allowed.

Pull: **Gap.** There is obvious demand sitting in plain sight and nothing appears to have been done with it.

Question: What happens to lead volume when the brand answers the eligibility questions in its own comment sections?

Why it matters: these are people raising a hand at the cheapest possible point in the funnel, before any form, and right now the only people answering them are rival agents. If replying converts even a fraction, comment response becomes a performance lever rather than a housekeeping chore.

Territory: **Messaging.**

**3. The audience talks about insurance far more than it talks about being a mom.**

"Insurance" appears in 284 of 1,322 records (21.5%). "Mom" appears in at most 73 (5.5%), and that figure is inflated because the string also matches "moment." The brand's entire creative device is that one word.

Pull: **Surprise.** For a brand named Health For Moms whose ads turn on the word "mom," the audience using the category word nearly four times as often is not what the setup would predict.

Question: How does this audience describe who she is when she talks about buying health insurance?

Why it matters: it decides whether "mom" is the identity the creative should lead with or a wrapper that is quietly generating eligibility confusion. 16 records across 7 ads are already asking whether grown kids still count, and 16 across 12 ads are asking about dads.

Territory: **Personas.**

**4. The brand's own stated timing objection is almost invisible in its comment sections.**

The brand context document names "I should just wait for open enrollment" as one of its five main objections. The phrase "open enrollment" appears in 1 of 1,322 records (0.1%), and "enrollment" in any form appears in 2 (0.2%). Meanwhile the pregnancy exclusion, which is on no stated list, appears in 42 across 15 ads.

Pull: **Tension.** The brand's account of what its buyers object to and the record of what they actually type cannot both be right as stated.

Question: Where does the timing objection actually show up for this brand, if it barely shows up in the comments?

Why it matters: the stated objection list is what the creative is built to handle. If two of five stated objections are not the real ones, the creative is answering questions nobody is asking and leaving the loudest one untouched.

Territory: **Messaging.**

**5. Three quarters of the corpus is a comment nobody agreed with.**

At least 331 and at most 390 of 1,322 records, roughly 25% to 30%, carry at least one like. The other 932 to 991 carry none. Yet the ten most-liked records include political blame at 36 and 24 likes, a warning about sales calls at 33, and a deductible disclosure at 47.

Pull: **Pattern.** The same few kinds of comment keep collecting the agreement while the bulk of the corpus collects none, and that split looks like it means something rather than being noise.

Question: What do the comments that earn agreement have in common that the silent three quarters do not?

Why it matters: agreement is the only proxy for resonance this corpus offers, since there is no rating field anywhere. If the shape of an agreed-with comment can be named, it is the closest thing to a message test this brand can run without spending anything.

Territory: **Messaging.**
