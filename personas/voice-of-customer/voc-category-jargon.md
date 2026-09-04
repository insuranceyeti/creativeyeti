---
brand: health-for-moms
doc: voc-category-jargon
category: category_jargon
generated_on: 2026-09-04
refresh_by: 2026-10-04
live_pulls_run_on: 2026-09-04. Every Parker MCP call behind this doc ran today, against a corpus re-pinned live at 1,342 by my own offset probe. The earliest sibling docs ran on 2026-09-03 against 1,322 and say so; carried figures keep their 1,322 denominator and are labelled.
corpus_denominator: 1342 Facebook and Instagram ad comments, Meta ad account HealthForMoms, act 484897827497337
corpus_date_range: 2025-01-08 to 2026-09-03
prior_version: none. First run. No recurrence history to carry forward.
snippets_captured: 17
terms_the_brand_also_uses: 4 of 17
sources_read:
  - Parker MCP search_facebook_ad_comments_sql, 31 filtered pulls on 2026-09-04, one or more per term plus spelling variants. Every count and row id here was re-derived by me from the returned rows, not carried from an upstream doc.
  - Parker MCP search_facebook_ad_comments_semantic, two passes on 2026-09-04 to catch fluent usage that a term search would miss. Both reported totalCommentsAnalyzed 1342.
  - Parker MCP search_customer_reviews_sql, unfiltered, 2026-09-04. Returned totalReviews 0. Checked live by me.
  - Parker MCP semantic_search_post_purchase_survey, 2026-09-04. Returned totalResponsesForBrand 0 with the collection existing.
  - Parker MCP search_facebook_ads_sql, 2026-09-04, lifetime mode with the scripts block, top ten ads by lifetime spend. Read at full media depth, because the only way to tell category jargon from a brand term the audience is repeating is to know which words the creative actually says.
  - source-pulls/brand-self-echo-detection.md, for the standing verdicts. The deductible-framing verdict and the out-of-pocket finding are carried forward, not re-judged.
  - personas/voice-of-customer/voc-corpus-profile.md, for field coverage, corpus bias and carried theme counts.
  - personas/voice-of-customer/voc-objection.md, voc-pain-phrase.md, voc-metaphor.md and voc-anti-language.md, the sibling extractions, used to route the correction argument and the vivid language away from this pass so only the vocabulary stays.
  - running-notes/missing-context.md and running-notes/brand-rules.md.
  - parker-system/creative-strategy-context/customer-review-mining-method.md and persona-research-and-creative-strategy-process.md, the two methods this pass is performed through.
expected_sources_missing:
  - customer reviews. Zero rows, verified live 2026-09-04.
  - post-purchase surveys. Zero responses, verified live 2026-09-04.
  - Reddit and forums. Not pulled, and the prompt names this as by far the richest jargon source because community members talk to each other in full shorthand with no brand present. This pass is materially incomplete without it and the gap is named on every confidence mark.
  - competitor and category reviews. No rival brands tracked in the Parker app.
  - brand-reputation, other-reviews, support tickets, organic social comments. None ingested.
  - personas-profile.md. Not yet written, so identity and behavioral-signal tags are null by rule.
data_limitations:
  - One source type only, so nothing here can rise above mixed under this prompt's confidence rule, however often a term repeats. Cross-source recurrence is what earns strong.
  - Counts are of comments containing the string, never of people. author_name and author_id are null on all 1,342 rows, so one fluent broker posting eight near-identical comments reads as eight.
  - That is not hypothetical and it is the biggest count risk in this doc. Eight of the twenty-one coinsurance rows are the same pasted sales pitch from one commenter promoting a level-funded plan with a link. Every affected count below says so on its own line.
  - Spelling variants are counted separately and summed by hand, never blended silently. Coinsurance runs across three spellings: "coinsurance" 21, "co insurance" 5, "co-insurance" 4.
  - permalink_url is null on all 1,342 rows, so url is null on every snippet.
  - The semantic comment tool and the SQL comment tool return different identifier spaces for the same row. Every review_id below is the SQL comment_id, resolved by exact-text lookup where a row was first surfaced semantically.
  - The database stores curly apostrophes, so any search written with a straight apostrophe silently misses rows. Terms were searched apostrophe-free wherever possible.
  - The SQL search is a plain case-insensitive substring match, verified rather than assumed. That means short terms over-match: "network" catches "networks", "HSA" catches "HSAs", and a search for "racket" would catch "bracket". Every count below was hand-checked against the returned rows.
  - Severe time skew. Most of this vocabulary lands in March and April 2026, inside the window the brand's own creative opened, which caps how much any first-seen date proves. This is stated on the terms where it is load-bearing.
  - refresh_by is 30 days rather than the 180-day voice-of-customer cadence, matching the sibling docs. Category vocabulary itself moves slowly, but this doc's coverage would change substantially the day a Reddit pull lands.
  - There is no get_current_time tool on this MCP surface, so the date comes from the session clock.
---

# Voice of Customer — category jargon — Health For Moms

## What this pass read, and why this is the richest category in the library

Every other pass in this build has had to report a thin corpus. This one does not. **Health insurance is a jargon-dense category and this audience is fluent in it**, far more fluent than the brand's creative gives it credit for. There is real vocabulary here, used correctly, at volume, by people who know what the words mean.

The reading surface is one thing: **1,342 Facebook and Instagram ad comments** from Meta ad account `HealthForMoms`, act `484897827497337`, 2025-01-08 to 2026-09-03. I re-pinned that total with my own offset probe today. Customer reviews returned zero rows live. Post-purchase surveys returned zero responses live. Reddit — which this prompt calls by far the richest jargon source, because that is where community members talk to each other in shorthand with no brand present — is not pulled.

That last gap matters more here than in any other pass, so it caps every mark. Cross-source recurrence is what earns `strong`, and this brand has one kind of source, so **nothing below is `strong`**. The best terms here are `mixed` because they recur heavily in one place.

One count risk, stated up front rather than buried. `author_name` is null on all 1,342 rows, so every figure counts comments, not people. In this doc specifically that bites, because a handful of insurance sellers are working these threads. **Eight of the twenty-one "coinsurance" rows are the same pasted pitch from one commenter**, word for word, addressed to eight different women, ending in a link to his own site. Where that inflates a count, the snippet says so.

## The fluency picture, measured

Here is the whole vocabulary, counted live today against 1,342 records. This table is the spine of the doc, and it is the thing a writer should read before writing a word of copy for this brand.

| Term | Records | Share | Does the brand's creative say it? |
|---|---|---|---|
| deductible | **207** | 15.4% | **Yes**, constantly |
| out of pocket | **74** | 5.5% | **No** |
| copay / copays | **46** | 3.4% | **Yes** |
| premium / premiums | **46** | 3.4% | **Yes** |
| pre-existing / preexisting condition | **33** | 2.5% | **No** |
| coinsurance, all three spellings | **30** | 2.2% | **No** |
| Obamacare | 15 | 1.1% | **No** |
| max out of pocket | 15 | 1.1% | **No** |
| marketplace | 14 | 1.0% | **No** |
| network | 12 | 0.9% | Adjacent only |
| catastrophic | 10 | 0.7% | **No** |
| self pay | 7 | 0.5% | **No** |
| HSA | 5 | 0.4% | **No** |
| 80/20 | 5 | 0.4% | **No** |
| subsidy / subsidies / subsidized | 4 | 0.3% | **No** |
| broker | 4 | 0.3% | **No** |
| health share | 3 | 0.2% | **No** |
| cash price | 2 | 0.1% | **No** |
| GoodRx | 2 | 0.1% | **No** |
| medical underwriting / guaranteed issue | 1 | 0.1% | **No** |

All counts `verified` — each is a case-insensitive substring search anyone can re-run through the same tool, and each returned row was read.

**The pattern in that right-hand column is the finding of this pass.** The brand's creative uses four of these words: deductible, copay, premium, and coverage in the general sense. `verified` from the transcripts of the ten highest-spending ads, which I read in full today. Sixteen other terms the fluent customer uses, the brand never says.

And the one it leans on hardest is the one the audience keeps telling it it is using wrong.

## The correction economy, and why it is a vocabulary finding rather than an objection

The single loudest thing happening in this corpus is people correcting the ad's terminology. `voc-objection.md` and `source-pulls/brand-self-echo-detection.md` already hold that argument as an objection cluster — 103 comments across 13 ads on a 1,322 denominator, carried. This pass does not repeat it. What this pass adds is the vocabulary the correction is made *in*, because that is the in-group language the brand could be speaking and is not.

The correction runs like this. The ad's flagship script opens with a woman saying "My deductible is $6,000. I have to spend $6,000 in medical expenses before everything is taken care of and there's no copays." `verified` from the `MOMS38 - 1 - V1` transcript. Fluent commenters point out that what she has described is not a deductible at all — it is an out-of-pocket maximum — and then they teach the whole ladder, unprompted, for free, in the brand's own comment section:

> "That's not a deductible. What she just described is an out of pocket maximum. A deductible is the amount you have to pay completely out of pocket before your insurance pays for *anything*... The out-of-pocket maximum is the amount you have to reach before everything is 100% covered."

> "You can have a 6000 deductible.. then meet your deductible and still have a 20% coinsurance so you're still responsible for 20% then once you meet your $15,000 out-of-pocket that is when things are gonna be covered at 100%."

> "That's your out of pocket maximum (aka: worst case scenario). Your deductible is lower. You meet your deductible for your co insurance to kick in. Usually then it will be 80/20. Obviously- if you're in a High deductible health plan it will be a big number, then you probably have the option to have a HSA card. Which saves you pre taxed.. and also you saying you Pay for that insurance.. that's called your premium.."

That third one is a complete glossary in a single comment. `verified`, row `052aa855-2a88-45b5-7d1f-d01d622e7e65`, ad `MOMS38 - 1 - V5`, 2026-03-29. She names deductible, out-of-pocket maximum, coinsurance, the 80/20 split, high-deductible health plan, HSA and premium, correctly, in the right order, in eight lines. She is the fluency ceiling of this audience and the brand has never spoken to her.

**The strategic read, `inferred`:** the account's creative is pitched at a woman who does not understand her plan. A meaningful slice of the audience it reaches understands it better than the ad does. `source-pulls/brand-self-echo-detection.md` reached the same conclusion from the other direction and called out-of-pocket language "the most valuable organic language in the corpus," noting the brand does not use it at all. This pass confirms that live at 74 records on 1,342 and adds the sixteen other unused terms around it.

## Three tiers of fluency, and why the tiers matter more than the list

Reading all of it, the vocabulary sorts into three tiers. `inferred`, from who uses each term and how. This is the part a writer needs, because using a tier-three word in a tier-one ad is exactly the outsider tell the prompt warns about.

**Tier one — every mom in the thread has these.** Deductible, copay, premium, out of pocket. These four carry 373 of the term-bearing records between them. They need no explanation and using them wrong is instantly caught.

**Tier two — the woman who has actually shopped for a plan.** Coinsurance, max out of pocket, marketplace, Obamacare, pre-existing condition, in-network, HSA, subsidy, 80/20. This is the vocabulary of someone who has sat with a benefits packet or a healthcare.gov screen. It is common enough to be safe — coinsurance alone runs to 30 records across three spellings — and specific enough to signal that the speaker has been through the same thing.

**Tier three — the professional.** Guaranteed issue, medical underwriting, guaranteed renewable, level-funded plan, IUA, care coordination, allowed amount, certified application counselor. These come almost entirely from brokers, medical billers and agents working the threads. They are real category vocabulary and they are **not this audience's language**. The prompt's warning applies exactly here: jargon used in the wrong context is as much an outsider tell as not using it at all. A mom reading tier-three vocabulary in an ad hears a sales office, not a neighbor.

The practical rule that falls out, `inferred`: **write in tier one, prove in tier two, never write in tier three.**

## Category jargon

Seventeen terms. Source type is `ad-comment` on every one, because it is the only source that exists. The `platform` line carries the ad the cited comment sits under. `review_id` is the Parker SQL `comment_id`. `url` is null on all seventeen because `permalink_url` is null on all 1,342 records. `identity_tag` and `behavioral_signal_tag` are null on all seventeen because `personas-profile.md` does not exist yet and this pass never invents a slug.

Every `snippet` is `stated` and exact. Every count is `verified` as a string check anyone can re-run. Every read of meaning and usage is `inferred` from the rows I read and says so. Nothing is `strong`, per the single-source ceiling.

- snippet: deductible
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: aa3d6d52-d3a5-63ad-78bb-570b4939eb59
    date: 2026-03-17
    url: null
  recurrence: 207
  source_diversity: [ad-comment]
  first_seen: 2025-05-29
  last_seen: 2026-09-03
  confidence: mixed
  brand_self_echo: false
  notes: Meaning as this audience uses it - the amount you pay yourself before the insurer pays anything - and a meaningful minority use it loosely to mean any large sum they owe, which is the confusion the whole correction cluster is about. 207 of 1,342, 15.4%, the most-used term in the corpus by a factor of nearly three. Usage condition - it almost never appears alone. It appears attached to a dollar figure, because the grammar of this corpus is name your number. The cited row is the shortest complete instance, "Lucky! Mine is $11,000," which carries 19 likes and is the highest-engagement row in the library. Echo verdict carried forward from source-pulls/brand-self-echo-detection.md and not re-judged: the deductible complaint is customer-owned, first seen 2025-05-29, with the specific complaint shape appearing 2025-11-28, three and a half months before the earliest ad carrying it. That doc also measured 95.2% of the framing inside an 83-day window the brand's creative opened, which is why this is mixed rather than higher. Claims-check clear. Voice-check in-voice - the brand already uses the word.

- snippet: out of pocket
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: de091d78-8a2f-47b0-89a4-f8d0b75be40f
    date: 2026-05-04
    url: null
  recurrence: 74, of which 15 use the fuller "max out of pocket"
  source_diversity: [ad-comment]
  first_seen: 2025-07-29
  last_seen: 2026-09-03
  confidence: mixed
  brand_self_echo: false
  notes: The most valuable term in this doc and the brand has never said it. Meaning - the annual ceiling on what you personally pay, after which the insurer covers everything. Usage condition - it appears overwhelmingly as a correction, aimed at someone who called it a deductible, which makes it the vocabulary of the audience teaching the brand. 74 of 1,342, 5.5%. Cannot be echo, because the brand does not use the phrase in any of its ten highest-spending ads, verified from the transcripts today. Carried forward from source-pulls/brand-self-echo-detection.md, which called it the most valuable organic language in the corpus at 74 of 1,322 - the count is unchanged against the larger denominator. The cited row is the clearest teaching instance in the corpus. Claims-check clear. Voice-check in-voice and this is the single strongest adoption candidate in the library.

- snippet: OOP Max
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: 3486a679-7242-6515-294d-89bbbf4ead71
    date: 2026-03-23
    url: null
  recurrence: 1 for this abbreviation, 74 for the spelled-out term
  source_diversity: [ad-comment]
  first_seen: 2026-03-23
  last_seen: 2026-03-23
  confidence: thin
  brand_self_echo: false
  notes: Captured separately from the spelled-out term because the abbreviation is a different fluency signal - shortening a term to initials is what someone does when she assumes her reader already knows it. One record in 1,342, so thin. The related abbreviations OPM and DED appear once each, in the same broker comment held in voc-metaphor.md. Usage condition - this belongs to tier two at most and should never be used in copy aimed at a general audience, because an abbreviation nobody has to decode is precisely the outsider tell in reverse: it flatters the fluent and locks out everyone else. Captured for the record, not for lifting.

- snippet: coinsurance
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: eab8e3f7-6acb-13dd-0f20-cafe015997f3
    date: 2026-03-19
    url: null
  recurrence: 30 across three spellings - "coinsurance" 21, "co insurance" 5, "co-insurance" 4
  source_diversity: [ad-comment]
  first_seen: 2026-03-19
  last_seen: 2026-05-02
  confidence: mixed
  brand_self_echo: false
  notes: Meaning - the percentage you keep paying after the deductible is met and before the out-of-pocket maximum is reached. Usage condition - it is the second beat of the correction, arriving right after out-of-pocket, and it is almost always paired with a ratio like 80/20. 30 of 1,342, 2.2%, and the count is a sum of three spellings computed by hand rather than one search. The count needs a hard caveat: 8 of the 21 closed-spelling rows are the same pasted sales pitch from a single commenter promoting a level-funded plan with a link, addressed to eight different women within six minutes on 2026-04-07. Excluding those, the genuine coinsurance vocabulary sits at roughly 22 records. Both numbers are given rather than blended. The cited row is a real mom laying out the full ladder in her own words. Brand never uses the term. Claims-check clear.

- snippet: copay
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: ed2d19f6-e044-f812-9109-53abf2855f13
    date: 2026-04-23
    url: null
  recurrence: 46, including copays and copayments
  source_diversity: [ad-comment]
  first_seen: 2025-01-08
  last_seen: 2026-09-03
  confidence: mixed
  brand_self_echo: false
  notes: Meaning - the flat fee per visit or prescription. Tier one: universally understood in this audience and used without explanation. 46 of 1,342, 3.4%, spanning the entire corpus date range, which makes it the term with the widest time spread here and the least vulnerable to the March-April skew. The brand does use it, in the negative - the flagship script says "there is no copays" - so echo needs watching, but a term appearing from the first week of the corpus and running to the last day is category-standard by any reading. Usage condition - it arrives as the thing people forget, the extra charge that survives everything else, which is why the most common construction is a warning that copays remain.

- snippet: premium
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V5
    review_id: 052aa855-2a88-45b5-7d1f-d01d622e7e65
    date: 2026-03-29
    url: null
  recurrence: 46, including premiums
  source_diversity: [ad-comment]
  first_seen: 2025-07-28
  last_seen: 2026-09-03
  confidence: mixed
  brand_self_echo: false
  notes: Meaning - the monthly payment, separate from anything you owe at the point of care. 46 of 1,342, 3.4%. Usage condition and this is the useful part - the word is most often deployed as the closing move in an argument, the thing the other person forgot to add. "And also you saying you Pay for that insurance.. that's called your premium.." is the cited row and it is a fluent commenter naming the word for someone who was describing it without having it. The brand uses "premiums" once, in the B1 samar- Copy script promising savings on them, verified. Not echo: customer use starts 2025-07-28, before that framing scaled, and it is plain category vocabulary. Claims-check clear.

- snippet: pre-existing condition
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B2 - 10TH JUNE - Copy 16
    review_id: 63b5bd3c-f128-4292-dfb6-d62cf860437c
    date: 2025-08-27
    url: null
  recurrence: 33 across the spellings pre-existing, preexisting and pre existing
  source_diversity: [ad-comment]
  first_seen: 2025-07-23
  last_seen: 2026-08-21
  confidence: mixed
  brand_self_echo: false
  notes: Meaning - a health problem you already have when you apply, which under ACA marketplace rules cannot be used to deny you and under other arrangements very much can. 33 of 1,342, 2.5%, spread across thirteen months, so this one survives the time skew cleanly. Usage condition - it is almost always the second question, right after price, and it is usually a warning to other women rather than a question to the brand. The cited row, "They don't cover preexisting conditions. Don't waste your time," carries 5 likes. The exclusion argument itself belongs to voc-objection.md and voc-anti-language.md, which hold it; only the term is captured here. Brand never says it. Claims-check gated - any copy using this term touches the eligibility rules and must be substantiated.

- snippet: Obamacare
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad Moms36 - 3 - A - 2 - V4c
    review_id: 5db97499-85e1-b2d1-619f-8e89522382d5
    date: 2026-05-26
    url: null
  recurrence: 15 for Obamacare, 14 for marketplace, both counted separately
  source_diversity: [ad-comment]
  first_seen: 2025-07-29
  last_seen: 2026-08-21
  confidence: mixed
  brand_self_echo: false
  notes: Meaning - the ACA individual market, and the name carries a political charge the formal term does not. Usage condition and this is why it matters - the corpus uses the two names for the same thing to do two different jobs. "Obamacare" shows up in arguments about blame and politics. "Marketplace" shows up when someone is describing what she actually did. Both at similar volume, 15 and 14 of 1,342. The cited row uses it in scare quotes as a grudging endorsement, "$70k out of pocket later, I am good with Obamacare," 3 likes and 3 replies. The brand says neither word in any of its ten highest-spending ads, verified, which is a deliberate-looking silence given that the marketplace is its main alternative. Claims-check clear as a customer term. Voice-check risky - the political charge on this specific word is exactly what the brand guidelines steer away from.

- snippet: Marketplace
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 8a885e35-71be-e442-a0da-f462b6eb3e9f
    date: 2025-08-09
    url: null
  recurrence: 14
  source_diversity: [ad-comment]
  first_seen: 2025-08-09
  last_seen: 2026-08-21
  confidence: mixed
  brand_self_echo: false
  notes: Captured separately from Obamacare because the wording carries different weight, per this prompt's rule that different terms for one concept get separate entries. Meaning - healthcare.gov and the state exchanges. Usage condition - this is the operational word, used by women describing what they did and what it cost, not by people arguing. The cited row is the one the echo doc singled out as the most organic-sounding comment in the corpus: "There is no middle class on the marketplace unfortunately. You either pay next to nothing or almost all of it with no subsidy." It predates most of the account's current creative and says something the brand has never said. 14 of 1,342. Claims-check clear.

- snippet: in network
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 88e4072a-3f3a-1f79-94ba-3a4ea1b3dfd4
    date: 2026-06-28
    url: null
  recurrence: 12 for network in any form, including out of network and networks
  source_diversity: [ad-comment]
  first_seen: 2025-07-25
  last_seen: 2026-06-28
  confidence: mixed
  brand_self_echo: false
  notes: Meaning - whether your doctor has a contract with your insurer, which decides what you pay. 12 of 1,342, 0.9%. Usage condition - it arrives as the hidden catch, the thing that undoes a plan that looked fine on paper. The brand gestures at the concept without using the word: the B1 samar- Copy script promises "the freedom to choose your own doctors, specialist without restrictions," verified from the transcript. That is the same idea in outsider language. Adjacent rather than echo, and the gap is the point - the brand is describing the benefit in its own words while the audience has a precise word for it sitting unused. Claims-check gated - network breadth is a hard product claim.

- snippet: 80/20
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 71c48a5b-f940-9a1b-e711-7410f1f5c0b2
    date: 2026-04-07
    url: null
  recurrence: 5 for 80/20, plus 1 record also carrying 90/10 and 1 carrying 70/30 in words
  source_diversity: [ad-comment]
  first_seen: 2026-03-28
  last_seen: 2026-04-07
  confidence: thin
  brand_self_echo: false
  notes: Meaning - the coinsurance split, the insurer paying 80% and you 20% after the deductible. Usage condition - it is spoken as a bare ratio with no explanation, which is exactly what makes it a fluency marker: nobody in these threads ever defines it. The cited row runs two ratios together, "80/20, 90/10, etc.," which is someone treating the whole family of splits as common knowledge. 5 of 1,342, so thin, and it sits entirely in an eleven-day window, which is too narrow to call a pattern. Tier two. Safe to recognize in copy, risky to lead with.

- snippet: HSA
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V8
    review_id: 6155f4df-56a0-dfdf-e091-0c5612b223a2
    date: 2026-04-18
    url: null
  recurrence: 5 for HSA and HSAs, plus 1 for the spelled-out "heath savings account"
  source_diversity: [ad-comment]
  first_seen: 2026-03-29
  last_seen: 2026-06-02
  confidence: thin
  brand_self_echo: false
  notes: Meaning - a health savings account, the pre-tax pot attached to a high-deductible plan. Usage condition - it appears as advice between women, "Get an HSA," and once as a flat rejection of that advice, "HSAs are AWFUL," which is the useful pair: the term is common enough that people argue about it rather than explain it. 5 of 1,342, thin. The one spelled-out use misspells it as "heath savings account," which is a small piece of evidence that the term travels by ear in this audience rather than off a benefits document. Brand never says it.

- snippet: catastrophic
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: 9821d190-7656-3ae3-08d7-ac1955aad88f
    date: 2026-03-16
    url: null
  recurrence: 10, of which 7 come from two commenters selling plans
  source_diversity: [ad-comment]
  first_seen: 2026-03-16
  last_seen: 2026-05-30
  confidence: thin
  brand_self_echo: false
  notes: Meaning - a plan that covers only major medical disasters, used both as a plan type and as a category of event. The count needs its caveat in the same breath: 7 of the 10 records are pasted sales pitches from commenters promoting their own products, so the genuine customer use is 3. Both numbers given, never blended. The cited row is one of the genuine three and it is the sharpest, because it reframes the brand's own offer: "That is essentially catastrophic insurance. You have to consider yourself self pay." That is a fluent customer classifying the product for other customers, and it is a harder read of the offer than anything in the ad. Thin at 3 real records. Claims-check unusable for copy without product verification.

- snippet: self pay
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 3f6fc36c-7b2e-6268-e8c9-abaf67dc4f49
    date: 2026-04-11
    url: null
  recurrence: 7 for self pay and selfpay, plus 2 for cash price and 2 for GoodRx in the same strategy
  source_diversity: [ad-comment]
  first_seen: 2025-11-27
  last_seen: 2026-05-27
  confidence: mixed
  brand_self_echo: false
  notes: Meaning - going without insurance on purpose and negotiating the uninsured rate directly with providers, which is treated here as a real strategy rather than a failure. Usage condition - it is offered as advice, and the fluent version comes with tactics attached: ask for the cash price, use a GoodRx card, take the self-pay discount. 7 of 1,342 for the term itself and 11 for the whole strategy family counting cash price and GoodRx. Marked mixed rather than thin because it is a coherent strategy recurring across five ads and ten months rather than one voice. voc-objection.md holds the exit-the-category argument; only the vocabulary is captured here. The brand never says any of it, which is notable since self-pay is its most direct competitor for this audience's dollar - not another insurer.

- snippet: subsidy
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: 87bf7f5d-1445-c1d8-1813-51f904002be8
    date: 2026-04-24
    url: null
  recurrence: 4 across subsidy, subsidies and subsidized
  source_diversity: [ad-comment]
  first_seen: 2025-08-09
  last_seen: 2026-04-24
  confidence: thin
  brand_self_echo: false
  notes: Meaning - the income-based discount on a marketplace plan, and the cliff you fall off when you earn slightly too much. Usage condition - it appears in the fairness argument, the specific grievance that being middle-income is the worst place to stand. 4 of 1,342, thin. Worth capturing despite the count because it is the technical name for the complaint that runs through the whole corpus - the brand context document quotes it as "We are super middle class, how are we stuck with everything?", a phrase source-pulls/brand-self-echo-detection.md could not trace to any customer. This is the traceable version of the same idea, in the audience's own vocabulary. Claims-check clear.

- snippet: health share
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads moms-63 3e and moms-63 3e - Copy
    review_id: f89d9430-aaa6-ef95-b0b3-775cb9d42e33
    date: 2026-08-31
    url: null
  recurrence: 3, including one as "Christian health share"
  source_diversity: [ad-comment]
  first_seen: 2026-04-09
  last_seen: 2026-08-31
  confidence: thin
  brand_self_echo: false
  notes: Meaning - a faith-based cost-sharing ministry, which is not insurance and is regulated differently. Usage condition and this is why a thin term earns a slot: the cited row is a woman asking whether Health For Moms is one. "Is this insurance or something like a Christian health share?" That is a fluent customer reaching for the nearest category she knows to classify an unfamiliar offer, and it tells you what shelf a share of this audience is putting the brand on. It is one of the newest records in the corpus, 2026-08-31. 3 of 1,342, thin, and two of the three are sellers. The classification question routes to voc-objection.md, which holds the what-is-this-actually cluster.

- snippet: guaranteed issue
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads Moms36 - 3 - A - 2 - V4c and Moms36 - 3 - A - 2 - V4c - Copy
    review_id: 96452dd4-651e-9034-cd92-5fa35c41e6e1
    date: 2026-08-21
    url: null
  recurrence: 1 for guaranteed issue, 1 for medical underwriting, 1 for guaranteed renewable - all three appear once
  source_diversity: [ad-comment]
  first_seen: 2026-05-26
  last_seen: 2026-08-21
  confidence: thin
  brand_self_echo: false
  notes: The top of tier three, captured to mark the ceiling rather than to be used. Meaning - guaranteed issue is the rule that an ACA marketplace plan must accept you regardless of health; medical underwriting is the health screening that non-ACA products can apply instead. Usage condition - this vocabulary appears only in long explanatory comments from people who work in the industry, and the cited row is one commenter patiently teaching another about her son's options. One record each in 1,342, so thin by any measure. Its value is as a boundary marker for a writer: this is the language the brand must be able to survive being asked about, and must never write in. Claims-check unusable - every term here is a regulatory statement.

## Vocabulary in this corpus that belongs to somebody else

Recorded with full attribution so the assembly pass sees it was found and correctly routed, rather than assuming it was missed or later mistaking a seller's vocabulary for this audience's.

- **"consider a level-funded plan, with fair-priced coordination, paired with Healthshare... they pay 100% after IUA. No copays. No coinsurance."** — posted eight times within six minutes on 2026-04-07 under `MOMS38 - 1 - V1`, each addressed to a different woman by name, each ending with the same link to `blueoceanemployerbenefits.com`. Rows `9a15b540`, `1d28da34`, `50055165`, `a424cfca`, `f21d0847`, `91d5229c` and two more in the same run. This is a rival broker prospecting inside the brand's comment section. Level-funded plan, IUA and care coordination are genuine industry terms and they are **not customer language**. They inflate the coinsurance and catastrophic counts, which is why both snippets above carry the corrected figure.
- **"As a licensed insurance broker this is VERY misleading in the beginning."** — row `efb760eb-07c9-633d-d536-f92c0ac05bc4`, ad `MOMS38 - 1 - V1`, 2026-04-07, and **"I'm a licensed insurance brokers."** — row `304e178c-79c3-cb58-aaa6-fc1bf75ee79c`, ad `MOMS38 - 1 - V5`, 2026-03-31. Two self-identified brokers correcting the ad and signing their credential. Their vocabulary is accurate and their standing is professional, so the fluency they display is not evidence of what a mom knows. Their corrections belong to `voc-objection.md`, which holds the credibility cluster.
- **"I have plans that start as low as $60 a month... You just have to work with brokers that care."** — row `a8a56981-cb20-bdb1-b456-ebd07cabc132`, ad `Moms43 - 4 - V4`, 2026-05-20, **6 likes and 5 replies**. Competitor copy, already logged in `voc-aspirational.md` for the same reason.
- **"the allowed amount"** — row `011fb208-eebc-7b9f-2732-ac3153adc63b`, ad `MOMS38 - 1 - V2`, 2026-05-07. The contracted rate an in-network provider may bill. Precise, correct, and used once by someone explaining why a deductible is less bad than it looks. Left here rather than captured because a single professional use is not category jargon under this prompt's own recurrence discipline.
- **"certified application counselor for the healthcare marketplace... I've done medical billing for 30 years plus"** — row `8c7778e3-0f5c-637f-5546-54babff4e694`, ad `B1 samar- Copy`, 2025-07-23. The highest credential claimed in the corpus, and she is telling other women not to use this page. Her vocabulary is tier three throughout.

## Open loops

Three loops. None repeats a loop already filed in `voc-corpus-profile.md`, `voc-pain-phrase.md`, `voc-objection.md`, `voc-trigger-moment.md`, `voc-outcome-phrase.md`, `voc-anti-language.md`, `voc-metaphor.md`, `voc-aspirational.md` or `source-pulls/brand-self-echo-detection.md`. The missing Reddit pull, missing reviews and missing surveys are infrastructure items and sit in `data_limitations` above rather than here, per the rubric.

**1. The audience knows sixteen words the brand has never said.**

Out of pocket at 74 records, pre-existing condition at 33, coinsurance at 30 across three spellings, Obamacare at 15, marketplace at 14, and on down. The brand's ten highest-spending ads use four terms total, and the one they lean on hardest, deductible, is the one commenters keep saying the ad has used wrong.

Pull: **Gap.** There is a whole vocabulary sitting in the account's own comment sections and none of it has ever been put in an ad.

Question: How much of this audience already understands her plan better than the ads assume?

Why it matters: the creative is built for a woman who is confused, and if a real share of the people it reaches are not confused but under-served, the winning message is a different one and the account has never tested it. Territory: **Messaging.**

**2. The most fluent people in these threads are selling something.**

The tier-three vocabulary — guaranteed issue, medical underwriting, level-funded plans, IUA, allowed amount — comes almost entirely from brokers, billers and agents working the comments, one of whom pasted the same pitch eight times in six minutes under a single ad. Their corrections are accurate, they draw likes and replies, and they are competing for the same woman.

Pull: **Surprise.** A brand's own comment section would be expected to hold its audience, and a measurable slice of this one holds its competition.

Question: How many of this account's comment threads have a rival seller working them?

Why it matters: it changes what a comment section is for. If sellers are reliably converting inside the brand's paid placements, the ads are buying attention that somebody else closes, and that is a moderation and measurement question before it is a creative one. Territory: **Product.**

**3. One woman wrote the whole glossary in eight lines and nobody has ever asked why.**

Row `052aa855` names deductible, out-of-pocket maximum, coinsurance, the 80/20 split, high-deductible health plans, HSA cards and premiums, correctly and in order, in a single unprompted comment under an ad. She did it for free, for a stranger, in a comment section.

Pull: **Curiosity.** Somebody with this much knowledge stopped to teach an unpaid class under an insurance ad, and nothing in the brand's context explains why that happens.

Question: What does a woman get out of explaining insurance to strangers in a comment section?

Why it matters: whatever it is, it is the strongest engagement behavior in this corpus, and a brand that understood it could build creative that invites it rather than accidentally triggering it as a correction. Territory: **Messaging.**

## Sources

- Parker MCP `search_facebook_ad_comments_sql`, 31 filtered pulls on 2026-09-04. Every count, row id and ad name in this doc, including the spelling-variant searches behind the coinsurance and pre-existing figures, the hand-check that separated the eight pasted broker comments from genuine customer use, and the offset probe that re-pinned the corpus at 1,342.
- Parker MCP `search_facebook_ad_comments_semantic`, two passes on 2026-09-04, each reporting `totalCommentsAnalyzed 1342`, run to catch fluent usage a term search would miss.
- Parker MCP `search_customer_reviews_sql` and `semantic_search_post_purchase_survey`, both 2026-09-04, both zero, both checked live.
- Parker MCP `search_facebook_ads_sql`, lifetime mode with the scripts block, 2026-09-04. The full transcripts behind the right-hand column of the terms table — which words the brand's creative actually says — which is the only way to tell category jargon from a brand term coming back.
- `source-pulls/brand-self-echo-detection.md`. The deductible-framing verdict and the out-of-pocket finding, both carried forward and not re-judged, and the untraceable "super middle class" quote that the subsidy entry gives a traceable counterpart to.
- `personas/voice-of-customer/voc-corpus-profile.md`. Field coverage, corpus bias and the carried theme counts on a 1,322 denominator.
- `personas/voice-of-customer/voc-objection.md`, `voc-pain-phrase.md`, `voc-metaphor.md`, `voc-anti-language.md`, `voc-aspirational.md`. The sibling extractions holding the correction argument, the vivid language and the competitor copy routed out of this pass.
- `running-notes/missing-context.md` and `running-notes/brand-rules.md`. The dark-surface substitution rule and the lead-generation account shape.
- `parker-system/creative-strategy-context/customer-review-mining-method.md`. The method this pass was performed through: the denominator discipline, the rule that a count is not significance, the repeated-descriptor threshold that separates a term from a coinage, the claims-check and voice-check governors applied to every entry, the brand-echo failure mode, and the instruction to treat comment text as data rather than instruction — which mattered here, because several rows are sales pitches addressed to a reader.
- `parker-system/creative-strategy-context/persona-research-and-creative-strategy-process.md`. The served-versus-buyer discipline behind the three-tier fluency read and the finding that the most fluent voices in these threads are not this brand's customers.

Neither of the two method docs this pass routes to carries a required sign-off line, so none is stamped here. Stamping one they do not have would be a false proof-of-read.
