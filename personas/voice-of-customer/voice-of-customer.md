---
brand: health-for-moms
last_updated: 2026-09-04
sources_synced:
  - customer-reviews: 2026-09-04 — zero rows, verified live. Nothing to sync.
  - ad-comments: 2026-09-04 — 1,342 records, the whole first-party corpus, dated 2025-01-08 to 2026-09-03.
  - post-purchase-surveys: 2026-09-04 — zero responses, verified live. Nothing to sync.
  - brand-reputation: never — branch not run for this brand.
  - reddit: never — named by the team as the substitute source on 2026-09-03, still not pulled.
  - other-reviews: never — no third-party or retail review surface ingested.
  - ad-account: 2026-09-04 — Meta ad account HealthForMoms, act 484897827497337, ten highest-spend ads read at full media depth with transcripts.
snippet_count_total: 167
category_counts:
  pain_phrase: 29
  outcome_phrase: 3
  metaphor: 15
  objection: 48
  aspirational: 10
  trigger_moment: 23
  surprise_delight: 2
  category_jargon: 17
  anti_language: 20
corpus_profile:
  total_records: 1342
  denominator_note: The nine extractions did not all run on the same day. voc-corpus-profile.md, voc-objection.md and voc-pain-phrase.md pulled on 2026-09-03 against 1,322 records. voc-metaphor.md, voc-aspirational.md, voc-category-jargon.md, voc-surprise-delight.md, voc-outcome-phrase.md, voc-trigger-moment.md and voc-anti-language.md pulled on 2026-09-04 against 1,342. Every carried figure keeps the denominator it was computed on and is labelled. The assembly did not rebase anyone's count, because rebasing a percentage without re-reading the rows would be inventing precision.
  date_range: 2025-01-08 to 2026-09-03
  source_types_available: 1
  strong_confidence_possible: false
  reason: Cross-source recurrence is what earns strong under the template's own rule. This brand has one source type, so the ceiling across all 167 snippets is mixed. Nothing in this library is strong, and that is a fact about the corpus rather than about the phrases.
  identity_slugs_available: 0
  behavioral_signal_slugs_available: 0
  sku_list: none. sub-context-docs/website-and-product-audit.md establishes that this business has no SKUs, only funnel surfaces and partly visible underlying plan types, so sku_tag is null on all 167 snippets by fact rather than by omission.
  product_version_timeline: none supplied. Every snippet is era-tagged by review date alone and the era-blindness is a stated limit.
---

# Voice of Customer — Health For Moms

## How Parker uses this library

At execution time, customer-facing skills load this library. The skill picks an identity tag for the persona being targeted and an optional behavioral signal tag for the situational state that is currently active. The identity tag drives voice consistency. The behavioral signal tag drives which salient pain or trigger to mirror in this specific moment.

Confidence weighting: prefer snippets with higher recurrence and broader source diversity. Treat single-source snippets as candidates rather than canon.

Flag any snippet where brand_self_echo is true. These phrases entered customer language only after the brand introduced them in marketing. They are low signal and high risk of marketing to ourselves.

**Four things about this particular library, before anything is pulled from it.**

**One. Every identity tag and every behavioral-signal tag is null, on all 167 snippets.** `personas-profile.md` does not exist yet. The template is explicit that VoC references slugs defined there and never introduces its own, so the tags stay empty rather than invented. This is the single biggest limit on the library as it stands: the mechanism Parker is supposed to use to pull the right voice for the right audience cannot run yet. Several extractions, `voc-trigger-moment.md` most of all, wrote in each snippet's notes what the signal would be, so the tags can be attached in one editing pass the day personas land. That is open loop 4 below.

**Two. Nothing here is strong, and nothing can be.** One source type. Read `mixed` in this library as "recurs meaningfully in the only place we can see" and `thin` as "one or a few records." A `mixed` snippet here is not the same animal as a `mixed` snippet in a brand with seven live sources.

**Three. Nobody in this corpus is confirmed to have bought anything.** The account is lead generation: 39,569 leads lifetime on $743,218.09 of spend at $18.78 each, and zero purchases, because no purchase event exists. The purchase completes on a phone call handled by a partner agency that no tool can see. So this is the language of people the algorithm served, standing outside the product. It is rich on the problem side and nearly empty on the result side, and the category counts show exactly that: 29 pain phrases and 48 objections against 3 outcome phrases and 2 surprise-and-delight phrases.

**Four. Two categories are near-blanks and the blanks are findings, not gaps in the work.** Outcome phrases and surprise-and-delight are almost empty because the moment they describe happens somewhere Parker cannot look. Do not write a testimonial or a pleasant-surprise line for this brand. There is no customer voice to base one on.

## What the assembly reconciled

This section exists so a reader can see the judgment calls rather than inherit them silently. The verbatim snippets below are exactly as the nine extractions captured them. The recurrence, the confidence, the echo flag, the tags and the two governors are the assembly's reasoning over those extractions, and they are `inferred` unless a count is named, in which case the count is `verified` by whichever extraction ran it.

**The 167 snippets come from 144 distinct source records, and that gap is correct rather than duplication.** Twenty-one records appear in more than one category, generating 44 entries between them. A single comment often does two jobs — a pain phrase riding inside an objection, an image sitting inside a complaint — and the template's rule is to keep one entry per category the phrase genuinely belongs to. The extractions were disciplined about splitting the fragments.

Two records do it three times each. Row `b7aa4d37`, the most-liked record in the entire corpus at 47 likes: its first sentence, "This sounds too good to be true," is anti-language; its last, "I want the 1990's back," is a pain phrase; and the whole record is an objection. And row `aa3d6d52`, "Lucky! Mine is $11,000," the highest-engagement row in the library at 19 likes: it is the counter-bid exemplar in pain phrases, the luck-frame anchor in metaphors, and the deductible exemplar in category jargon — three lenses on six words, carrying three different recurrence counts because they measure three different families.

Every multi-category entry's notes name its siblings, so Parker never counts one record as three pieces of evidence. **The honest evidence base is 144 records out of 1,342 comments, a yield of 10.7%**, and that figure is the one to quote when someone asks how much of this corpus was usable.

**One pair of snippets turns out to be one woman, thirty-four seconds apart.** The assembly spot-checked cited row ids against the live database with a whole-thread pull, and row `f7ddf89a`, "What happens if you accidentally get pregnant while having this coverage?", captured as an objection, is a **direct reply to** row `de24f387`, "My family isn't done growing," captured as the strongest aspirational phrase in the library. Posted 2026-04-22 at 00:59:14 and 00:59:48. `verified` on 2026-09-04. Neither extraction could see this, because neither pulled the thread structure. It matters in a specific way: the aspiration and the risk question are the same person working through one problem out loud, which makes the aspirational snippet stronger evidence than a lone record and shows the shape of how this want actually surfaces — a woman states the future she is planning for, then immediately asks whether the product will punish her for it. Both entries stand; the link is recorded here rather than merged, because the wordings are genuinely different and a writer would pull them for different jobs.

**One echo verdict was changed by the assembly, and it is the only one.** `voc-objection.md` set `brand_self_echo: false` on row `c07a7826`, the "insurance that has your back" record, with a light caution in its notes. `voc-metaphor.md` set it `true`. **The assembly resolves it to `true` in both categories.** The reason is the template's own test: the phrase is the brand's, it closes five of the ten highest-spending ads, and it appears in exactly one of 1,342 comments — the one where a woman puts it in quotation marks before turning it against the brand. That is a phrase entering customer language only after the brand used it, which is the definition. The objection underneath it is entirely hers and is carried by the other pregnancy and pre-existing entries, so nothing is lost by flagging the record.

**Three echo verdicts were carried forward without re-judging, per the standing verdicts in `source-pulls/brand-self-echo-detection.md`.** The word "scam" is customer-owned, first used 2025-01-13, fourteen months before the brand's first scam ad. The deductible framing is customer-originated but 95.2% concentrated inside an 83-day window the brand's own creative opened, which is why every deductible-adjacent snippet is capped at `mixed`. And "wife of the year energy," the text hook carrying most of the last 90 days of spend, appears zero times in the corpus — re-verified live against 1,342 records on 2026-09-04, still zero.

**One snippet is flagged echo besides those.** Row `1afe1a89`, "Health care for moms but you don't qualify if your pregnant? Make that make sense," was flagged by `voc-objection.md` because it turns the brand's own tweet-overlay sentence pattern back on it. The assembly keeps that flag.

**The alliteration flag was re-run across all 167 snippets and stayed at two.** `voc-metaphor.md` set both, "health poor, house poor" and "Buyer beware." The assembly reviewed every other snippet in the library and added none, rejecting "Make that make sense" as word repetition rather than alliteration and "mind blowing" as a single compound rather than a pair. Two phonetic flags across 144 distinct records is itself a finding: this audience types dollar figures, not rhythms.

**Two counts are floors and say so on their own entries.** The deductible correction cluster and the state-exclusion cluster were derived semantically rather than by exact string match, so the true numbers are higher than recorded.

**No snippet was invented, promoted, or merged out of existence.** Where an extraction produced little, the category is left sparse.

---

## Pain phrases

What the customer says about the problem in their own words, before they have encountered the solution.

Twenty-nine snippets, the second-largest category in the library and the richest in usable language. Counts in this section were computed by `voc-pain-phrase.md` on 2026-09-03 against **1,322** records and are carried at that denominator.

The shape to hold: this audience answers a number with a number. The counter-bid family — a woman replying to the ad's $6,000 with her own larger figure — runs to **82 of 1,322, 6.2%, across 8 distinct ad names**, and 64 of the 82 name a figure above the ad's. That is the single largest behavioral pattern in the corpus.

- snippet: I want the 1990’s back.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: cost-grief
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: b7aa4d37-2243-d0fe-03e6-50c8b7d495ca
    date: 2026-03-22
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-22
  last_seen: 2026-03-22
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: One instance in 1,322, kept at mixed rather than thin because it sits inside the single most-liked record in the corpus at 47 likes and 9 replies, where roughly three quarters of records carry no likes at all. The full comment opens "This sounds too good to be true. I pay over $1,000 a month for a premium. We have to pay an $8000 deductible per family member or up to $17,000 for the entire family." Assembly note — this row also appears as an objection and as anti-language, three fragments of one comment. Count it once as evidence.

- snippet: Why we have insurance and still have a damn bill when we go to the doctor.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: paying-twice
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V8
    review_id: fd6d3fb4-3868-cc4d-1ebe-ca2e8ef40dc8
    date: 2026-04-15
    product_version: null
    url: null
  recurrence: 1 exact, roughly 20 as a family
  source_diversity: [ad-comment]
  first_seen: 2025-11-28
  last_seen: 2026-05-26
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: The tightest statement of the corpus's central pain. Exact wording appears once; the idea recurs across the paying-twice snippets and in the 45 records containing "premium" and 46 containing "afford" on a 1,322 denominator. First_seen is set for the family, from row d12d9274 on 2025-11-28, eight months before the MOMS38 creative, which is why echo is false even though the ad carries its own version in "But yet I pay for that insurance." Voice-check transformable for "damn".

- snippet: Lucky! Mine is $11,000
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: counter-bid
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: aa3d6d52-d3a5-63ad-78bb-570b4939eb59
    date: 2026-03-17
    product_version: null
    url: null
  recurrence: 82 in the counter-bid family
  source_diversity: [ad-comment]
  first_seen: 2026-03-13
  last_seen: 2026-05-24
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: The best exemplar of the counter-bid at 19 likes and 4 replies, the highest-engagement row in the library. Recurrence 82 is the string count for "mine is" against 1,322, 6.2%, all 82 read; 76 post a specific figure and 64 of those name a number above the ad's $6,000, spread across 8 ad names. Every one is dated 2026-03-13 to 2026-05-24, so this behavior is a spring 2026 event on one creative family. Assembly note — this exact row is also the anchor of the luck frame in metaphors, counted there at 11, and it is the deductible exemplar in category jargon. Three lenses, one record, three different counts because they measure three different families.

- snippet: Wow only 6? Must be nice
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: counter-bid
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 22fc32bf-dfce-3e9f-59ca-4f44df9c9493
    date: 2026-03-27
    product_version: null
    url: null
  recurrence: 3
  source_diversity: [ad-comment]
  first_seen: 2026-03-20
  last_seen: 2026-04-10
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Thin because "must be nice" appears in 3 of 1,322, under the ten-record bar. Kept because it is the sharpest short form of the counter-bid and carries 13 likes, inside the top fifteen most-agreed records. The other two are "Must be nice. I was told I would have to spend $15,000" and "Yes, 6000 must be nice. Mine is 9000." Hook candidate, not a pattern claim.

- snippet: Mine is a 20k deductible before insurance helps with anything. 6k is a dream
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: counter-bid
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: c28373d7-0028-0042-fc87-1cc7e3858509
    date: 2026-03-21
    product_version: null
    url: null
  recurrence: 82 in the counter-bid family
  source_diversity: [ad-comment]
  first_seen: 2026-03-13
  last_seen: 2026-05-24
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: 7 likes and 6 replies. "6k is a dream" is the phrase — four words that name the ad's own number as the fantasy, which is the exact inversion the brand needs to know about. Same 82-row denominator.

- snippet: 600? Try 1000+, then this ad would be more realistic. American healthcare and insurance is a scam. Americans can’t even afford to die either.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: counter-bid
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: df4332e6-35fe-5247-4cfe-78ae66601144
    date: 2025-07-28
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-07-28
  last_seen: 2025-07-28
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: off-voice
  notes: The most load-bearing single record in this category despite recurrence 1. Dated 2025-07-28, on a different ad, answering a different number — a $600 premium rather than a $6,000 deductible. That makes it proof the counter-bid is how this audience answers any number an insurance ad shows, not a quirk of one creative. Carries the corpus's strongest standalone line, "Americans can't even afford to die either." Mixed on what it establishes about era, not on its own count. Off-voice: the brand cannot say this.

- snippet: Paying a deductible plus paying for a monthly fee is such a scam
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: paying-twice
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: fc4a4b8f-e082-a311-ba58-0bc592068e09
    date: 2026-04-06
    product_version: null
    url: null
  recurrence: 1 exact, roughly 20 as a family
  source_diversity: [ad-comment]
  first_seen: 2025-11-28
  last_seen: 2026-05-26
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: The plainest naming of the paying-twice pain. Echo checked rather than assumed: "scam" appears in 45 of 1,322 and 15 of those, 33%, predate the MOMS38 launch, earliest 2025-07-28, against "deductible" at 5 of 207, 2.4%, predating. So the scam vocabulary came from the audience and the deductible framing came from the ad. Standing verdict carried from source-pulls/brand-self-echo-detection.md.

- snippet: Mine is $10,000 and pay $1,200 a month in premiums. Total. Scam.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: counter-bid
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: d635af48-3b6d-4b5e-0320-08a671f85c33
    date: 2026-04-08
    product_version: null
    url: null
  recurrence: 82 in the counter-bid family
  source_diversity: [ad-comment]
  first_seen: 2026-03-13
  last_seen: 2026-05-24
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Sits in the counter-bid and paying-twice families at once, which is the shape most of the 82 take when they run past three words. The clipped ending, "Total. Scam.", is the rhythm to keep.

- snippet: We pay $40,000 a year in premiums. Doesn’t include anything. We still pay deductible and pay for services
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: counter-bid
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: 3f89f249-7ea8-6751-8cde-95fb64c13bc7
    date: 2026-04-12
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-12
  last_seen: 2026-04-12
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: One record, a quote candidate rather than a pattern. The largest premium figure disclosed anywhere in the corpus. Specific numbers are the mining method's top qualifying signal and this is the extreme end of the range. Claims-check gated because the figure is self-reported by an anonymous commenter and cannot be verified. Useful as an outlier showing the ceiling, never as a typical customer.

- snippet: I still pay full price for everything all year until I pay $6k which has been never. They have never helped me pay for anything, but I give them thousands a year for what?
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: never-reaches-deductible
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V5
    review_id: be59e705-66a5-1215-96a0-bdd826f0f68c
    date: 2026-04-08
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-08
  last_seen: 2026-04-08
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Thin on count and high on usability, which the mining method treats as different questions. It names a pain nothing else names as clearly — she never reaches the deductible at all, so the coverage is theoretical every year. "which has been never" is the phrase. Her plan is $645 a month for her and her kid with a $15k out-of-pocket max. Assembly note — the same record's closing line, "It's a joke all around," is captured as a metaphor.

- snippet: And then it's the end of the year, and we start all over. I literally hate NYE for this reason!
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: annual-reset
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: 78af9428-b3e7-a3d2-cc23-87e43de0db3a
    date: 2026-04-04
    product_version: null
    url: null
  recurrence: 5
  source_diversity: [ad-comment]
  first_seen: 2026-03-24
  last_seen: 2026-05-13
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: 6 likes. Recurrence 5 is a classification read of the reset idea confirmed row by row, not a string count, and it is under the ten-record bar. The others are terse — "And it starts over yearly," "And it resets every year." This is the only version with a feeling attached, and tying the dread to a date on the calendar is the reason to keep it. The reset is a December and January event, so a spring-heavy corpus almost certainly undercounts it.

- snippet: This year it took 35 days to hit our 8k OOP. Next year it could take as few as 1 depending on how prescriptions hit.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: chronic-condition
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads MOMS39 - 2 - V2 and MOMS39 - 2 - V2 - Copy
    review_id: b3e776b8-a237-3d00-f3ad-8cbf4cf4f298
    date: 2026-03-31
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-31
  last_seen: 2026-03-31
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: Thin at one record and worth every line. "35 days" and "as few as 1" are the specific, odd numbers the mining method names as the top realness signal. Carries the category's own vocabulary, OOP, which is the audience showing fluency the creative does not assume. The full record names prescription costs of $2,600, $1,800 and $3,200 and a child's medication at $3,600 per fill. Gated: self-reported figures.

- snippet: my deductible is $4500 and I can’t afford it so I can’t go to the doctor.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: avoided-care
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V5
    review_id: 7fb10e8d-9947-c623-ef23-1612cfd63b5c
    date: 2026-04-10
    product_version: null
    url: null
  recurrence: 7
  source_diversity: [ad-comment]
  first_seen: 2025-11-28
  last_seen: 2026-06-28
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: The pain where the money problem becomes a health problem. Recurrence 7 is the string count for "go to the doctor" against 1,322, all read. Small, but spread across four ads and three eras from November 2025 to June 2026, which is the kind of durability this corpus can rarely show. The rest of the record is an eligibility complaint held by voc-objection.md; only the pain half is here.

- snippet: I don't want to go to the doctor because the copay alone is $65 and the doctor isn't really listening to me most of the time 😭
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: avoided-care
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: c045c882-291f-e8d6-3039-8471b635fb4c
    date: 2026-04-12
    product_version: null
    url: null
  recurrence: 7 in the avoided-care family
  source_diversity: [ad-comment]
  first_seen: 2025-11-28
  last_seen: 2026-06-28
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Kept alongside the one above because it names a second reason on top of the money — not being listened to. That is the only place in the corpus where the cost pain and the care-quality pain are said in one sentence, and it is the more human of the two. Same 7-record denominator.

- snippet: This is me. Im on moujaro for diabetes and now I can't afford it because they want me to pay $1000 a month till my deductible is met. Im lost, can't afford it now.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: medication-cost
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 6c7fc8bc-6da9-09e3-2684-a4225d319004
    date: 2026-03-30
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-30
  last_seen: 2026-03-30
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: One record, here for two words. "Im lost" is the only time in the corpus anyone names the feeling rather than the figure, and the mining method treats emotive language as a qualifying signal a number cannot supply. It opens "This is me," which is recognition the rest of the corpus almost never gives. The drug-name misspelling is preserved. Assembly note — voc-trigger-moment.md holds the same record as a trigger; the pain half and the trigger half are different halves of one sentence and both passes correctly keep it.

- snippet: Mine is $6k per person too but since it’s thru my job I don’t really have a choice
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: employer-plan
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads MOMS39 - 2 - V2 and MOMS39 - 2 - V2 - Copy
    review_id: 33936dcd-893a-25ec-3240-bd21906f0e5a
    date: 2026-03-17
    product_version: null
    url: null
  recurrence: 24 in the employer family, 82 in the counter-bid family
  source_diversity: [ad-comment]
  first_seen: 2026-03-13
  last_seen: 2026-08-16
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: The pain of having no choice, which is different from having a high number. The employer denominator of 24 is the string count for "employer" carried from voc-corpus-profile.md, confirmed across rows including one from 2026-08-16 reading "If your job offers insurance you have to pick an insurance. They make you pay for one." That August date makes this the most durable family in the category, since almost everything else went quiet after May. "I don't really have a choice" is the phrase. Assembly note — also carried as an objection.

- snippet: Insurance through employer we pay $250/week and still have copay of $50. Individual deductible is $15,000. They don’t even want to cover an MRI so I had to pay out of pocket anyway.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: employer-plan
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: 1e315434-c861-3f23-4fae-2a38acd72263
    date: 2026-03-13
    product_version: null
    url: null
  recurrence: 24 in the employer family
  source_diversity: [ad-comment]
  first_seen: 2026-03-13
  last_seen: 2026-08-16
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: The fullest version of the employer pain, stacking four costs in one sentence, which is how this audience actually experiences the bill. Note the weekly framing rather than monthly — that is her real unit of pain and no ad in the account uses it. Dated three days after the MOMS38 launch, so early in the wave rather than independent of it.

- snippet: Insurance companies LOVEEEEE to take money from people YET will do everything they can to not pay out for stuff that its suppose to cover. Nightmare and mind blowing how they play games  and give the big run around.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: claim-denial
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad OMC - C11 - 2b
    review_id: 59d80f5f-496d-7d55-08c2-1492fca4c32d
    date: 2026-03-19
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-19
  last_seen: 2026-03-19
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: Thin at one record. The only place in the corpus where the pain is named as an adversary doing something to her on purpose rather than as a number that is too big. "they play games and give the big run around" is the usable half. Sits on OMC - C11 - 2b, one of the few pain records outside the MOMS38 family. Double space before "and" is original. Assembly note — also carried as a metaphor, where the game, run-around and nightmare images are counted at one record each.

- snippet: I literally was just on the phone for hours today figuring out something eith insurance...and still no answer.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: admin-burden
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 2 - V1
    review_id: 622cb438-d58d-9f87-f722-59a7c197eccf
    date: 2026-04-04
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-04
  last_seen: 2026-04-04
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: The time cost rather than the money cost, and the corpus has almost none of it. Kept for where it sits: MOMS38 - 2 - V1 is the skit creative where one woman plays both the mom and the claims rep, the one family in the account that draws agreement instead of argument. So this is a person answering creative that named her experience rather than her bill. The typo "eith" is preserved.

- snippet: girl, we pay $2,200 a month and its a battle for them to cover anything. I have MS so I NEED to be covered for my treatments
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: chronic-condition
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: cf52967d-33bb-3f5d-ed9d-138895e40607
    date: 2026-03-23
    product_version: null
    url: null
  recurrence: 7 for "cover anything", roughly 20 for the chronic-condition family
  source_diversity: [ad-comment]
  first_seen: 2026-03-23
  last_seen: 2026-05-26
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: 4 likes. "its a battle for them to cover anything" is the phrase, and "battle" is the closest thing to a metaphor the pain language offers — one of the two highest-value signals the mining method says most passes miss. The chronic-condition family is small by count and loudest by intensity, and the persona method is explicit that volume and intensity are two rankings that must not be flattened.

- snippet: so by December just hit it...oh but its Jan. Now so it starts over...and they still never cover anything.... insurance is the biggest scam 😒
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: annual-reset
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: b74814f1-85d4-8eec-8ccb-8f62e9df0b1f
    date: 2026-03-24
    product_version: null
    url: null
  recurrence: 5 for the reset family, 45 for the scam word
  source_diversity: [ad-comment]
  first_seen: 2026-03-24
  last_seen: 2026-05-13
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: The reset pain told by someone with a medical reason to hit it every year. She pays 16,000 before anything is covered, her husband pays over 300 a week, and she is in cancer remission needing CT scans every six months. The run-on punctuation is the rhythm of the pain and should not be cleaned up in a lift. Scam echo carried as the standing customer-owned verdict.

- snippet: Don’t bother looking into it if you’re diabetic . I’ll be uninsured until I die.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: chronic-condition
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 01b5ff6d-1ea1-b12f-fe1f-136348d8c40b
    date: 2025-08-14
    product_version: null
    url: null
  recurrence: 2
  source_diversity: [ad-comment]
  first_seen: 2025-08-14
  last_seen: 2026-04-03
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: off-voice
  notes: Thin, and the reason it is here is the reason the category exists. "uninsured" appears in only 2 of 1,322 records, 0.15%, and this is one of the two. So the most quotable line about being uninsured in this corpus is also proof of how rare that state is here. The first clause is an objection to this brand's underwriting and is carried by voc-objection.md; only the second sentence is the pain, and it is the pain of the category as she expects to live it, not of this product. Off-voice: the brand cannot put "until I die" in an ad.

- snippet: There is no middle class on the marketplace unfortunately. You either pay next to nothing or almost all of it with no subsidy.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: subsidy-cliff
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 8a885e35-71be-e442-a0da-f462b6eb3e9f
    date: 2025-08-09
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-08-09
  last_seen: 2025-08-09
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: One record from 2025, thin and historical. Kept because it explains the money pain rather than reporting it, and because it names a structural gap the brand's own stated persona sits inside. Useful as era evidence: it predates the MOMS38 creative by seven months and shows the cost grief was live before this campaign lit it up. Assembly note — also the exemplar for the Marketplace jargon entry, and the closest traceable customer version of the brand's untraceable "super middle class" quote.

- snippet: I’m self employed and can’t find anything that doesn’t have at least $5k deductible
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: self-employed
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads MOMS39 - 2 - V2 and MOMS39 - 2 - V2 - Copy
    review_id: 2c7f384f-cae6-a020-456c-e5534a427218
    date: 2026-04-02
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-02
  last_seen: 2026-04-02
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: 7 likes, high for a record this quiet. The string "self employed" returns only 2 records and the other is a rival agent's pitch, so this is the only genuine instance. Kept because it is the one snippet in this category that lines up with a persona the brand has already stated, and the persona method treats corroborating a stated persona as a different and useful result from surfacing a new one.

- snippet: I pay $400 a month, my deductible is 13,000 I make 12700 in a year on disability. Cuz this makes sense.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: fixed-income
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 6510e12d-3ac0-df2d-1b6b-af541fcbb690
    date: 2026-04-08
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-08
  last_seen: 2026-04-08
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: One record holding the most arresting number relationship in the corpus: her deductible of 13,000 is larger than her annual income of 12,700. The sarcasm at the end, "Cuz this makes sense," does the emotional work. Gated for the claims-check governor before any use, since the figures are self-reported by an anonymous commenter.

- snippet: shoot im just trying to figure out on how to pay the monthly charges to get health insurance let alone the charges they dont cover with copays its annoying when im barely making it
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: household-strain
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads MOMS39 - 2 - V2 and MOMS39 - 2 - V2 - Copy
    review_id: aaefb729-af45-6ee5-6dd0-c9017487a6bc
    date: 2026-03-22
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-22
  last_seen: 2026-03-22
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: Thin at one record. "im barely making it" is the phrase, and it is the only line in the corpus that names the household's overall financial state rather than an insurance figure. The all-lowercase, unpunctuated register will not survive a lift as written, so transformable rather than in-voice.

- snippet: Except the premium for that policy costs more than my house note. Who can afford that? If you get a lower premium then your deductible is much higher and no one can afford the higher deductible so either way people are screwed. Broken system
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: cost-grief
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS33 - N3 - V2
    review_id: dc090fc7-be0b-3156-eaaa-efcdc96f62c6
    date: 2026-02-14
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-02-14
  last_seen: 2026-02-14
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: Mixed rather than thin on era value. Dated twenty-four days before the MOMS38 family launched, and one of only 5 comments in the whole corpus using "deductible" before that launch. So it is the cleanest single proof that the cost pain is the customer's own and not something the ad taught her. It carries the corpus's best comparison, "costs more than my house note," and its best two-word summary, "Broken system." The trap it describes, where a lower premium buys a higher deductible, is the exact bind the brand's offer claims to solve and the creative never names it.

- snippet: It doesn't make sense. It's never made sense.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: cost-grief
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad Moms43 - 5 - V1
    review_id: f1f160d4-9962-e98e-eece-5b9bde1234e2
    date: 2026-09-03
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-09-03
  last_seen: 2026-09-03
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: One record, the single newest in the corpus, dated the day the pulls ran. Kept for freshness rather than weight. The corpus holds only 86 comments since 2026-07-01 and most are the single word "Help" under one ad, so pain language in the current era is nearly absent. This is the live end of the bank. It sits on Moms43 - 5 - V1, not the MOMS38 family, so it is evidence that the pain persists even where the creative has stopped naming a number.

- snippet: I need insurance I don’t have to pay
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: paying-twice
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad Moms43 - 4 - V3
    review_id: 1693a793-1dcb-5945-d2e6-958e69a70fd3
    date: 2026-08-26
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-08-26
  last_seen: 2026-08-26
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: One record, thin, kept for freshness. The shortest statement of the paying-twice pain and the only one from the current era. It points at a want as well as a hurt, so a reader could route it to aspirational; it stays here because the sentence is built on the present grievance of paying, not on a future self.

---

## Outcome phrases

What the customer says after the product has worked.

**Three snippets, and none of them describes the core promise being delivered.** This is the emptiest category in the library and the blank is the finding rather than a gap in the work. `voc-outcome-phrase.md` ran seven zero-return string searches and two semantic sweeps to establish it: a relief-and-gratitude pass across the whole corpus at a 0.35 floor returned **two results in 1,342 records**, and neither was about this brand.

The reason is structural. Nobody in this corpus has bought anything, the purchase completes on a partner-agency phone call no tool can see, and a comment section under a paid ad selects against the satisfied. The honest statement is not "customers report no results." It is **"Parker has no way to observe whether customers get results, and the brand does not either."**

The cost is concrete. The four outcome phrases in the brand's own context document — "I finally understand my insurance," "My family is covered, no matter what," "I made a smart choice," "No more worrying every time my kid gets sick" — return **zero** in the customer record, re-verified live against 1,342 on 2026-09-04. The only outcome language this brand possesses is language it wrote for itself.

- snippet: Best advice I have gotten from an insurance agent! She didn’t have anything that fit but pointed me in the right direction!
  category: outcome_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: agent-consultation
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads Moms Nahuel WV#1 - V9 and Moms Nahuel WV#1 - V9 - Copy
    review_id: 45bc3e26-5d26-1d96-30c2-686ca6e5fbf8
    date: 2026-04-17
    product_version: null
    url: null
  recurrence: 1 exact, 2 for the helpful-agent family
  source_diversity: [ad-comment]
  first_seen: 2026-04-01
  last_seen: 2026-04-17
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: One of exactly two records in 1,342 reporting a good experience with this brand's own service, 0.15% of the corpus. Captured on a specific reading that should stay visible: the product is a match-and-consult referral, so the deliverable is the consultation, not a policy, and on that reading good advice from the agent is the product working. What it explicitly is not is the result the ads promise — she says outright that nothing fit. Echo false: no ad uses "pointed me in the right direction" or anything near it, checked against the ten highest-spend transcripts. 2 likes. Claims-check gated — usable only as service proof, never as proof that a plan was found. Assembly note — voc-surprise-delight.md holds this same record under the delight lens, where the exceeded-expectation reading is stronger. One record, two entries, one piece of evidence.

- snippet: I was connected to a very helpful agent. They weren't able to find a lower price for our particular situation but he was very kind and helpful and respectful.
  category: outcome_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: agent-consultation
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: df460383-699e-27a3-e2ef-e4f3197790f4
    date: 2026-04-01
    product_version: null
    url: null
  recurrence: 1 exact, 2 for the helpful-agent family
  source_diversity: [ad-comment]
  first_seen: 2026-04-01
  last_seen: 2026-04-17
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: The other of the two, stating the miss even more plainly — they could not find a lower price. Together these two are the entire public evidence base for this brand's service quality. The pattern inside them is worth naming as an inference: both women were told no and both praised the brand anyway, which suggests the consultation has standalone value even when it produces nothing to sell. Two records is a candidate, not a pattern. "kind and helpful and respectful" is the phrase. 1 like. Also held in voc-surprise-delight.md.

- snippet: I called them they spammed me and wasted hours of my time to tell me it was going to cost $400/month LOL
  SO IT DOESNT SAVE YOU $400 it literally costs just the same if not more than regular scammy health insurance.
  category: outcome_phrase
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: completed-journey
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads moms-63 3e and moms-63 3e - Copy
    review_id: 7a6c83e0-affb-e39e-aa7c-c52ff1d59739
    date: 2026-09-03
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-09-03
  last_seen: 2026-09-03
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: A realized outcome and a negative one. Captured because it is the only record in 1,342 that walks the whole journey — she saw the ad, she called, she got a real quote, she reported the number back. One record, thin, and it must never be presented as a pattern. It matters far beyond its count: it is the newest substantive record in the corpus, it names a specific figure the mining method flags as the top realness signal, and it directly contradicts the savings promise in the account's own creative. Claims-check unusable and flagged as the single highest-priority claims item in the library. Echo false — "scammy" is her own inflection of the customer-owned scam vocabulary. The observation is the asset, not the wording.

---

## Metaphors

How the customer analogizes the product, the problem, or the outcome.

Fifteen snippets, and the category is thinner than it looks because **this audience speaks in arithmetic, not images**. Eleven metaphor families that a health-insurance corpus would be expected to carry returned zero records each, including "gamble," "hostage," "rigged," "trapped," "bankrupt" and — the one that should stop a reader — **"feels like," which appears zero times in 1,342 records**. All counts here were computed on **1,342** on 2026-09-04.

Four frames carry essentially all of it: the category is a crime, the category is a joke, your coverage is luck rather than a choice, and the brand's own metaphor handed back with a knife in it.

- snippet: Insurance is the BIGGEST forced scam in the entire world
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: cost-grief
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: 3c25dae8-59c4-b8fe-5911-08d1153d6401
    date: 2026-03-30
    product_version: null
    url: null
  recurrence: 48 for the scam cluster, of which roughly 31 use it for the category rather than for this brand
  source_diversity: [ad-comment]
  first_seen: 2025-01-13
  last_seen: 2026-09-03
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: off-voice
  notes: The clearest metaphorical use of scam in the corpus, because "forced" concedes the thing is legal and mandatory in the same breath that calls it a crime. 48 of 1,342, 3.58%, across 15 distinct ad names — the widest-spread language this brand owns. 10 likes. Echo verdict carried forward and not re-judged: customer use begins 2025-01-13, fourteen months before the earliest brand ad carrying the scam hook. Off-voice as written because the brand's guidelines forbid scare tactics, but the observation is fully usable at a lower temperature.

- snippet: Health and Car insurance are the biggest legal scams that are RDQUIRED to be payed into. Nobody benefits from either except the insurance providers
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: cost-grief
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: 85ad24c4-1ffa-c22c-da1c-617049382bcf
    date: 2026-04-14
    product_version: null
    url: null
  recurrence: 1 exact, 2 for the qualified-scam wording that concedes legality
  source_diversity: [ad-comment]
  first_seen: 2026-03-30
  last_seen: 2026-04-14
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: The same image as the entry above, kept separate because the wording is more precise. "Legal scam" is the customer naming the exact shape of her grievance — not that anyone broke a law, but that the law permits this. Typo preserved. The second half, that the only party served is the seller, is a separate reusable idea the brand could speak to since it positions against big insurance.

- snippet: All insurance is a scam and robbery but a high DED and OPM  with high coinsurance rates is absolutely outrageous. You are better off being self pay and asking for selfpay pricing than using insurance.
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: exit-the-category
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: e8dab1a2-dfb3-1d0d-9026-2342a40768de
    date: 2026-04-10
    product_version: null
    url: null
  recurrence: 1 for "robbery" in the whole corpus
  source_diversity: [ad-comment]
  first_seen: 2026-04-10
  last_seen: 2026-04-10
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: The only appearance of "robbery" in 1,342 records, verified by substring search. Kept because it sits at the sharpest end of the crime frame and because the speaker is plainly fluent — she uses DED and OPM without explaining them. Double spacing preserved. Mixed rather than thin because the image it belongs to is the corpus-wide crime frame rather than a lone flourish, though the exact word appears once.

- snippet: Lol!!! Sooooo......health insurance is a racquet.
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: cost-grief
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V10
    review_id: dea2d778-1d23-a7c4-a4b1-43c79be3f9ed
    date: 2026-03-26
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-26
  last_seen: 2026-03-26
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: off-voice
  notes: Her spelling, kept exactly. The word she means is racket in the organized-crime sense, and a search for "racket" returns zero real instances — the one row it matches contains "bracket" — so this is the only mafia-flavored image in the corpus. Snippet trimmed to the metaphor; the rest describes refusing to pay medical bills and belongs to the objection and jargon passes. This is the clearest case of the identifier trap in the library: the semantic tool returns dc84e8fd for this row and the SQL comment_id is dea2d778.

- snippet: $15,000 is our deductible for the insurance we can’t afford... Insurance is a joke….
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: cost-grief
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V5
    review_id: 800d9f1a-cbb6-e7af-963c-93ee3e5eed4b
    date: 2026-03-31
    product_version: null
    url: null
  recurrence: 8 for "a joke", of which 5 aim at the category and 3 at this brand's offer
  source_diversity: [ad-comment]
  first_seen: 2025-07-23
  last_seen: 2026-08-31
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: The cleanest example of the joke frame and it shows the frame's grammar — a number first, then the verdict. Calling something a joke says it is not a serious request, a different accusation from scam: scam is angry, joke is exhausted. 4 likes. The joke cluster runs at 0.60% against the scam cluster's 3.58%. Curly apostrophes and the four-dot ellipsis preserved as stored.

- snippet: I have a $6k deductible and my out of pocket maximum is $15k 😂 my kid and I are on a plan that is $645 a month. I still pay full price for everything all year until I pay $6k which has been never. They have never helped me pay for anything, but I give them thousands a year for what? Once I pay the $6k, they pay a portion and I STILL have to pay lmao. It’s a joke all around.
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: never-reaches-deductible
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V5
    review_id: be59e705-66a5-1215-96a0-bdd826f0f68c
    date: 2026-04-08
    product_version: null
    url: null
  recurrence: 8 for "a joke", 5 in the category sense
  source_diversity: [ad-comment]
  first_seen: 2025-07-23
  last_seen: 2026-08-31
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: Kept whole because the structure is the asset — four specific numbers, a rhetorical question in the middle, and the image only at the end. "Which has been never" is the sharpest line: she has never once reached her own deductible. Assembly note — this is the one snippet in the library that comes closest to the whole-review-concept unit the mining method says belongs in a separate concept bank rather than a phrase bank. It is kept here because the lift-able fragments inside it are real, and flagged so a later concept bank can claim the whole arc. voc-pain-phrase.md holds the middle fragment.

- snippet: Lucky! Mine is $11,000
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: coverage-as-luck
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: aa3d6d52-d3a5-63ad-78bb-570b4939eb59
    date: 2026-03-17
    product_version: null
    url: null
  recurrence: 11 for the luck-and-winning frame, 9 of them using luck for someone else's coverage
  source_diversity: [ad-comment]
  first_seen: 2026-03-17
  last_seen: 2026-05-07
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Six words and the highest-engagement row in the library at 19 likes and 4 replies. The image is implied rather than spelled out, which this category explicitly allows: coverage is a hand you were dealt. Calling another woman lucky for having a $6,000 deductible reframes the entire category as chance rather than choice, which is the opposite of what the ad above it argues. The honest limit: all 11 records sit inside the MOMS38 - 1 family, so this is a source-specific pattern until something outside it corroborates. Assembly note — same row as the counter-bid exemplar in pain phrases and the deductible exemplar in jargon; the three counts measure three different families and must not be added together.

- snippet: I think I win mine is $9000
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: coverage-as-luck
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V8
    review_id: d7812c81-61d4-be87-5b79-dd0914a0ea7e
    date: 2026-03-30
    product_version: null
    url: null
  recurrence: 2 exact for "I win", 11 for the wider luck-and-winning frame
  source_diversity: [ad-comment]
  first_seen: 2026-03-30
  last_seen: 2026-04-09
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: The contest half of the frame and the more revealing half. She treats the comment thread as a competition in which the worst deductible wins, which is a real image and a strange one — the prize for winning is that your life is worse. 3 likes and 5 replies, so it did what a contest does and pulled others in to top it.

- snippet: I win, we pay $1500 a month and still have $2500 deductible 😞
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: coverage-as-luck
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V8
    review_id: 8e64382e-a644-c112-a9e4-220c94726675
    date: 2026-04-09
    product_version: null
    url: null
  recurrence: 2 exact for "I win", 11 for the wider frame
  source_diversity: [ad-comment]
  first_seen: 2026-03-30
  last_seen: 2026-04-09
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: The same contest image with the emotion left visible. "I win" and a sad face in the same eleven words is the whole frame compressed: she is claiming a victory she does not want. Captured separately from the entry above because the wording carries the tone break the other does not.

- snippet: I like how it’s "insurance that has your back" but apparently there’s no plans for someone who’s pregnant with type one diabetes. Yeah, totally has my back on the condition that I’m healthy before getting the insurance
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: pregnancy-exclusion
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: c07a7826-7f12-090e-db52-0b8ff04c4abb
    date: 2026-04-12
    product_version: null
    url: null
  recurrence: 1, and the only appearance of "your back" or "our back" in 1,342 records
  source_diversity: [ad-comment]
  first_seen: 2026-04-12
  last_seen: 2026-04-12
  confidence: thin
  brand_self_echo: true
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Echo true and the direction is not in doubt — she puts the brand's line in quotation marks before turning it. "Has your back" closes five of the ten highest-spending ads, verified from transcripts, and comes back exactly once in customer language, sarcastically, from a woman who was excluded. Captured rather than discarded because the assembly needs hostile echo visible as its own thing. 4 likes and 3 replies. Claims-check unusable and routed to the governor as a live risk on the account's most repeated line. Assembly note — this is the one echo verdict the assembly changed: voc-objection.md had it false with a caution, voc-metaphor.md had it true, and the assembly resolves to true in both categories.

- snippet: We’re health poor, house poor, vehicle poor, Walmart addicted, stuck in a rut people.
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: household-strain
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 0bb56fef-8bb4-8bf6-1cce-06a292d0bb80
    date: 2025-07-23
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-07-23
  last_seen: 2025-07-23
  confidence: thin
  brand_self_echo: false
  alliteration: true
  claims_check: clear
  voice_check: transformable
  notes: The best-written sentence in 1,342 records and one of only three alliteration flags in the library. "Health poor, house poor" is a genuine alliterative pair, and the escalating list is a customer doing copywriting in her own words — she takes an existing phrase, house poor, and extends it into a whole identity. "Stuck in a rut" is the metaphor proper. One record, so thin; its value is as a single voice, not a movement. Off-voice in part — the brand cannot call its audience Walmart addicted — but the health-poor construction is transformable and is the strongest headline candidate in the library.

- snippet: It’s not insurance, yet they pass it off as if it is. Buyer beware!
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: legitimacy-doubt
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: a69e2ffe-d4f2-cd89-49ef-b130b136cb2b
    date: 2025-07-29
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-07-29
  last_seen: 2025-07-29
  confidence: thin
  brand_self_echo: false
  alliteration: true
  claims_check: unusable
  voice_check: off-voice
  notes: Captured for the alliteration flag more than the image. "Buyer beware" is a stock phrase rather than an invented one, but the phonetic pair is real and the mining method treats alliteration as one of the two highest-priority signals most passes miss. Aimed at this brand rather than the category, so its argumentative content belongs to voc-anti-language.md and voc-objection.md; only the phrasing is captured here. Unusable as written — it is an accusation against the brand.

- snippet: Insurance companies LOVEEEEE to take money from people YET will do everything they can to not pay out for stuff that its suppose to cover. Nightmare and mind blowing how they play games  and give the big run around.
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: claim-denial
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad OMC - C11 - 2b
    review_id: 59d80f5f-496d-7d55-08c2-1492fca4c32d
    date: 2026-03-19
    product_version: null
    url: null
  recurrence: 1 each for "play games", "run around" and "nightmare" — all three appear only in this record
  source_diversity: [ad-comment]
  first_seen: 2026-03-19
  last_seen: 2026-03-19
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: Three separate images stacked in one comment, which is why it is captured whole. The game frame says the insurer is playing while she is not; the run-around says the process is designed to exhaust her; nightmare says the whole thing has the logic of a bad dream. Each returns exactly one record across 1,342 in its own search, so none is a pattern and the stack is one person being unusually vivid. Sits on a different creative family from the luck frame, which almost nothing else here does. Assembly note — "mind blowing" was reviewed for an alliteration flag and rejected as a single compound rather than a pair.

- snippet: Yep but what if you don’t have kids... Just another crack I slip through
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: eligibility-exclusion
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 0998c107-008d-4faf-2a24-995e4ad699f9
    date: 2025-07-28
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-07-28
  last_seen: 2025-07-28
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: A real metaphor and an unusually good one — she turns the stock phrase about people falling through the cracks into something she does personally and repeatedly, which is what "another" is doing in that sentence. Aimed at the qualifier that excluded her for not having children, so the exclusion complaint belongs to voc-objection.md; only the image is here. A second, unrelated use of falling through the cracks appears in a long comment about Texas school funding, which suggests the image is category-standard rather than invented here.

- snippet: makes me feel like a pile of shit
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: household-strain
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V9
    review_id: 39142f88-ca24-f10f-ebc6-e0918d2d82b4
    date: 2026-04-04
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-04
  last_seen: 2026-04-04
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: off-voice
  notes: The only simile in the corpus describing the speaker rather than the industry, and the emotional low point of 1,342 records. The speaker is a father, and 96.1% of this account's lifetime spend delivers to women, so he is off-persona — the fact that the only self-directed image in the corpus comes from the demographic the brand does not address is a finding rather than a footnote. The whole comment is worth reading in place: spinal fusion, lost the good job with good insurance, back in school, and in the meantime the one racking up medical debt for his family. Off-voice, not liftable; the observation — that being the sick one in a family reads to that person as being the burden — is an angle nothing in the account touches. Assembly note — voc-aspirational.md holds this record's other fragment.

---

## Objection phrases

Pre-purchase doubts the customer expressed in their own words.

**Forty-eight snippets, the largest category in the library by a distance.** Counts here were computed by `voc-objection.md` on 2026-09-03 against **1,322** records and are carried at that denominator. Eleven distinct clusters, ordered below by size.

One thing to hold before reading: these are *publicly performed* objections, which is not the same thing as the private hesitation that stops a purchase. A woman who quietly decided not to click leaves no record anywhere. What is here is what people were willing to say out loud under an ad, and the shape that selects for is argument, correction and warning.

### Maternity and pregnancy exclusion — 36 of 1,322, 2.7%, across 15 ad names and five creative families

- snippet: How can you have healthcare for moms if you don’t cover maternity? Makes zero sense. False advertising.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: pregnancy-exclusion
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 3b2ac139-83f3-123e-bd63-6321ff80f4d4
    date: 2025-08-12
    product_version: null
    url: null
  recurrence: 36
  source_diversity: [ad-comment]
  first_seen: 2025-07-01
  last_seen: 2026-06-09
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: 36 of 1,322, 2.7%, across 15 distinct ad names and five creative families over fourteen months. Underlying concern, inferred — this reads as a verdict on the brand's honesty rather than a coverage question, which is why the words reach for false advertising. Assembly note — voc-anti-language.md holds the last two words of this same record as the anti-language half. One record, two entries, one piece of evidence.

- snippet: Health for Moms, but only if your babies are out of the womb. I was denied for being pregnant. Scam.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: pregnancy-exclusion
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: a04168ce-2e0e-2ceb-7992-d6427575062f
    date: 2026-02-03
    product_version: null
    url: null
  recurrence: 36
  source_diversity: [ad-comment]
  first_seen: 2025-07-01
  last_seen: 2026-06-09
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: A distinct phrasing of the same doubt, kept separate because the wording is what a writer lifts. This one carries a first-hand denial rather than an inference from the form, which makes it the strongest single piece of evidence in the cluster. Unusable as a claim — the brand cannot repeat it. Usable only as the objection a script answers head on.

- snippet: One question literally asks if you are pregnant or planning to be pregnant? The answer choices are no and I’m not planning to be or yes I’m pregnant. I’m not pregnant but I’m planning to be. So I picked yes pregnant and it says there are no plans. You would think if it is advertising as a mom insurance company then pregnancy status should not matter.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: pregnancy-exclusion
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: a8f8a46c-9484-ad65-fcc5-28e9f8ebb25c
    date: 2026-02-08
    product_version: null
    url: null
  recurrence: 36
  source_diversity: [ad-comment]
  first_seen: 2025-07-01
  last_seen: 2026-06-09
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: The most precise record in the cluster. She narrates the exact qualifier screen and the exact dead end it produced. A whole-review concept candidate in the mining method's sense — the full arc, from clicking through to being turned away by a question about a future she has not lived yet, maps to a producible ad if the product ever changes. No resolution exists in the thread; the brand does not answer.

- snippet: Plans not available for those that don’t plan or can’t get pregnant anymore bc of an unexpected hysterectomy last year  - yet have kids already… (health for moms) makes sense 👍🏼
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: pregnancy-exclusion
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 7a742fa2-fc66-940e-3000-b682cf371251
    date: 2026-04-08
    product_version: null
    url: null
  recurrence: 36
  source_diversity: [ad-comment]
  first_seen: 2025-07-01
  last_seen: 2026-06-09
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: transformable
  notes: Kept because it inverts the cluster and shows the screen is wider than pregnancy — she is excluded for the opposite reason to everyone else here. Inferred: the qualifier reads reproductive status in both directions, so the objection is not really the maternity exclusion, it is that an unrelated health fact decides whether she counts as a mom to this brand.

- snippet: What happens if you accidentally get pregnant while having this coverage? do you lose this coverage? ￼
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: pregnancy-exclusion
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: f7ddf89a-3efb-2a0e-a997-acec679181a0
    date: 2026-04-22
    product_version: null
    url: null
  recurrence: 36
  source_diversity: [ad-comment]
  first_seen: 2025-07-01
  last_seen: 2026-06-09
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: The forward-looking version and the only phrasing in the cluster that is a genuine risk question rather than an accusation. Inferred: she is asking whether buying this is safe, not whether it covers her today. That is a different objection to answer and a friendlier one. No reply from the brand exists on the thread.

- snippet: Health care for moms but you don’t qualify if your pregnant? Make that make sense.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: pregnancy-exclusion
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 1afe1a89-020a-5fba-9d5d-592484d005e1
    date: 2026-05-05
    product_version: null
    url: null
  recurrence: 36
  source_diversity: [ad-comment]
  first_seen: 2025-07-01
  last_seen: 2026-06-09
  confidence: thin
  brand_self_echo: true
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Echo flag set and confidence dropped to thin deliberately. The ad MOMS39 - 2 - V2 overlays a tweet reading "My deductible is $6000... Make that make sense...." and this commenter turns the brand's own sentence pattern back on it. Per the echo rule this is brand language returning, not customer language, and it must not enter the phrase bank as a customer phrase. The objection underneath is real and is carried by the entries above. Assembly note — one of two echo-flagged snippets in the library.

### The terminology correction — 51 of 1,322 as a floor, 3.9%, across 8 ad names

This count is a floor rather than a total. It is the exact-string count for "out of pocket" or "OOP"; 207 records contain "deductible" and were not all classified.

- snippet: That’s not a deductible that’s a medical maximum out of pocket. You should educate people, not misinform!!
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: terminology-correction
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: c0a3c689-ecb4-a5a8-ae30-3176267bcc34
    date: 2026-03-29
    product_version: null
    url: null
  recurrence: 51 as a floor
  source_diversity: [ad-comment]
  first_seen: 2026-03-16
  last_seen: 2026-05-22
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Inferred: this is not a coverage doubt at all, it is a competence verdict. If the brand is wrong about the first sentence, she has no reason to trust the rest of it. 2 likes and 3 replies. Assembly note — voc-anti-language.md holds the second sentence as anti-language, because "educate people, not misinform" prescribes a posture rather than correcting a fact.

- snippet: As a licensed insurance broker this is VERY misleading in the beginning. The first half is talking about a medical maximum out of pocket. A deductible is something you pay before your insurance kicks in with co insurance.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: terminology-correction
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: efb760eb-07c9-633d-d536-f92c0ac05bc4
    date: 2026-04-07
    product_version: null
    url: null
  recurrence: 51 as a floor
  source_diversity: [ad-comment]
  first_seen: 2026-03-16
  last_seen: 2026-05-22
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Quoted to its first three sentences; the full record continues into a four-paragraph explanation of coinsurance. Sits on MOMS38 - 1 - V1, the account's highest-spend creative at $54,322.63 lifetime. The word "misleading" from a self-identified broker is the sharpest version of this doubt in the corpus. Off-voice for the brand to adopt, but the observation is exactly right. Assembly note — also carried as anti-language, and its vocabulary is the tier-three example in category jargon.

- snippet: Deductible is different than maximum out of pocket 😃 -an insurance agent
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: terminology-correction
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: b41c3c21-4571-2770-b3ae-65e929619418
    date: 2026-05-01
    product_version: null
    url: null
  recurrence: 51 as a floor
  source_diversity: [ad-comment]
  first_seen: 2026-03-16
  last_seen: 2026-05-22
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: The shortest and most quotable form of the correction, and the one that carries its own credential in the sign-off. A golden nugget by the mining method's test, though only as the line an ad answers rather than a line the brand can say.

- snippet: A deductible ≠ out of pocket max. You should consider yourself lucky if your OOP Max is $6,000. A $6,000 deductible would the the amount you pay in full BEFORE copays kick in.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: terminology-correction
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 3486a679-7242-6515-294d-89bbbf4ead71
    date: 2026-03-23
    product_version: null
    url: null
  recurrence: 51 as a floor
  source_diversity: [ad-comment]
  first_seen: 2026-03-16
  last_seen: 2026-05-22
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Distinct because it does two jobs at once. It corrects the term and it rejects the premise that $6,000 is a shocking number, which undercuts the ad's whole emotional setup. Inferred: the hook is trying to agitate with a figure a sophisticated slice of this audience reads as lucky, so the agitation lands backward on them. Assembly note — also the OOP Max exemplar in category jargon, and the "lucky" here is part of the luck frame counted in metaphors.

- snippet: Bc careful woth that Max Out of Pocket. U can have a $0 Deductible but an $8,000 Max Out of Pocket. Pay attention to the fine lines bc that's how they get u. Working with health insurance. This is kinda a sneak trick that's hidden out in the open. It's why I do not get insurance
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: terminology-correction
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 8694ba97-9d45-43ac-565c-a768450c6c43
    date: 2026-05-05
    product_version: null
    url: null
  recurrence: 51 as a floor
  source_diversity: [ad-comment]
  first_seen: 2026-03-16
  last_seen: 2026-05-22
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: The most damaging single record in the cluster and the reason it earns its own entry. It aims the correction directly at the brand's own headline offer, the zero-dollar deductible, and calls it the trick. This is the objection that turns a terminology fight into a doubt about the product being sold.

- snippet: THANK YOU  I was so annoyed that she was talking about how shit is covered in full once ded is met because unless it’s the same amount as OOPM, that’s incorrect.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: terminology-correction
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: ab8cce20-9d2e-f8e5-f305-b3fe52cd7eb1
    date: 2026-04-03
    product_version: null
    url: null
  recurrence: 51 as a floor
  source_diversity: [ad-comment]
  first_seen: 2026-03-16
  last_seen: 2026-05-22
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Kept because it is agreement with an earlier correction rather than a fresh one, which shows the correction thread compounding. Assembly note — this is one of only three records in 1,342 containing "thank you," and all three thank another commenter rather than the brand. voc-surprise-delight.md makes that the sharpest line in its section.

### Pre-existing conditions and underwriting — 42 of 1,322, 3.2%, across 17 ad names, the widest spread of any objection

- snippet: Don’t bother looking into it if you’re diabetic . I’ll be uninsured until I die.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: pre-existing-exclusion
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 01b5ff6d-1ea1-b12f-fe1f-136348d8c40b
    date: 2025-08-14
    product_version: null
    url: null
  recurrence: 42
  source_diversity: [ad-comment]
  first_seen: 2025-07-02
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: The widest-spread objection in the corpus. The second sentence is the highest-intensity line in the cluster and is a pain phrase riding inside an objection; voc-pain-phrase.md holds that half. Note the shape — she is warning other women off, not asking the brand a question, which is the most costly form an objection takes.

- snippet: It only works if you don’t have any preexisting conditions. You gotta be perfectly healthy to qualify it looks like
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: pre-existing-exclusion
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 6537b3b8-785c-62e2-6891-2b1ac3ebd571
    date: 2026-08-13
    product_version: null
    url: null
  recurrence: 42
  source_diversity: [ad-comment]
  first_seen: 2025-07-02
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: in-voice
  notes: The plainest statement of the barrier in the corpus and the most lift-ready as the doubt a script answers. 2 likes and a reply. Recent, on live creative, which matters because era tagging shows this cluster has not faded the way the AI-creative rejection did.

- snippet: Preexisting health condition of cancer disqualified me
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: pre-existing-exclusion
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 3bcd0ddf-30f5-1e4c-a318-1868b9e7055f
    date: 2026-09-02
    product_version: null
    url: null
  recurrence: 42
  source_diversity: [ad-comment]
  first_seen: 2025-07-02
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: in-voice
  notes: The newest record in this cluster, posted the day before the pulls ran. Six flat words, no anger, no audience. It is the closest thing in the corpus to a private hesitation written in public, which is why it is kept despite carrying no quotable heat.

- snippet: I like how it's "insurance that has your back" but apparently there's no plans for someone who's pregnant with type one diabetes. Yeah, totally has my back on the condition that I'm healthy before getting the insurance
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: pre-existing-exclusion
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: c07a7826-7f12-090e-db52-0b8ff04c4abb
    date: 2026-04-12
    product_version: null
    url: null
  recurrence: 42
  source_diversity: [ad-comment]
  first_seen: 2025-07-02
  last_seen: 2026-09-02
  confidence: thin
  brand_self_echo: true
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Counted once in the pregnancy cluster and quoted here because it is the record where both screens fire on one person. 4 likes and 3 replies. Assembly note — this is the one verdict the assembly changed. voc-objection.md set echo false with a caution; the assembly sets it true and drops confidence to thin, because the quoted phrase is the brand's own line, it closes five of the ten highest-spend ads, and it appears in exactly one of 1,342 comments. The objection underneath is entirely hers and is fully carried by the other entries in this cluster, so nothing is lost by the flag.

- snippet: So u mean to tell me I have to be in good health to qualify? Because they turned me down when I said I have an existing condition.  Please explain
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: pre-existing-exclusion
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 3b9c3df6-07eb-c1f4-adc8-c88e974f5563
    date: 2025-07-05
    product_version: null
    url: null
  recurrence: 42
  source_diversity: [ad-comment]
  first_seen: 2025-07-02
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: The earliest record in the cluster and the only one framed as a direct request for an answer rather than a warning to peers. "Please explain" went unanswered on the thread. Inferred: the objection hardens into warning language over the following months precisely because nobody answers it at this stage.

- snippet: And they’re holding pre-existing conditions against you, which is illegal. Their system automatically bounced me out. Since I’m a certified application counselor for the healthcare marketplace I know these things I’ve done medical billing for 30 years plus. I wouldn’t waste my time on this page.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: pre-existing-exclusion
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 8c7778e3-0f5c-637f-5546-54babff4e694
    date: 2025-07-23
    product_version: null
    url: null
  recurrence: 42
  source_diversity: [ad-comment]
  first_seen: 2025-07-02
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Carried as customer language, not endorsed. The legal claim is the commenter's, marked stated and not verified, and it is a question for the brand and its counsel rather than for this library. Kept because it is the version that carries a credential and tells other readers to leave, which makes it the most costly single phrasing in the cluster. Her vocabulary is the tier-three ceiling in category jargon.

### Silent rejection — 11 of 1,322, 0.8%, across 7 ad names over eleven months

Not on the brand's stated objection list and not surfaced as its own cluster upstream.

- snippet: Well, this mom did not qualify and it didn’t tell me why.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: silent-rejection
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 74fca251-35b8-f2ea-3eac-104d73d47476
    date: 2025-08-03
    product_version: null
    url: null
  recurrence: 11
  source_diversity: [ad-comment]
  first_seen: 2025-07-28
  last_seen: 2026-06-03
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: Inferred: the doubt is not about eligibility, it is about being left without an answer, which is what turns a screened-out visitor into someone who posts about it. No resolution exists on the thread.

- snippet: So me and my kids still dont qualify thats stupid thought yall were supposed to help moms but I guess not thanks for another time waster
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: silent-rejection
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: be1f0c49-c3f3-65da-6203-60f13c71ef54
    date: 2025-08-03
    product_version: null
    url: null
  recurrence: 11
  source_diversity: [ad-comment]
  first_seen: 2025-07-28
  last_seen: 2026-06-03
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: "another time waster" is the closest thing in the corpus to the brand's stated "I don't have time" objection, and note where it appears — after the form, not before it. Inferred: the time objection for this brand is not a reason to skip the funnel, it is a verdict on the funnel after she has already spent the time.

- snippet: Who do you actually help because I’m a single mom but every time I try to get a quote it tells me you have no plan for me? So what are the qualifications m? Making over $30,000 or needing to have preexisting things? Not sure while I fall short at.. 🤷🏻‍♀️
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: silent-rejection
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 890aae1e-37cf-d43e-2057-a4730d81221f
    date: 2026-05-10
    product_version: null
    url: null
  recurrence: 11
  source_diversity: [ad-comment]
  first_seen: 2025-07-28
  last_seen: 2026-06-03
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: The fullest statement of the doubt in the corpus, and it names repeat attempts rather than one. "Who do you actually help" is the underlying question beneath every entry in this cluster, stated outright by the commenter rather than inferred. A golden nugget as the objection a script answers.

- snippet: So I don’t qualify with the 4 questions they asked! WTF! This is a joke!
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: silent-rejection
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: e06f2bcc-c1df-fb43-5146-404586cf9bf1
    date: 2025-08-07
    product_version: null
    url: null
  recurrence: 11
  source_diversity: [ad-comment]
  first_seen: 2025-07-28
  last_seen: 2026-06-03
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Distinct because it counts the questions. Four questions and a rejection is the specific detail that makes the record replayable, and specificity of that kind is a qualifying signal under the mining method. Assembly note — one of the three "a joke" records aimed at the brand's offer rather than the category, so it is not part of the joke metaphor frame.

### The call flood — 17 of 1,322, 1.3%, across 10 ad names

Strictly a post-form service complaint rather than a pre-purchase doubt, kept in the objection set because it is the source the 2026 fear entries are quoting.

- snippet: Filled it out and have been getting calls everyday from all sorts of companies which are mostly India based.  Also, the harassment from whomever keeps calling me about Medicare (India again).  This is the ONLY form I've filled out since getting my new phone number 3 months ago so it came from this site!
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: call-flood
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 3e6adba4-f376-7605-39dc-2dba27b2a2a5
    date: 2026-03-16
    product_version: null
    url: null
  recurrence: 17
  source_diversity: [ad-comment]
  first_seen: 2025-08-13
  last_seen: 2026-05-17
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: 33 likes, the third-most-liked record in 1,322, where roughly three quarters carry no likes at all, so the agreement is the signal rather than the count. The new-phone-number detail is what makes it credible to other readers. This is the record that most directly contradicts the brand context document's claimed customer phrase "Nobody pressured me — they just showed me my options."

- snippet: How many calls will I get if I try to see how this works?
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: call-flood
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 3707bfa1-c0bd-2629-63b4-6987e500f611
    date: 2026-05-17
    product_version: null
    url: null
  recurrence: 17
  source_diversity: [ad-comment]
  first_seen: 2025-08-13
  last_seen: 2026-05-17
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: 17 likes and a reply. The purest pre-click form of the objection in the corpus and the single best line in this category for a writer, because it is short, spoken, and asks the exact question a script can answer with a number. A golden nugget, and clear on the claims-check only if the brand can actually state the number.

- snippet: I filled this out because it literally says we won't be contacted by random agents. That's a lie. I immediately received 5 text messages from 5 different agents claiming to be from 5 different companies.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: call-flood
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 8604c6b5-e71e-48d6-70fc-f849f514c914
    date: 2025-11-28
    product_version: null
    url: null
  recurrence: 17
  source_diversity: [ad-comment]
  first_seen: 2025-08-13
  last_seen: 2026-05-17
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Echo left false, and worth a note: she is quoting the brand's own promise back at it, which is the reverse of a brand echo — the reassurance became the evidence against it. Inferred: promising no contact from random agents is currently generating the objection rather than answering it, which is a claims-check problem in the funnel copy, not in the ads. Assembly note — also carried as anti-language, where it is the highest-stakes entry in that category.

- snippet: I don’t wanna put my information and get called by hundreds of people though..
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: call-flood
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: a90f4907-4814-82da-e141-d85c223b181f
    date: 2026-03-11
    product_version: null
    url: null
  recurrence: 17
  source_diversity: [ad-comment]
  first_seen: 2025-08-13
  last_seen: 2026-05-17
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: 2 likes. The plain-spoken 2026 fear version, from someone who has not filled anything out. This is the objection sitting closest to the click and the exact wording a hook can answer. In-voice and liftable as written.

- snippet: Absolutely do not give them your info. You will receive calls and texts nonstop from an insane amount of reps.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: call-flood
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 7af3b3e3-998b-1c9f-f978-43bc96334e0a
    date: 2025-09-17
    product_version: null
    url: null
  recurrence: 17
  source_diversity: [ad-comment]
  first_seen: 2025-08-13
  last_seen: 2026-05-17
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: 6 likes and a reply. The warning form, aimed at other viewers rather than at the brand, which is the most costly shape this objection takes because it does the discouraging work under live paid creative. Two more near-identical warnings sit on the same ad within hours.

- snippet: If only you didnt send out info to 100 companies so moms werent getting bombarded with calls. Just give quotes online
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: call-flood
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 8c5ec2e3-3230-ef04-4d1c-60d721726634
    date: 2026-02-08
    product_version: null
    url: null
  recurrence: 17
  source_diversity: [ad-comment]
  first_seen: 2025-08-13
  last_seen: 2026-05-17
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: transformable
  notes: Kept separate because it carries the objection and the fix in one line. It bridges into the friction cluster below, where the doubt is about the form itself rather than what happens after it. The two are related and should not be merged: one fears the calls, the other resents the gate.

### Form friction and the phone call — 6 and 3 of 1,322

- snippet: Just give some pricing without making people sign up 🙄
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: form-friction
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 780a583d-3016-d6e2-bc0f-2c74428396e5
    date: 2026-03-15
    product_version: null
    url: null
  recurrence: 6
  source_diversity: [ad-comment]
  first_seen: 2025-07-07
  last_seen: 2026-03-15
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: 3 likes. 6 of 1,322, 0.5%, across 6 distinct ad names, below the ten-record threshold so thin by rule. Not on the brand's stated objection list. Short, spoken and liftable, which is why it is captured despite the thinness.

- snippet: Why can't you give a quote without my email!
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: form-friction
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 8053eec5-803f-436f-740c-1115dfa23232
    date: 2025-08-12
    product_version: null
    url: null
  recurrence: 6
  source_diversity: [ad-comment]
  first_seen: 2025-07-07
  last_seen: 2026-03-15
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: The earliest form of the same doubt, ten months before the entry above, which is what makes the pair worth carrying despite the low count. Persistent rather than recent.

- snippet: Id be way more interested if I didn't have to talk on the phone immediately tbh. It's super difficult for me to process information without reading and I get so flustered on the phone
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: phone-aversion
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 26f24c05-00d0-6bda-e4e7-10ae9ddd0617
    date: 2025-02-15
    product_version: null
    url: null
  recurrence: 3
  source_diversity: [ad-comment]
  first_seen: 2025-02-15
  last_seen: 2026-03-10
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: A related but genuinely separate doubt, so it carries its own count of 3 rather than the cluster's 6. Three records across three ads name the phone call itself as the barrier, not the number of calls. The closest match in the corpus to the brand's stated "I don't want to get on a call and be sold to," and the only one of the three that explains why, which makes it the most useful. Opens with what would fix it, which is rare in this corpus.

### State eligibility — 15 of 1,322 as a floor, 1.1%, across 5 ad names

Derived semantically across two thresholds rather than by exact string count, so the true number is higher.

- snippet: I didn't see my state... So why am I getting this ad?
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: state-exclusion
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: aac32b22-a132-0510-6269-9ca7e8dc6cdd
    date: 2026-04-07
    product_version: null
    url: null
  recurrence: 15 as a floor
  source_diversity: [ad-comment]
  first_seen: 2026-03-13
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: The clearest form of the doubt: the objection is to being served the ad, not to the state list itself. That makes it a targeting finding as much as a copy one.

- snippet: Why is this being shown in IL if it’s not on the list???😭🤦🏼‍♀️
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: state-exclusion
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 713721dc-21b1-d455-1fdd-ca76dc7ed44e
    date: 2026-09-02
    product_version: null
    url: null
  recurrence: 15 as a floor
  source_diversity: [ad-comment]
  first_seen: 2026-03-13
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Posted the day before the pulls ran, on the newest creative in the corpus, which is what makes it worth its own entry. The objection is current, not historical. Era: live.

- snippet: Ha… “in these states” proceeds to list all 50 states… scam
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: state-exclusion
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: ac7bbaaf-2fd0-fd96-43a1-57a6a6551ca4
    date: 2026-03-26
    product_version: null
    url: null
  recurrence: 15 as a floor
  source_diversity: [ad-comment]
  first_seen: 2026-03-13
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Distinct because it converts the state device into a legitimacy objection rather than an eligibility one. Inferred: the creative device meant to compel a click reads to part of the audience as a tell that the exclusivity is fake, which is a straight line from this cluster into the legitimacy one. Assembly note — voc-anti-language.md holds the same record for the false-scarcity technique rather than the coverage map.

### Legitimacy — 45 of 1,322 for the scam word, 6 for the direct question

- snippet: This sounds too good to be true. I pay over $1,000 a month for a premium. We have to pay an $8000 deductible per family member or up to $17,000 for the entire family. It’s insane. I have 2 members of the family with chronic diseases. This absolutely insane. I want the 1990’s back.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: legitimacy-doubt
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: b7aa4d37-2243-d0fe-03e6-50c8b7d495ca
    date: 2026-03-22
    product_version: null
    url: null
  recurrence: 45 for the scam word
  source_diversity: [ad-comment]
  first_seen: 2025-01-13
  last_seen: 2026-09-01
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: transformable
  notes: 47 likes and 9 replies, the most-liked record in the entire corpus. Only the first sentence is the objection; the rest is a pain phrase held by voc-pain-phrase.md and the opening line is anti-language held by voc-anti-language.md. Assembly note — this single record generates three entries across three categories. Count it once as evidence, and note the scam count of 45 was computed on 1,322 while voc-metaphor.md re-ran it live at 48 on 1,342.

- snippet: Anyone actually have this and have insight?
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: legitimacy-doubt
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 7d74447b-bc85-97f5-c3ec-39d711ff885b
    date: 2026-03-20
    product_version: null
    url: null
  recurrence: 6 for the direct legitimacy question
  source_diversity: [ad-comment]
  first_seen: 2025-07-24
  last_seen: 2026-05-15
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: 15 likes and 6 replies, and its own count of 6 separate from the 45 scam records. The politest and highest-agreement form of the doubt: she is not accusing, she is asking the crowd for proof. Inferred: with zero reviews, zero surveys and only two positive service reports in the whole corpus, there is nothing anywhere for her to find, which is a supply problem rather than a copy problem. Assembly note — this is the objection the outcome and surprise-delight blanks explain.

- snippet: A Google search doesn't pull anything about this. Is it legit?
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: legitimacy-doubt
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 1dd3618f-3693-cd9e-93e7-d3adba4a8118
    date: 2025-07-24
    product_version: null
    url: null
  recurrence: 6
  source_diversity: [ad-comment]
  first_seen: 2025-07-24
  last_seen: 2026-05-15
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: 1 like and a reply. The most actionable legitimacy record in the corpus because it names the exact check she ran and the exact result. This is the brand's own stated "is this legit" objection, confirmed in the record and given a specific cause.

- snippet: Ok. What if you or your children have a preexisting condition? Is it guaranteed renewable? Whats the catch, because I guarantee there is one.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: legitimacy-doubt
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 5db97499-85e1-b2d1-619f-8e89522382d5
    date: 2026-05-26
    product_version: null
    url: null
  recurrence: 6
  source_diversity: [ad-comment]
  first_seen: 2025-07-24
  last_seen: 2026-05-15
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: 3 likes and 3 replies. Quoted to its first four sentences; the full record continues into her cost history and a preference for the marketplace. She stacks three objections into one comment. "Whats the catch, because I guarantee there is one" uses the term "guaranteed renewable" correctly, more evidence of how fluent this audience is. Assembly note — also the Obamacare exemplar in category jargon.

- snippet: click bait sends you to the same sales team for private quotes 🙄
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: legitimacy-doubt
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: ae4f05db-ea31-1f07-3d17-db49d4dfa1cf
    date: 2025-07-07
    product_version: null
    url: null
  recurrence: 6
  source_diversity: [ad-comment]
  first_seen: 2025-07-24
  last_seen: 2026-05-15
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: A single record and therefore a candidate rather than a pattern. Kept because it names the specific mechanism the doubt rests on — that the ad and the funnel lead to the same generic sales team — which no other record states this plainly. Assembly note — also carried as anti-language, where the two extractions record different ad names for the same row; voc-anti-language.md has it on 14TH JUNE - Copy9.

### Who counts as a mom — roughly 7 of 1,322 across 5 ad names, count data-limited

No reliable string isolates this objection, so the count is a classification read rather than a string count.

- snippet: What if your kids are over 18, do I still qualify as a Mom?
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: mom-definition
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 0bf2b362-2726-f4a9-ebc0-3b5017d1037c
    date: 2026-04-29
    product_version: null
    url: null
  recurrence: 7, data-limited
  source_diversity: [ad-comment]
  first_seen: 2025-01-08
  last_seen: 2026-07-22
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: Inferred: this is not a coverage doubt at all, it is a permission question. She is asking whether she is allowed to want this, which is a completely different thing for copy to answer than a price or a trust objection. Assembly note — this cluster is the evidence behind open loop 3 in voc-aspirational.md, which reads the whole eligibility conversation as an argument about belonging.

- snippet: Why do you have to be a mother to qualify?
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: mom-definition
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 893d8ee3-88a0-3fc6-45f4-381245a04be9
    date: 2026-03-26
    product_version: null
    url: null
  recurrence: 7, data-limited
  source_diversity: [ad-comment]
  first_seen: 2025-01-08
  last_seen: 2026-07-22
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: The version that questions the rule itself rather than her fit inside it. Worth carrying into persona work: 284 of 1,322 records, 21.5%, contain "insurance" while at most 73, 5.5%, contain "mom" — and that 5.5% is inflated because the string also matches "moment." The audience is talking about the category far more than about the identity the brand named itself after.

- snippet: Do you have to be a SHM or do working moms qualify also?
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: mom-definition
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: efbfc74f-dde7-9346-8830-e6840c5ff3a1
    date: 2026-07-22
    product_version: null
    url: null
  recurrence: 7, data-limited
  source_diversity: [ad-comment]
  first_seen: 2025-01-08
  last_seen: 2026-07-22
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: Uses the insider shorthand SHM for stay-at-home mom without expanding it, which is category jargon in its own right. The most recent record in this cluster, so the confusion is current rather than solved.

- snippet: Only for moms? Lol
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: mom-definition
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 81b9eb5f-aa87-be8c-8e56-a941e5be5f71
    date: 2025-01-08
    product_version: null
    url: null
  recurrence: 7, data-limited
  source_diversity: [ad-comment]
  first_seen: 2025-01-08
  last_seen: 2026-07-22
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: The single oldest record in the entire corpus, and it is this objection. Thin on its own as four words with no reasoning attached. Kept for the era point: the very first thing anyone said under this brand's advertising was a question about who the word "mom" lets in.

### The income floor — 4 of 1,322, 0.3%, across 4 ad names

On no stated objection list anywhere.

- snippet: But if you make under 30k a year you don’t qualify smh
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: income-floor
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 45b22fb4-ca7c-f1bb-b935-21e946bcae2c
    date: 2026-09-01
    product_version: null
    url: null
  recurrence: 4
  source_diversity: [ad-comment]
  first_seen: 2025-08-03
  last_seen: 2026-09-01
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: Thin by the ten-record rule and flagged as a candidate. Posted two days before the pulls ran, so it is live. Claims-check gated: the income floor itself is unverified by Parker and only the brand can confirm it.

- snippet: I make less than 30,000 bc I'm a student in school and don't qualify for this.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: income-floor
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: b9341ab7-c197-b4d6-b7da-4cbf57a08d81
    date: 2026-05-28
    product_version: null
    url: null
  recurrence: 4
  source_diversity: [ad-comment]
  first_seen: 2025-08-03
  last_seen: 2026-09-01
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: Independent corroboration of the same floor at the same number, three months earlier and on a different ad. Two records naming the identical threshold is what lifts this from noise to a candidate worth the brand's answer.

- snippet: I don't have any pre-existing conditions, so I don't think that was it. Probably more likely that they don't cover in my area. Or my income doesn't fall into the sweet spot. I don't make very much, just more than medicaid allows (which is far below poverty level).
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: income-floor
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 057b1714-d666-2d73-a6c5-3a480d672d3f
    date: 2025-08-03
    product_version: null
    url: null
  recurrence: 4
  source_diversity: [ad-comment]
  first_seen: 2025-08-03
  last_seen: 2026-09-01
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: The earliest record and the one that shows the doubt and the silent rejection working together: she is guessing at why she was turned down because nothing told her. "Sweet spot" is her own phrase for the income band and was surfaced as a category-jargon candidate; the assembly left it out of that category because a single coinage is not in-group vocabulary.

### No standing to shop — 5 of 1,322, 0.4%, across 3 ad names

- snippet: Tamara Paige nope.  My job picks the plan that they offer.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: employer-plan
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 0f3700de-8f66-22bf-5b20-88e3477ab128
    date: 2026-03-30
    product_version: null
    url: null
  recurrence: 5
  source_diversity: [ad-comment]
  first_seen: 2026-03-17
  last_seen: 2026-08-09
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: 1 like. Inferred: this is not a doubt about the plan, it is a belief that she has no standing to shop at all. A resolution exists in the corpus but not from the brand — another commenter explains on 2026-05-05 that employer coverage can be declined. That makes this an objection with a known answer nobody is giving.

- snippet: Mine is $6k per person too but since it’s thru my job I don’t really have a choice
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: employer-plan
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 33936dcd-893a-25ec-3240-bd21906f0e5a
    date: 2026-03-17
    product_version: null
    url: null
  recurrence: 5
  source_diversity: [ad-comment]
  first_seen: 2026-03-17
  last_seen: 2026-08-09
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: "I don't really have a choice" is the clean statement of the barrier and is in-voice and liftable. She is agreeing with the ad's pain and declining its premise in the same sentence, which is the shape of this whole objection. Assembly note — also carried as a pain phrase, where the employer family is counted at 24.

---

## Aspirational phrases

Statements about who the customer wants to become, or what they want their life to look like.

**Ten snippets, and only four name a personal future self.** Counts computed on **1,342** on 2026-09-04. The other six ask for the whole category to be replaced.

The finding underneath this category is worth carrying into every creative decision: **ask this audience what she wants and she asks you whether she is allowed in.** A semantic sweep for desired-future language returned mostly eligibility questions — "What if you're not a mom?", "Why do you have to be a mom???", "Markets to moms. Provides zero plans for moms. 🚩" at 15 likes. And the brand's own aspirational identity, "wife of the year," appears **zero times in 1,342 records**, re-verified live.

### The system-level wish — 6 records, the loudest and least serviceable

- snippet: This is why we need universal healthcare.
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: system-replacement
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: bb851402-3cbc-6d0e-7497-bb9f6c2cc3de
    date: 2026-04-26
    product_version: null
    url: null
  recurrence: 6 for the system-replacement wish — 5 for "universal healthcare" and 1 for "socialized healthcare"
  source_diversity: [ad-comment]
  first_seen: 2025-07-23
  last_seen: 2026-04-26
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: The most-liked aspirational statement in the corpus at 7 likes, and the most repeated. 0.45% across 5 distinct ads spanning fourteen months, which makes it the only aspiration here that survives the corpus time skew. Captured as aspirational rather than routed to objection because it is a positive statement of a wanted future rather than a complaint about the present. It is also the aspiration this brand can least serve, and that is the point of capturing it — a writer needs to see it so they do not accidentally write toward it. Strategic value only, never liftable.

- snippet: We need to get rid of insurance companies and invest in single payer, universal healthcare. We don't need more "more compassionate" insurance companies.
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: system-replacement
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad OMC - C11 - 2b
    review_id: 5b252400-94b4-fe51-ee63-495a40cd0dba
    date: 2026-03-12
    product_version: null
    url: null
  recurrence: 1 exact, 6 for the system-replacement wish
  source_diversity: [ad-comment]
  first_seen: 2026-03-12
  last_seen: 2026-03-12
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: The sharpest record in this category, kept whole because the second sentence is the finding. She names this brand's exact positioning — a kinder insurance company for a group nobody serves well — and rejects the category rather than the product. Her scare quotes around "more compassionate" are hers. This is the clearest evidence in the library that a segment of the served audience is not shoppable at any price or with any message, which is a targeting question rather than a copy question. Routes to the persona and messaging work, not to a writer.

- snippet: we should all just have socialized healthcare.
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: system-replacement
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 0bb56fef-8bb4-8bf6-1cce-06a292d0bb80
    date: 2025-07-23
    product_version: null
    url: null
  recurrence: 1 exact, 6 for the system-replacement wish
  source_diversity: [ad-comment]
  first_seen: 2025-07-23
  last_seen: 2026-04-26
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: The earliest system wish in the corpus and the anchor for the family's first_seen date, which is what shows the wish is not an artifact of the spring 2026 comment surge. Snippet trimmed to the aspiration. Assembly note — the rest of this record holds the best-written sentence in the corpus and is captured in metaphors, alliteration flag set.

### The normative wish — how the category ought to work, 3 of the 5 "shouldn" records

- snippet: Health insurance shouldnt cost you a fortune. PERIOD.
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: affordability
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads MOMS39 - 2 - V2 and MOMS39 - 2 - V2 - Copy
    review_id: f566d1d8-95e5-71bd-d0f9-8f0c540f87fc
    date: 2026-04-28
    product_version: null
    url: null
  recurrence: 5 for the "houldn" family, 3 of them stating a wanted state of affairs
  source_diversity: [ad-comment]
  first_seen: 2026-03-22
  last_seen: 2026-05-04
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: The judgment call in this category, made in the open. It is a normative statement about the category rather than a personal future self, and the prompt is clear the absence of a pain is not on its own an aspiration. Captured because it states a wanted state of affairs in the positive and unprompted, which is the test this category runs. Read it as category-level, never identity-level. The all-caps PERIOD and missing apostrophe are hers. This is the closest thing in the corpus to a phrase the brand could adopt directly, which is exactly why the echo flag needs watching on the next run: if the brand starts saying it, later customer uses stop being evidence.

- snippet: I think if we pay for health insurance, we shouldn’t have a deductible
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: affordability
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: 724f34e4-47df-48c7-51ba-dba35561db5f
    date: 2026-03-22
    product_version: null
    url: null
  recurrence: 5 for the "houldn" family, 3 stating a wanted state of affairs
  source_diversity: [ad-comment]
  first_seen: 2026-03-22
  last_seen: 2026-05-04
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: The earliest of the three normative wants and the one that lands nearest the product, since a zero-dollar deductible is precisely what the brand sells. That proximity is a risk rather than a win. The deductible framing is settled as 95.2% concentrated inside an 83-day window the brand's creative opened, so a want expressed in the brand's own vocabulary, in a window the brand created, is weak evidence of an organic aspiration. Echo false because the construction is hers and appears in no ad transcript, but that concentration is why this is mixed and not stronger.

### The personal future self — four records in 1,342

- snippet: Why can’t you get this if you want another kid? I don’t know when I’m gonna have another kid, but I do know I want another kid. My family isn’t done growing.
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: growing-family
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: de24f387-6146-3d93-36f7-ce3df523a9fb
    date: 2026-04-22
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-22
  last_seen: 2026-04-22
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: The best aspirational phrase in 1,342 records and worth the whole pass on its own. "My family isn't done growing" names a future life in five words, and it does it while she is being told she does not qualify — the aspiration and the rejection in the same breath. One record, thin, never a pattern. The exclusion complaint around it belongs to the pregnancy cluster in objections; only the want is here. Strongest headline candidate in this category. A trailing object-replacement character in the stored row was dropped from the snippet; nothing else changed.

- snippet: You know it would be great to be able to travel and not have to worry about only being in your hometown to be able to go to the doctor if there’s an emergency or you’re visiting for a long period of time at least be able to go to the urgent cares
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: coverage-portability
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads Moms Nahuel WV#1 - V9 and Moms Nahuel WV#1 - V9 - Copy
    review_id: 7d41203a-6335-bf85-93fa-c7fadc338e92
    date: 2026-04-15
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-15
  last_seen: 2026-04-15
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: transformable
  notes: The only record in the corpus describing a wanted day rather than a wanted number, and it carries 3 likes. The want is freedom of movement — being able to leave your town without leaving your coverage behind. The brand's top-spending script promises exactly this, "nationwide coverage that truly protects your family" and "the freedom to choose your own doctors, specialist without restrictions," verified from the B1 samar- Copy transcript. Echo false all the same: she states the want in her own words with no phrase overlap, and the network-restriction complaint is a well-worn category grievance. Gated — nationwide access is a specific product claim.

- snippet: I just want insurance for me and one child without having to pay for a whole family plan.
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: household-size
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad Moms36 - 3 - A - 2 - V4a
    review_id: 270c3096-0d86-0259-bf00-6d48b423e338
    date: 2026-06-01
    product_version: null
    url: null
  recurrence: 1 exact, 2 for the "I just want" string of which only this one is a want
  source_diversity: [ad-comment]
  first_seen: 2026-06-01
  last_seen: 2026-06-01
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: A small, precise want and the most actionable one here, because it names a product shape rather than a feeling: a household of two, priced as two. It sits on a different creative family from most of this library, which is worth noting in a corpus this ad-skewed. The underlying idea recurs in different words — "What if I'm a mom, but my son is in college," "What about moms with adult children" — but those are eligibility questions held by objections, so recurrence is recorded as 1 for the want as stated.

- snippet: I’m currently in school now so that one day I can have a good paying job with good insurance again
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: job-change
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V9
    review_id: 39142f88-ca24-f10f-ebc6-e0918d2d82b4
    date: 2026-04-04
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-04
  last_seen: 2026-04-04
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: The only record naming a future self reached by a plan the speaker is already executing — back in school, aiming at a job that carries insurance. "Again" is the load-bearing word: this is a want to return to something lost, not to reach something new. The speaker is a father, and 96.1% of lifetime spend delivers to women, so he is off-persona. That the corpus's clearest statement of an aspiration reached through effort comes from the demographic the brand does not address is recorded rather than smoothed over. Assembly note — the same record supplies the only self-directed simile in metaphors.

### The aspiration pointed at someone else

- snippet: I wish I had the money to make a for dad’s or men only insurance company! My ex-husband worked hard until his body broke! Why doesn’t he get help?
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: advocacy-for-others
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 54d534aa-6273-934b-7ce2-35dcb21892f0
    date: 2026-03-30
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-30
  last_seen: 2026-03-30
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: off-voice
  notes: An aspiration pointed at someone else, which is why it is unusual enough to capture. She is not naming a self she wants to become; she is naming a thing she wishes existed for her ex-husband, and the emotional detail — worked hard until his body broke, split because he became too mean, still not happy about his options — makes it one of the most human records in 1,342. Its strategic value is a lens the account has never used: this brand's audience contains women advocating for men. Snippet trimmed to the want and its reason.

---

## Trigger moments

What was happening in the customer's life at the moment they decided to buy.

**Twenty-three snippets.** Counts computed on **1,342** on 2026-09-04.

Two limits govern the whole category and neither should be smoothed over. **The behavioral-signal tag is null on all 23**, which is the field this prompt says is load-bearing here and should rarely be empty. `personas-profile.md` does not exist, and this library never invents a slug, so every snippet names in its notes what the signal would be and the tags can be attached in one editing pass once personas land. And **not one commenter here is confirmed to have bought anything**, so strictly these are moments that pushed people to comment, not moments that pushed people to buy. The whole category is read down one notch for that.

The shape worth holding: the things that actually change a woman's coverage in this corpus are a job, a state move, a marriage, an employer, or a diagnosis. Almost never a decision she made after seeing an ad.

- snippet: This is what I'm afraid of. Just found out I desperately need a hysterectomy. My husband is looking into insurance for me so that I can get it done. They told him we don't have to meet the deductible which is $7500 but that's hard to believe. I'm worried that when I finally get the surgery scheduled  that I'm gonna have to come up with thousand before it can be done. I don't have that kind of money laying around.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: scheduled-procedure
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: 1f6f1f3e-b0ed-117f-6b73-2cc3090e019e
    date: 2026-04-14
    product_version: null
    url: null
  recurrence: 2 for the exact "just found out" opening, 6 for the scheduled-medical-event shape
  source_diversity: [ad-comment]
  first_seen: 2026-04-10
  last_seen: 2026-05-04
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: The single richest trigger moment in 1,342 records and the one to build a brief on first. It carries a diagnosis just received, a procedure not yet scheduled, a husband already shopping on her behalf, and the exact fear that stops the purchase, all in one comment. Signal would be a newly diagnosed condition forcing a coverage decision. A candidate rather than a pattern by the ten-record bar. Note the buying is being done by her husband, which lines up with the separate finding that the woman in this audience is often the household's insurance shopper and sometimes is not. Double space before "that I'm gonna" is original.

- snippet: how can I get that because I pay $1000 a month for my insurance and tomorrow I have surgery
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: scheduled-procedure
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads MOMS39 - 2 - V2 and MOMS39 - 2 - V2 - Copy
    review_id: c1478851-ccf4-9289-116a-345c3d6a8f51
    date: 2026-05-04
    product_version: null
    url: null
  recurrence: 6 for the scheduled-medical-event shape
  source_diversity: [ad-comment]
  first_seen: 2026-03-31
  last_seen: 2026-05-04
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: The tightest deadline anywhere in the corpus. "tomorrow I have surgery" is a trigger with a clock on it, and it opens with "how can I get that," which is intent stated outright rather than inferred. Signal would be an imminent scheduled procedure. Useless as a sale, since no plan starts overnight, and that is exactly why it is worth knowing: the moment she is most motivated is the moment the product can least help her, and the creative has never spoken to the window before it.

- snippet: Our deductible is $10,500 😭
  And I have to have surgery in June
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: scheduled-procedure
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V10
    review_id: cb09b87a-d42c-d3f0-b5d7-72ade82bee9b
    date: 2026-04-02
    product_version: null
    url: null
  recurrence: 6 for the scheduled-medical-event shape
  source_diversity: [ad-comment]
  first_seen: 2026-03-31
  last_seen: 2026-05-04
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: The same shape as the one above with two months of runway instead of one night, which makes it the more useful version commercially. She names the number and the date in two lines. Signal would be a scheduled procedure with a known cost ahead of it. The line break is original and should be kept in a lift, because the beat between the figure and the deadline is the whole effect.

- snippet: It's still sucks! My deductible is $5000 and my out of pocket maximum is $7500. I owe that from a total emergency hysterectomy last year and starting over, cancelled all my prescriptions and just can't afford it.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: medical-debt-carryover
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V5
    review_id: eebbfee2-c611-c8e0-2218-05237293d1f5
    date: 2026-03-31
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-31
  last_seen: 2026-03-31
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: One record, thin, and kept because it is the only place in the corpus where the trigger is the aftermath rather than the event. The emergency was last year. What is happening now is that she is still paying for it and has stopped taking her medication because of it. Signal would be carrying medical debt from a past emergency into a new plan year. "cancelled all my prescriptions" is the sharpest consequence stated anywhere in 1,342 records. 2 likes.

- snippet: Tried to look into it because I'm having my baby within the next month and I am still a dependent on my parents coverage so she will not be covered. I will be aging out of their insurance in Nov. I put in my information and they said there's no plans available for me...
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: aging-off-parents-plan
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: c40131c5-d9af-f066-e301-0f1fe281755b
    date: 2025-07-23
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-07-23
  last_seen: 2025-07-23
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: Thin at one record and the most load-bearing snippet in this category after the hysterectomy one. Three triggers stacked in a single comment: a birth inside a month, a baby who will have no coverage, and her own coverage ending in November. It is the only snippet in the corpus where a commenter states the causal chain outright — "Tried to look into it because" — a trigger and an attribution in the same clause. Signal would be aging off a parent's plan with a dependent arriving. It ends in the funnel turning her down, so it belongs half to objections. Dated eight months before the MOMS38 wave, which makes it era evidence that these moments predate the campaign that produced most of the corpus. 1 like and 6 replies.

- snippet: My Mom needs coverage, my Dad died end of June & the insurance Co called her 5 days after the e passed to tell her she won't have coverage after end of July
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: bereavement
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B2 - 10TH JUNE - Copy 16
    review_id: 4b95ef6b-b643-590c-cc9e-5a8e6a257d34
    date: 2025-07-10
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-07-10
  last_seen: 2025-07-10
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: off-voice
  notes: One record, thin, and the hardest one in the corpus to read. A death, a phone call five days later, and a coverage termination date, all with dates attached. Signal would be losing coverage through a spouse's death. Two things make it worth carrying past its count: it is a daughter shopping for her mother, the buying-on-behalf-of pattern the corpus profile flagged as a persona signal, and it is the only bereavement trigger in 1,342 records. The typo "the e passed" is original. 2 replies. Gated — a bereavement story lifted into insurance copy is a judgment the brand should make deliberately.

- snippet: Ive never had insurance through work and i just found out what tf a deductible is(mines $12,000) and now i have a 2000$ hospital bill that if id had known id have just suffered.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: bill-landing
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads MOMS39 - 2 - V2 and MOMS39 - 2 - V2 - Copy
    review_id: 1fd0a565-7a47-d657-98fe-a75e65f0d6a0
    date: 2026-04-10
    product_version: null
    url: null
  recurrence: 2 for "just found out", 5 for the bill-landing shape
  source_diversity: [ad-comment]
  first_seen: 2026-03-26
  last_seen: 2026-05-11
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: off-voice
  notes: The moment of discovery, a distinct trigger from the moment of cost. She did not know what a deductible was until a bill taught her. Signal would be a first encounter with the real cost of a plan she already held. "if id had known id have just suffered" is the line to keep and it is the bleakest sentence in the category: the lesson she took is to avoid care, not to switch plans.

- snippet: I about hit my deductible last month just getting blood work done. So dumb.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: bill-landing
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 893b21cf-2a53-935d-6fb2-0d5401f82354
    date: 2026-03-31
    product_version: null
    url: null
  recurrence: 1 exact, 5 as the bill-landing shape
  source_diversity: [ad-comment]
  first_seen: 2026-03-26
  last_seen: 2026-05-11
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Thin at one record and short enough to be a hook as written. The trigger is the smallness of the thing that did it — not a surgery, blood work. Signal would be routine care exposing the plan's real cost. "So dumb." is the rhythm to keep. Verified as a string: "hit my deductible" returns exactly 1 of 1,342 and "blood work" returns 2, of which this is one.

- snippet: Mine is $8,000 and I hit it in the beginning of march 🤣😭
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: bill-landing
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V8
    review_id: 3561c1ce-a975-6929-7316-36feaea03697
    date: 2026-03-26
    product_version: null
    url: null
  recurrence: 1 exact, 5 as the bill-landing shape
  source_diversity: [ad-comment]
  first_seen: 2026-03-26
  last_seen: 2026-05-11
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Thin on count. Kept because it dates the trigger inside the calendar year, which nothing else does as cleanly: eight thousand dollars gone by early March. Signal would be exhausting the deductible early in the plan year. The two emoji together, laughing and crying, are the corpus's default register for this and should not be cleaned up in a lift. 2 likes. Assembly note — this record also sits inside the 82-row counter-bid family counted in pain phrases on a 1,322 denominator; that count was not rebased here.

- snippet: I had my son schedule for tubes bc he keeps getting ear infections.  He is autistic.  They called me a week before his appointment and said they need 1500 down.... I was like how.  Our deductible is 4500. I told her I guess I'll call back after we meet our deductible.  So I guess my son will have to suffer from ear pain till then.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: child-care-blocked
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: d0a0a016-0f7f-7069-7cca-2829b3891982
    date: 2026-04-11
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-11
  last_seen: 2026-04-11
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: One record and the most producible story in the library, because it is a scene with a phone call, a number, a decision and a consequence — the whole-review-concept shape the mining method says is rare and high leverage. The trigger is a call a week before a child's procedure. Signal would be a child's scheduled care blocked by an up-front payment. It is the only moment in the corpus where the person who goes without care is the child rather than the mother, and for a brand called Health For Moms that is worth noticing. She and her husband's employer pay about $1,000 a month between them. Four-dot ellipsis and double spaces are original.

- snippet: My was $7000 they are now raising to $9000
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: renewal-hike
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: cd97741c-695c-8ada-8c99-357297a77607
    date: 2026-04-09
    product_version: null
    url: null
  recurrence: 1 exact, 2 for the renewal-hike shape
  source_diversity: [ad-comment]
  first_seen: 2026-04-09
  last_seen: 2026-04-16
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Thin at one record and structurally important out of proportion to its size. This is the renewal increase, which in most insurance categories is the single biggest switching trigger there is, and in 1,342 comments it appears about twice. The other is "Britt Johnson cost went up." on 2026-04-16, row 324e9b13. Signal would be a renewal repricing. The near-absence is the finding: either the brand's ads never run when renewal letters land, or this audience does not narrate that moment publicly. Typo "My was" is original.

- snippet: When i realized the premium was NOT part of the deductible I was flabbergasted what the point if ill spend more on a premium than I will in routine visits and even if I need a big time care the hospital will charge less than I spent all year on paying premium+deductible 🫠
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: realization
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: 0691ad4c-2fd7-6109-3b4f-290b377b39e9
    date: 2026-04-13
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-13
  last_seen: 2026-04-13
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: One record. The trigger is a realization rather than an event, which stretches the category, kept because the prompt is explicit that judgment beats the shape list when a source plainly names the moment something tipped. "When i realized" is a moment in time with a before and an after. Signal would be understanding the premium and deductible stack for the first time. The conclusion she reaches is that coverage is not worth buying at all, the same exit the corpus profile counted at 33 records across 10 ads on a 1,322 denominator. The brand's own hook opens that door. Assembly note — voc-surprise-delight.md logs this record as a surprise pointed the wrong way.

- snippet: This is me. Im on moujaro for diabetes and now I can't afford it because they want me to pay $1000 a month till my deductible is met. Im lost, can't afford it now.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: medication-cost
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 6c7fc8bc-6da9-09e3-2684-a4225d319004
    date: 2026-03-30
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-30
  last_seen: 2026-03-30
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: One record, and the only one in the corpus that opens with recognition and then supplies its own trigger. "This is me" appears in exactly 1 of 1,342 comments, checked as a string. The trigger is a drug cost changing under her. Signal would be a medication becoming unaffordable mid-treatment. "Im lost" is the phrase and voc-pain-phrase.md holds the pain half; the pain half and the trigger half are different halves of the same sentence and both passes correctly keep it.

- snippet: A mom with no job..... when I was a SAHM free insurance. Got a job after kids got school aged.... no free insurance anymore
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: return-to-work
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad Yeti State Angle - 1 - V1
    review_id: b0f32883-685f-fdd1-378e-39cf37d68f54
    date: 2026-04-06
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-06
  last_seen: 2026-04-06
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: One record and a genuinely counterintuitive trigger: going back to work is what cost her the coverage. Signal would be a return to work ending subsidized eligibility. Worth flagging to the persona work, because it names a moment in a mother's life the brand's creative has never touched and it maps onto the life stage the account already targets hardest, ages 35 to 44 at 44.5% of lifetime spend. Sits on Yeti State Angle - 1 - V1, one of the few records outside the MOMS38 family. Uses SHM's cousin SAHM, category shorthand. The five-dot and four-dot ellipses are original.

- snippet: I'm heading in to work so couldn't really look at this.
  And with bring a new rehiring I'm able to enroll into insurance. Not sure if I want to.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: enrollment-window
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: c3a8a407-abdd-ffe1-25af-b9e556bafa04
    date: 2026-04-30
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-30
  last_seen: 2026-04-30
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: One record, thin, and the only live enrollment window in the corpus. A rehire opens a special enrollment period and she is standing inside it, undecided. Signal would be a special enrollment window opened by a job change. It is also a usability finding the brand should have: she says outright she could not look at the offer because she was leaving for work, which is a mobile audience at 99.3% of spend being asked to complete a form on the way out the door. Typo "with bring" is original.

- snippet: Holly Jamison thanks. Currently looking for a new job with better insurance, but not having the best luck
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: job-change
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: fcf8227e-e6cc-7489-aaf0-73589b463a71
    date: 2026-03-28
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-28
  last_seen: 2026-03-28
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: One record. The trigger is an active job hunt undertaken for the coverage rather than the work, which inverts the usual order and is the strongest single piece of evidence in the corpus that this audience treats insurance as the thing worth changing your life around. Signal would be job searching in order to solve coverage. The record opens with another commenter's name, which is how replies render here; the name is preserved because the snippet rule is verbatim, and a writer lifting it would drop it.

- snippet: Had a similar conversation recently with my soon to be former insurance company.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: mid-switch
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 2 - V4
    review_id: 8eab4c8b-250f-7eda-5c90-294f5c168bb6
    date: 2026-03-23
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-23
  last_seen: 2026-03-23
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: One record and the closest thing in 1,342 comments to someone announcing they are mid-switch. "soon to be former" is doing all the work and is the most quotable four words in this category. Signal would be an in-progress decision to leave a current carrier. Where it sits matters as much as what it says: MOMS38 - 2 - V4 is the skit family where one woman plays both the frustrated mom and the claims rep, identified as the only creative in the account that draws agreement instead of argument. So the one person announcing a switch is answering the one ad that dramatizes an experience rather than a bill.

- snippet: What if I have an insurance plan that is too expensive but want to change it? Can I apply?
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: mid-switch
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: e9635fa0-755d-a07e-d415-00ea106aaa34
    date: 2026-03-23
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-23
  last_seen: 2026-03-23
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: One record, thin, sitting right on the line between a trigger and an objection. Kept here because it names a decision she has already made — the plan is too expensive and she wants out — and asks only whether the door is open. Signal would be an active intent to switch pending eligibility. It belongs to the wider eligibility-question cluster counted at 166 records containing a question mark on a 1,322 denominator, which is the largest untouched demand signal in the account.

- snippet: Does this work in Louisiana? Because they wouldnt let me apply for good insurance here until November.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: enrollment-window
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad Moms43 - 4 - V3
    review_id: 746bf70c-d78f-a999-85c6-e7873b195657
    date: 2026-05-27
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-05-27
  last_seen: 2026-05-27
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: One record. The trigger is a window she has been locked out of, which is the timing objection the brand says it has, arriving as a live situation instead of a stated hesitation. Signal would be being blocked from enrolling until the next window. This is the sharpest evidence available on that question and it is one comment. Verified as a string: "open enrollment" returns 1 of 1,342 and it is a different record, someone explaining the rule to a stranger. The full record continues into an anti-language complaint about smaller insurers costing more, held by voc-anti-language.md.

- snippet: That reminds me my sons insurance has been bullshit I need to call them again
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: ad-as-trigger
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad OMC - C11 - 2b
    review_id: 999a381a-b982-0b4b-b33a-96861545d9e5
    date: 2026-03-05
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-05
  last_seen: 2026-03-05
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: off-voice
  notes: One record and the only one where the ad itself is the trigger. "That reminds me" is the moment a dormant problem gets reactivated by a piece of creative, which is the exact job a top-of-funnel ad is supposed to do, and it is the single clearest evidence in 1,342 records that this account's creative can do it. Signal would be a dormant coverage problem reactivated by an ad. It is also a reminder that the thing she goes to do is call her existing insurer, not click. Off-voice; the observation survives.

- snippet: Moved from NY to GA. Went from $6500 deductible to $250 🙌🏼
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: state-move
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads MOMS39 - 2 - V2 and MOMS39 - 2 - V2 - Copy
    review_id: 67902773-6f7b-9c0a-4dc3-42d08a70c586
    date: 2026-08-14
    product_version: null
    url: null
  recurrence: 2 for "moved", 1 for this shape
  source_diversity: [ad-comment]
  first_seen: 2026-04-26
  last_seen: 2026-08-14
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: in-voice
  notes: One instance of the shape, thin, kept for two reasons: it is the only geographic trigger in the corpus, a state move that changed her deductible by a factor of twenty-six, and it is one of the few records from the quiet current era rather than the spring wave. Signal would be a move across state lines resetting plan options. Careful routing: the result she reports is real but it came from moving, not from this brand, so it is not an outcome phrase for Health For Moms and voc-outcome-phrase.md records it as a non-brand outcome. Claims-check unusable for exactly that reason. The other "moved" record is a woman whose children have moved out, a different trigger entirely.

- snippet: This is why I didn't have health insurance until I got married
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: marriage
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: d289a474-90d4-a87b-906a-57fa89cfcb79
    date: 2026-03-27
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-27
  last_seen: 2026-03-27
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: One record, thin, and historical rather than live. She is describing a trigger that already fired — marriage being what finally got her covered. Signal would be gaining coverage through a spouse. The only marriage trigger in 1,342 records, worth carrying precisely because it shows a route into coverage the brand cannot compete with. She did not buy insurance. She married into it.

- snippet: OK, this is great for mom's of young children. What about the rest of us? What about those of us who got screwed by Obama's healthcare system, and have to pay all that money out before anything is covered. What about those of us whose children are grown and moved out of the house now?  My deductible used to be reasonable, now it's almost $7000 a year.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: children-leaving-home
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: 168a3a89-cf67-9b91-d113-49e2b1fe40e7
    date: 2026-04-26
    product_version: null
    url: null
  recurrence: 2 for "moved", 16 across 7 ads for the grown-children eligibility cluster carried on a 1,322 denominator
  source_diversity: [ad-comment]
  first_seen: 2026-04-26
  last_seen: 2026-04-26
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: transformable
  notes: Mixed rather than thin because the life stage behind it is the one recurring trigger family in this category with a real count attached, even though that count is carried rather than freshly derived. The children leaving home is the trigger, and it changes her from the person the ad is speaking to into the person it is speaking past. "My deductible used to be reasonable, now it's almost $7000 a year" is a renewal-drift trigger tucked inside an eligibility complaint. 2 likes and 1 reply. The eligibility half belongs to objections. Double space before "My deductible" is original.

---

## Surprise/delight phrases

Unexpected positives the customer surfaces about the product or experience.

**Two snippets, and neither is about the product.** This is the emptiest category in the library alongside outcome phrases, and the blank is measured rather than assumed. A semantic sweep for unexpected positives across all 1,342 records at a deliberately loose 0.30 floor returned **seven results total**, and reading all seven, **not one was about Health For Moms** — five were people pleased with an employer or a plan they already held, one was a bad surprise, one was a question.

The reason is structural. A delight requires having received something. There is no unboxing here, and the one place a delight could be created is a partner-agency phone call with no recording, no transcript and no review request reaching any tool. The three product-experience phrases in the brand's context document — "It was so easy — I just answered a few questions," "They actually explained things in a way I could understand," "Nobody pressured me — they just showed me my options" — plus "Now you can cross this off your never ending to-do list!" all return **zero**, re-verified live against 1,342 on 2026-09-04.

The sharpest single fact in this category: **"thank you" appears in 3 of 1,342 records and all three thank another commenter. In fourteen months under its own ads, nobody has ever thanked Health For Moms.**

- snippet: Best advice I have gotten from an insurance agent! She didn’t have anything that fit but pointed me in the right direction!
  category: surprise_delight
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: agent-consultation
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads Moms Nahuel WV#1 - V9 and Moms Nahuel WV#1 - V9 - Copy
    review_id: 45bc3e26-5d26-1d96-30c2-686ca6e5fbf8
    date: 2026-04-17
    product_version: null
    url: null
  recurrence: 2 for the kind-agent surprise, which is the whole category
  source_diversity: [ad-comment]
  first_seen: 2026-04-01
  last_seen: 2026-04-17
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: The clearest surprise in 1,342 records and it qualifies precisely because the core job failed. She says outright that nothing fit, so the good thing cannot be the outcome she came for — it is entirely a benefit beyond it. "Best advice I have gotten from an insurance agent" is a comparative against every agent she has dealt with before, which is the exceeded-expectation signal this category is built on. 2 likes. 0.15% of the corpus. Echo false: no ad uses the phrase, checked against the ten highest-spend transcripts. Gated — usable only as service proof. Assembly note — voc-outcome-phrase.md holds the same record under the outcome lens. One record, two entries, one piece of evidence; the delight reading is the stronger of the two.

- snippet: I was connected to a very helpful agent. They weren’t able to find a lower price for our particular situation but he was very kind and helpful and respectful.
  category: surprise_delight
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: agent-consultation
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: df460383-699e-27a3-e2ef-e4f3197790f4
    date: 2026-04-01
    product_version: null
    url: null
  recurrence: 2 for the kind-agent surprise
  source_diversity: [ad-comment]
  first_seen: 2026-04-01
  last_seen: 2026-04-17
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: The other of the two, same shape, stating the miss even more plainly. "Kind and helpful and respectful" is the phrase, and the three-word pile-up is the tell that she is describing something she did not expect rather than rating a service. The pattern across both is worth naming as an inference: both women were told no and both praised the brand anyway. Two records is a candidate, nowhere near the mining method's ten-record bar, and it must never be written as a stable finding. 1 like. Also held in voc-outcome-phrase.md.

---

## Category jargon

Insider language for the category. Signals fluency.

**Seventeen terms, and this is the richest category in the library.** Health insurance is jargon-dense and this audience is fluent in it, far more fluent than the brand's creative assumes. All counts computed on **1,342** on 2026-09-04.

The finding that matters most: **the brand's ten highest-spending ads use four of these terms. The audience uses twenty.** And the one the brand leans on hardest, deductible, is the one commenters keep saying the ad has used wrong.

The practical rule that falls out of the three fluency tiers, `inferred`: **write in tier one, prove in tier two, never write in tier three.** Tier one is deductible, copay, premium and out of pocket, which every mom in the thread has. Tier two is the woman who has actually shopped for a plan — coinsurance, max out of pocket, marketplace, Obamacare, pre-existing condition, in-network, HSA, subsidy, 80/20. Tier three is the professional — guaranteed issue, medical underwriting, level-funded plan, IUA — and it belongs to the brokers and billers working these threads, not to this audience. A mom reading tier-three vocabulary in an ad hears a sales office, not a neighbor.

One count caution applies across this whole category: `author_name` is null on every row, so figures count comments and not people, and **eight of the twenty-one closed-spelling coinsurance rows are the same pasted pitch from one seller**. Where that inflates a count, the entry says so.

- snippet: deductible
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: tier-one
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: aa3d6d52-d3a5-63ad-78bb-570b4939eb59
    date: 2026-03-17
    product_version: null
    url: null
  recurrence: 207
  source_diversity: [ad-comment]
  first_seen: 2025-05-29
  last_seen: 2026-09-03
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Meaning as this audience uses it — the amount you pay yourself before the insurer pays anything — and a meaningful minority use it loosely to mean any large sum they owe, which is the confusion the whole correction cluster is about. 207 of 1,342, 15.4%, the most-used term in the corpus by a factor of nearly three. Usage condition: it almost never appears alone, always attached to a dollar figure, because the grammar of this corpus is name your number. Echo carried forward and not re-judged: customer use begins 2025-05-29 with the specific complaint shape appearing 2025-11-28, three and a half months before the earliest ad carrying it, but 95.2% of the framing sits inside an 83-day window the brand's creative opened, which is why this is mixed. The brand uses the word constantly.

- snippet: out of pocket
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: tier-one
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: de091d78-8a2f-47b0-89a4-f8d0b75be40f
    date: 2026-05-04
    product_version: null
    url: null
  recurrence: 74, of which 15 use the fuller "max out of pocket"
  source_diversity: [ad-comment]
  first_seen: 2025-07-29
  last_seen: 2026-09-03
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: The most valuable term in the library and the brand has never said it. Meaning — the annual ceiling on what you personally pay, after which the insurer covers everything. Usage condition: it appears overwhelmingly as a correction aimed at someone who called it a deductible, which makes it the vocabulary of the audience teaching the brand. 74 of 1,342, 5.5%. Cannot be echo: the phrase appears in none of the ten highest-spending ads, verified from transcripts. source-pulls/brand-self-echo-detection.md called it the most valuable organic language in the corpus at 74 of 1,322 — unchanged against the larger denominator. **The single strongest adoption candidate in the library.**

- snippet: OOP Max
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: tier-two
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: 3486a679-7242-6515-294d-89bbbf4ead71
    date: 2026-03-23
    product_version: null
    url: null
  recurrence: 1 for this abbreviation, 74 for the spelled-out term
  source_diversity: [ad-comment]
  first_seen: 2026-03-23
  last_seen: 2026-03-23
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: off-voice
  notes: Captured separately from the spelled-out term because the abbreviation is a different fluency signal — shortening a term to initials is what someone does when she assumes her reader already knows it. One record in 1,342. The related abbreviations OPM and DED appear once each, in the same broker comment held in metaphors. Usage condition: tier two at most, and never for copy aimed at a general audience, because an abbreviation nobody has to decode flatters the fluent and locks out everyone else. Captured for the record, not for lifting.

- snippet: coinsurance
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: tier-two
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: eab8e3f7-6acb-13dd-0f20-cafe015997f3
    date: 2026-03-19
    product_version: null
    url: null
  recurrence: 30 across three spellings — "coinsurance" 21, "co insurance" 5, "co-insurance" 4
  source_diversity: [ad-comment]
  first_seen: 2026-03-19
  last_seen: 2026-05-02
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Meaning — the percentage you keep paying after the deductible is met and before the out-of-pocket maximum is reached. Usage condition: it is the second beat of the correction, arriving right after out-of-pocket, and almost always paired with a ratio like 80/20. The count is a hand-computed sum of three spellings, not one search, and it needs its caveat: 8 of the 21 closed-spelling rows are the same pasted sales pitch from a single commenter, addressed to eight different women within six minutes on 2026-04-07. Excluding those, genuine coinsurance vocabulary sits at roughly 22 records. Both numbers given rather than blended. Brand never uses the term.

- snippet: copay
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: tier-one
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: ed2d19f6-e044-f812-9109-53abf2855f13
    date: 2026-04-23
    product_version: null
    url: null
  recurrence: 46, including copays and copayments
  source_diversity: [ad-comment]
  first_seen: 2025-01-08
  last_seen: 2026-09-03
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Meaning — the flat fee per visit or prescription. Tier one: universally understood and used without explanation. 46 of 1,342, 3.4%, spanning the entire corpus date range, which makes it the term with the widest time spread here and the least vulnerable to the March-April skew. The brand uses it in the negative, "there is no copays," so echo needs watching, but a term appearing from the first week of the corpus to the last day is category-standard by any reading. Usage condition: it arrives as the thing people forget, the extra charge that survives everything else, so the most common construction is a warning that copays remain.

- snippet: premium
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: tier-one
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V5
    review_id: 052aa855-2a88-45b5-7d1f-d01d622e7e65
    date: 2026-03-29
    product_version: null
    url: null
  recurrence: 46, including premiums
  source_diversity: [ad-comment]
  first_seen: 2025-07-28
  last_seen: 2026-09-03
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Meaning — the monthly payment, separate from anything owed at the point of care. 46 of 1,342, 3.4%. Usage condition and this is the useful part: the word is most often deployed as the closing move in an argument, the thing the other person forgot to add. The cited row is the corpus's complete glossary in one comment — she names deductible, out-of-pocket maximum, coinsurance, 80/20, high-deductible health plan, HSA and premium, correctly and in order, in eight lines, ending "and also you saying you Pay for that insurance.. that's called your premium.." She is the fluency ceiling of this audience and the brand has never spoken to her. The brand uses "premiums" once, promising savings on them; not echo, since customer use starts 2025-07-28.

- snippet: pre-existing condition
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: tier-two
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B2 - 10TH JUNE - Copy 16
    review_id: 63b5bd3c-f128-4292-dfb6-d62cf860437c
    date: 2025-08-27
    product_version: null
    url: null
  recurrence: 33 across the spellings pre-existing, preexisting and pre existing
  source_diversity: [ad-comment]
  first_seen: 2025-07-23
  last_seen: 2026-08-21
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: Meaning — a health problem you already have when you apply, which under ACA marketplace rules cannot be used to deny you and under other arrangements very much can. 33 of 1,342, 2.5%, spread across thirteen months, so this one survives the time skew cleanly. Usage condition: almost always the second question, right after price, and usually a warning to other women rather than a question to the brand. The cited row, "They don't cover preexisting conditions. Don't waste your time," carries 5 likes. Brand never says it. Gated — any copy using this term touches the eligibility rules and must be substantiated.

- snippet: Obamacare
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: tier-two
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads Moms36 - 3 - A - 2 - V4c and Moms36 - 3 - A - 2 - V4c - Copy
    review_id: 5db97499-85e1-b2d1-619f-8e89522382d5
    date: 2026-05-26
    product_version: null
    url: null
  recurrence: 15 for Obamacare, 14 for marketplace, counted separately
  source_diversity: [ad-comment]
  first_seen: 2025-07-29
  last_seen: 2026-08-21
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: off-voice
  notes: Meaning — the ACA individual market, and the name carries a political charge the formal term does not. Usage condition and this is why it matters: the corpus uses the two names for one thing to do two different jobs. "Obamacare" shows up in arguments about blame and politics. "Marketplace" shows up when someone is describing what she actually did. The cited row uses it in scare quotes as a grudging endorsement, "$70k out of pocket later, I am good with Obamacare," 3 likes and 3 replies. The brand says neither word in any of its ten highest-spending ads, a deliberate-looking silence given that the marketplace is its main alternative. Off-voice: the political charge is exactly what the brand's guidelines steer away from.

- snippet: Marketplace
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: tier-two
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 8a885e35-71be-e442-a0da-f462b6eb3e9f
    date: 2025-08-09
    product_version: null
    url: null
  recurrence: 14
  source_diversity: [ad-comment]
  first_seen: 2025-08-09
  last_seen: 2026-08-21
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Captured separately from Obamacare because the wording carries different weight, per the rule that different terms for one concept get separate entries. Meaning — healthcare.gov and the state exchanges. Usage condition: this is the operational word, used by women describing what they did and what it cost, not by people arguing. The cited row is the most organic-sounding comment in the corpus, predating most of the account's current creative and saying something the brand has never said. Assembly note — also held as a pain phrase, and it is the closest traceable customer version of the brand's untraceable "super middle class" quote.

- snippet: in network
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: tier-two
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 88e4072a-3f3a-1f79-94ba-3a4ea1b3dfd4
    date: 2026-06-28
    product_version: null
    url: null
  recurrence: 12 for network in any form, including out of network and networks
  source_diversity: [ad-comment]
  first_seen: 2025-07-25
  last_seen: 2026-06-28
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: Meaning — whether your doctor has a contract with your insurer, which decides what you pay. 12 of 1,342, 0.9%. Usage condition: it arrives as the hidden catch, the thing that undoes a plan that looked fine on paper. The brand gestures at the concept without using the word — the B1 samar- Copy script promises "the freedom to choose your own doctors, specialist without restrictions," verified from the transcript. Adjacent rather than echo, and the gap is the point: the brand is describing the benefit in outsider language while the audience has a precise word for it sitting unused. Gated — network breadth is a hard product claim.

- snippet: 80/20
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: tier-two
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 71c48a5b-f940-9a1b-e711-7410f1f5c0b2
    date: 2026-04-07
    product_version: null
    url: null
  recurrence: 5 for 80/20, plus one record also carrying 90/10 and one carrying 70/30 in words
  source_diversity: [ad-comment]
  first_seen: 2026-03-28
  last_seen: 2026-04-07
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: Meaning — the coinsurance split, the insurer paying 80% and you 20% after the deductible. Usage condition: spoken as a bare ratio with no explanation, which is exactly what makes it a fluency marker — nobody in these threads ever defines it. The cited row runs two ratios together, "80/20, 90/10, etc.," treating the whole family of splits as common knowledge. 5 of 1,342 and it sits entirely in an eleven-day window, too narrow to call a pattern. Safe to recognize in copy, risky to lead with.

- snippet: HSA
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: tier-two
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V8
    review_id: 6155f4df-56a0-dfdf-e091-0c5612b223a2
    date: 2026-04-18
    product_version: null
    url: null
  recurrence: 5 for HSA and HSAs, plus 1 for the spelled-out "heath savings account"
  source_diversity: [ad-comment]
  first_seen: 2026-03-29
  last_seen: 2026-06-02
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: transformable
  notes: Meaning — a health savings account, the pre-tax pot attached to a high-deductible plan. Usage condition: it appears as advice between women, "Get an HSA," and once as a flat rejection of that advice, "HSAs are AWFUL," which is the useful pair — the term is common enough that people argue about it rather than explain it. 5 of 1,342, thin. The one spelled-out use misspells it as "heath savings account," small evidence that the term travels by ear in this audience rather than off a benefits document. Brand never says it.

- snippet: catastrophic
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: tier-two
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: 9821d190-7656-3ae3-08d7-ac1955aad88f
    date: 2026-03-16
    product_version: null
    url: null
  recurrence: 10, of which 7 come from two commenters selling plans, so genuine customer use is 3
  source_diversity: [ad-comment]
  first_seen: 2026-03-16
  last_seen: 2026-05-30
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: transformable
  notes: Meaning — a plan covering only major medical disasters, used both as a plan type and as a category of event. Both numbers given, never blended. The cited row is one of the genuine three and the sharpest, because it reframes the brand's own offer: "That is essentially catastrophic insurance. You have to consider yourself self pay." That is a fluent customer classifying the product for other customers, and it is a harder read of the offer than anything in the ad. Unusable for copy without product verification.

- snippet: self pay
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: exit-the-category
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 3f6fc36c-7b2e-6268-e8c9-abaf67dc4f49
    date: 2026-04-11
    product_version: null
    url: null
  recurrence: 7 for self pay and selfpay, plus 2 for cash price and 2 for GoodRx in the same strategy
  source_diversity: [ad-comment]
  first_seen: 2025-11-27
  last_seen: 2026-05-27
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Meaning — going without insurance on purpose and negotiating the uninsured rate directly with providers, treated here as a real strategy rather than a failure. Usage condition: offered as advice, and the fluent version comes with tactics attached — ask for the cash price, use a GoodRx card, take the self-pay discount. 7 of 1,342 for the term and 11 for the whole strategy family. Mixed rather than thin because it is a coherent strategy recurring across five ads and ten months rather than one voice. **The brand never says any of it, which is notable since self-pay is its most direct competitor for this audience's dollar — not another insurer.**

- snippet: subsidy
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: subsidy-cliff
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: 87bf7f5d-1445-c1d8-1813-51f904002be8
    date: 2026-04-24
    product_version: null
    url: null
  recurrence: 4 across subsidy, subsidies and subsidized
  source_diversity: [ad-comment]
  first_seen: 2025-08-09
  last_seen: 2026-04-24
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Meaning — the income-based discount on a marketplace plan, and the cliff you fall off when you earn slightly too much. Usage condition: it appears in the fairness argument, the grievance that being middle-income is the worst place to stand. 4 of 1,342, thin. Worth capturing despite the count because it is the technical name for the complaint running through the whole corpus — the brand's context document quotes it as "We are super middle class, how are we stuck with everything?", a phrase source-pulls/brand-self-echo-detection.md could not trace to any customer. This is the traceable version in the audience's own vocabulary.

- snippet: health share
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: category-classification
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads moms-63 3e and moms-63 3e - Copy
    review_id: f89d9430-aaa6-ef95-b0b3-775cb9d42e33
    date: 2026-08-31
    product_version: null
    url: null
  recurrence: 3, including one as "Christian health share", and two of the three are sellers
  source_diversity: [ad-comment]
  first_seen: 2026-04-09
  last_seen: 2026-08-31
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: gated
  voice_check: in-voice
  notes: Meaning — a faith-based cost-sharing ministry, which is not insurance and is regulated differently. Usage condition and this is why a thin term earns a slot: the cited row is a woman asking whether Health For Moms is one. "Is this insurance or something like a Christian health share?" That is a fluent customer reaching for the nearest category she knows to classify an unfamiliar offer, and it tells you what shelf a share of this audience is putting the brand on. One of the newest records in the corpus. The classification question itself routes to the legitimacy cluster in objections.

- snippet: guaranteed issue
  category: category_jargon
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: tier-three
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads Moms36 - 3 - A - 2 - V4c and Moms36 - 3 - A - 2 - V4c - Copy
    review_id: 96452dd4-651e-9034-cd92-5fa35c41e6e1
    date: 2026-08-21
    product_version: null
    url: null
  recurrence: 1 each for guaranteed issue, medical underwriting and guaranteed renewable
  source_diversity: [ad-comment]
  first_seen: 2026-05-26
  last_seen: 2026-08-21
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: The top of tier three, captured to mark the ceiling rather than to be used. Meaning — guaranteed issue is the rule that an ACA marketplace plan must accept you regardless of health; medical underwriting is the health screening non-ACA products can apply instead. Usage condition: this vocabulary appears only in long explanatory comments from people who work in the industry, and the cited row is one commenter patiently teaching another about her son's options. One record each in 1,342. Its value is as a boundary marker: this is the language the brand must be able to survive being asked about and must never write in. Unusable — every term here is a regulatory statement.

---

## Anti-language

What the customer explicitly hates about competitors, category messaging, or marketing tropes.

**Twenty snippets, and this category has an unusual shape for this brand that is stated up front rather than buried.** Anti-language is defined as what the customer hates about competitor or industry messaging. This corpus holds almost none of that, because no rival brands are tracked in the Parker app and no competitor's comment section has been read. **What it holds instead is the audience rejecting this brand's own messaging, at close range, under the ads themselves.** That is a more useful finding and a different one, and every entry says which it is.

Counts computed by `voc-anti-language.md` on 2026-09-04 against **1,342**, with model-applied cluster counts carried from upstream on 1,322 and labelled.

### The AI-creative rejection — 6 captured, 32 across 7 ads as a model-applied tag on 1,322

The largest anti-language cluster and the only one that is genuinely about a marketing tactic rather than a product fact. Note the split between the two counts: 32 is a model-applied classification carried from `source-pulls/ad-comments.md`, while 6 is the assembly's captured set from exact-string checks. Both numbers are shown rather than blended.

- snippet: Please dont use AI instead of actors.  AI advertizing use in spite of actors goes against the morals that health for moms promotes
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: ai-creative-rejection
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 0a2fd312-dfd7-66ab-4a9b-2f7ad23795d2
    date: 2025-07-20
    product_version: null
    url: null
  recurrence: 6 captured, 32 across 7 ads carried as a model-applied tag on 1,322
  source_diversity: [ad-comment]
  first_seen: 2025-07-20
  last_seen: 2026-04-05
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Do not say — do not present a synthetic person as the face of the ad. The sharpest version of the cluster because it does not argue aesthetics, it argues hypocrisy: a brand built on caring about mothers using a machine instead of hiring one. That is a positioning problem, not a production preference. Echo false and cleanly so: the brand has never used the word AI in any of its ten highest-spend scripts, checked against the transcripts. The double space after "actors." and the misspelling "advertizing" are original.

- snippet: This is the problem with AI online commercials. If you are using a fake person for your testimonial, it unintentionally sends a message to people that no real actual person would say this about your service. I think it's always better to have a real person.

  Especially with something that is famous for being a scam, like health insurance.
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: ai-creative-rejection
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 97e9fc85-d576-2f94-1d7d-20bf77724a8d
    date: 2025-07-25
    product_version: null
    url: null
  recurrence: 6 captured
  source_diversity: [ad-comment]
  first_seen: 2025-07-20
  last_seen: 2026-04-05
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: transformable
  notes: Do not say — do not use a synthetic face to deliver a testimonial. The most valuable single record in this category because it names the mechanism rather than the irritation. Her argument is that a fake testimonial implies no real person would give a true one, and that the damage is worst in a category already assumed to be dishonest. That is a precise, testable read of why AI creative costs this brand more than it would cost a mattress company. The word "scam" here carries the standing customer-owned verdict, and this record predates the brand's scam hook by nearly eight months. The blank line is original.

- snippet: You aren’t even a real person. I’m so sick of these AI ads.
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: ai-creative-rejection
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 8c320847-b1af-9a77-439e-f9364a718984
    date: 2025-07-31
    product_version: null
    url: null
  recurrence: 6 captured
  source_diversity: [ad-comment]
  first_seen: 2025-07-20
  last_seen: 2026-04-05
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Do not say — nothing verbal, in the sense that the rejection is not of a phrase but of the speaker. "sick of these" is fatigue language, which this category treats as a first-class signal because it marks a tactic the audience has already been worn out by elsewhere. Note she is addressing the presenter directly, in the second person, which nothing else here does.

- snippet: Why is everywhere using AI actors now???
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: ai-creative-rejection
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 00bd7ced-713d-399b-f4f0-ae25e11efad2
    date: 2025-07-20
    product_version: null
    url: null
  recurrence: 6 captured
  source_diversity: [ad-comment]
  first_seen: 2025-07-20
  last_seen: 2026-04-05
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: in-voice
  notes: Do not say — nothing verbal; this rejects the category-wide tactic rather than this brand's use of it, which makes it the closest thing in the library to true industry-level anti-language as the prompt defines it. "everywhere" is doing that work. 1 like and 2 replies, so it started a conversation, which in this corpus is a reasonable proxy for resonance given there is no rating field anywhere.

- snippet: Customers hate AI ads!
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: ai-creative-rejection
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad Internal Videos - OCT - B2 - Copy 2
    review_id: 4f085c63-83e7-dc06-c714-1121bb3865c9
    date: 2025-10-26
    product_version: null
    url: null
  recurrence: 6 captured
  source_diversity: [ad-comment]
  first_seen: 2025-07-20
  last_seen: 2026-04-05
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: clear
  voice_check: off-voice
  notes: Do not say — nothing verbal. Kept for era rather than content. It sits on a different creative family from the July 2025 cluster and three months later, one of the three data points establishing that this rejection survives across ad families and years rather than belonging to one bad ad. Four words, addressed to the marketer rather than the audience.

- snippet: Creepy AI blonde lady ruins the ad tbh
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: ai-creative-rejection
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: bb13f8fd-2b12-3d19-557a-427dff553fbd
    date: 2026-04-05
    product_version: null
    url: null
  recurrence: 6 captured
  source_diversity: [ad-comment]
  first_seen: 2025-07-20
  last_seen: 2026-04-05
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Do not say — nothing verbal, but this is the most operationally useful record in the cluster, because it is the newest and it lands on MOMS38 - 1 - V2, one of the account's highest-spend ads at $41,592.95 lifetime. The rejection is not confined to old 2025 creative that has been retired; it is live on a flagship. "ruins the ad" is the phrase — she is saying the rest of the ad worked.

### The mother-identity tactic — 3 captured

- snippet: Marketing towards mothers while not covering pregnancy is a disgusting tactic.
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: identity-tactic-rejection
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 5befe57b-b90b-7f4e-8432-be2b6c4e23b7
    date: 2025-11-23
    product_version: null
    url: null
  recurrence: 3 captured for the tactic rejection
  source_diversity: [ad-comment]
  first_seen: 2025-08-12
  last_seen: 2025-12-20
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Do not say — do not lead with the mother identity while the product excludes maternity. The word doing the work is "tactic." She is not objecting to the exclusion, which would be a product objection held by voc-objection.md. She is objecting to the marketing choice of naming yourself after a group you then turn away, which is anti-language proper. "disgusting" returns 4 of 1,342 and this is the only one aimed at the brand's marketing rather than at insurance generally. The cleanest example in the library of the objection-versus-anti-language line.

- snippet: It’s illigal to deny coverage for women who are pregnant so yall need to keep that in mind with the deceitful marketing
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: identity-tactic-rejection
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 6ae515bc-68cf-3ba3-dd93-4919090bcaf2
    date: 2025-12-20
    product_version: null
    url: null
  recurrence: 3 captured for the tactic rejection
  source_diversity: [ad-comment]
  first_seen: 2025-08-12
  last_seen: 2025-12-20
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Do not say — do not describe coverage in terms that imply maternity is included. "deceitful marketing" is the exact charge and the phrase to avoid earning. The legal claim inside it is the commenter's own reading and is carried as her language, not endorsed. "deceit" returns exactly 1 of 1,342, so the specific word is a one-off while the sentiment behind it recurs. Claims-check and legal flag before this record is used anywhere.

- snippet: How can you have healthcare for moms if you don’t cover maternity? Makes zero sense. False advertising.
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: identity-tactic-rejection
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 3b2ac139-83f3-123e-bd63-6321ff80f4d4
    date: 2025-08-12
    product_version: null
    url: null
  recurrence: 3 captured for the tactic rejection
  source_diversity: [ad-comment]
  first_seen: 2025-08-12
  last_seen: 2025-12-20
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Do not say — do not use the brand name as the claim. "False advertising" is the charge and the string returns exactly 1 of 1,342, a single instance of a very specific accusation sitting inside a wide sentiment. 1 like. Assembly note — voc-objection.md correctly carries this same record as the anchor of the 36-record maternity cluster, because the first half is a product complaint. Only the last two words are anti-language.

### Do not misuse the terms — 3 captured, inside the 103-across-13-ads correction cluster carried on 1,322

- snippet: That’s not a deductible that’s a medical maximum out of pocket. You should educate people, not misinform!!
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: terminology-correction
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V5
    review_id: c0a3c689-ecb4-a5a8-ae30-3176267bcc34
    date: 2026-03-29
    product_version: null
    url: null
  recurrence: 3 captured; sits inside the 103-across-13-ads correction cluster carried on 1,322
  source_diversity: [ad-comment]
  first_seen: 2026-03-29
  last_seen: 2026-04-07
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Do not say — do not call an out-of-pocket maximum a deductible. This is the anti-language half of the corpus's single largest conversation; the product-correction half is held by voc-objection.md. What makes it anti-language rather than objection is the second sentence: she is prescribing a posture, teach rather than mislead, which is a rule about how to talk. Timing caveat governing this whole cluster: 95.2% of deductible comments sit inside the 83-day window the brand's own creative opened on 2026-03-10, so this rejection was provoked by the ad rather than found in the wild. 2 likes and 3 replies.

- snippet: As a licensed insurance broker this is VERY misleading in the beginning. The first half is talking about a medical maximum out of pocket. A deductible is something you pay before your insurance kicks in with co insurance.
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: terminology-correction
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: efb760eb-07c9-633d-d536-f92c0ac05bc4
    date: 2026-04-07
    product_version: null
    url: null
  recurrence: 3 captured; "misleading" returns 1 of 1,342
  source_diversity: [ad-comment]
  first_seen: 2026-03-29
  last_seen: 2026-04-07
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Do not say — do not open on a claim a professional can dismantle in one paragraph. The credential is the point. This is a licensed broker publishing a correction under the account's single highest-spend video at $54,322.63 lifetime, and the corpus holds several more from self-identified brokers, billers and a certified application counselor. The word to avoid earning is "misleading," which returns exactly 1 of 1,342 as a string while the behavior behind it recurs across 13 ads. Trimmed to the first three sentences; the full record is available at the row id.

- snippet: Kathy Johnson no. They’re marketing to moms and not being transparent about what they work with. I’m a licensed agent with a team that works with all plans across the board and these ads seem sooooo fishy OR they targeted the wrong demographic.
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: transparency-demand
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: b14cf007-7f2d-4f53-99dd-1f48d67324db
    date: 2025-07-25
    product_version: null
    url: null
  recurrence: 3 captured; "fishy" returns 1 of 1,342
  source_diversity: [ad-comment]
  first_seen: 2025-07-25
  last_seen: 2025-07-25
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Do not say — do not advertise without naming which carriers or plan types you actually broker. "not being transparent about what they work with" is the precise do-not-say and the most actionable line in this category, because it names a fix rather than a feeling. Thin at one record. Read with care: the author is a competing agent, so she has a commercial motive to call the ads fishy, and voc-objection.md counted 39 records across 10 ads where a rival agent pitches in these threads. The observation survives the motive; the count does not support a pattern. 3 likes.

### Do not overpromise — the too-good-to-be-true reflex

- snippet: This sounds too good to be true.
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: overpromise-rejection
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: b7aa4d37-2243-d0fe-03e6-50c8b7d495ca
    date: 2026-03-22
    product_version: null
    url: null
  recurrence: 1 exact
  source_diversity: [ad-comment]
  first_seen: 2026-03-22
  last_seen: 2026-03-22
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: in-voice
  notes: Do not say — do not pitch a benefit so far above her experience that the gap itself reads as dishonest. Mixed rather than thin on the strength of where it sits, which is checkable: this is the opening sentence of the single most-liked record in the entire corpus at 47 likes and 9 replies. "too good to be true" returns exactly 1 of 1,342 as a string, so the phrase is a one-off and its weight comes entirely from the agreement attached to it. Assembly note — this record generates three entries across three categories; count it once as evidence.

- snippet: Ha… “in these states” proceeds to list all 50 states… scam
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: false-scarcity-rejection
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: ac7bbaaf-2fd0-fd96-43a1-57a6a6551ca4
    date: 2026-03-26
    product_version: null
    url: null
  recurrence: 1 exact; the scam word returns 48 of 1,342, 3.6%
  source_diversity: [ad-comment]
  first_seen: 2026-03-26
  last_seen: 2026-03-26
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Do not say — do not use false scarcity. The ads say "you can only get that if you are a mom and you live in one of these states," verified in the transcripts of four of the ten highest-spend ads. She watched the qualifier, counted the states, and the exclusivity evaporated. This is the audience catching a specific persuasion technique in the act, which is exactly what this category means by a tactic the customer can see through. The scam word carries the standing customer-owned verdict rather than an echo flag. Assembly note — voc-objection.md holds the same record as a state-eligibility objection; the anti-language reading is about the technique, not the coverage map.

- snippet: click bait sends you to the same sales team for private quotes 🙄
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: bait-and-handoff
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad 14TH JUNE - Copy9
    review_id: ae4f05db-ea31-1f07-3d17-db49d4dfa1cf
    date: 2025-07-07
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-07-07
  last_seen: 2025-07-07
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Do not say — do not promise a distinct destination and deliver the same broker handoff. "click bait" as two words returns exactly 1 of 1,342 and the single word "clickbait" returns 0, so this is a one-off and thin. Kept because it names the mechanism of the whole funnel in eight words and because it predates the MOMS38 era by eight months, evidence that the bait complaint is not an artifact of the spring 2026 creative. Assembly note — the two extractions record different ad names for this row; voc-objection.md carries it without an ad name.

### Do not hide the handoff — inside the 15-across-10-ads call-flood cluster carried on 1,322

- snippet: Dont forget the 15k premiums plus the deductible!!!! Dont click this you will be marketed relentlessly
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: call-flood
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 6f319e61-a71d-65d1-d2ba-3cff94652445
    date: 2026-03-26
    product_version: null
    url: null
  recurrence: 1 exact; sits inside the 15-across-10-ads call-flood cluster carried on 1,322
  source_diversity: [ad-comment]
  first_seen: 2026-03-26
  last_seen: 2026-03-26
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Do not say — do not describe the next step in a way that hides that it is a marketing handoff. This is anti-language in its most damaging form, a warning issued to other viewers rather than a complaint made to the brand. "marketed relentlessly" is the phrase and it is the audience's own name for the account's business model. Mixed rather than thin because the behavior it warns about is the same one the call-flood cluster documents across ten ads.

- snippet: I filled this out because it literally says we won't be contacted by random agents. That's a lie. I immediately received 5 text messages from 5 different agents claiming to be from 5 different companies.
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: call-flood
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 8604c6b5-e71e-48d6-70fc-f849f514c914
    date: 2025-11-28
    product_version: null
    url: null
  recurrence: 1 exact; the call-flood cluster is 15 across 10 ads carried on 1,322
  source_diversity: [ad-comment]
  first_seen: 2025-11-28
  last_seen: 2025-11-28
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: off-voice
  notes: Do not say — do not promise she will not be contacted by multiple agents. **The highest-stakes entry in the library**, because it is not a rejection of a tone, it is a specific written promise quoted back with evidence that it broke. "That's a lie" is the verdict. It directly contradicts the brand context document's claimed customer phrase "Nobody pressured me — they just showed me my options," which source-pulls/brand-self-echo-detection.md verified as brand-authored copy with zero customer instances. So the brand's imagined testimonial and its customers' actual experience point in opposite directions on the same point, which is the most useful single collision in this library. 1 like. This specific promise should not be used in copy until the brand can confirm the handoff behavior changed.

- snippet: I don't like the fact that I have to click a box saying that I could get AI generated messages and 1 million phone calls.. what happened to one person calling you and just signing up for the insurance?
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: call-flood
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 959f8298-a7cd-8555-3308-4de024c91964
    date: 2025-08-13
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-08-13
  last_seen: 2025-08-13
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: transformable
  notes: Do not say — do not ask her to consent to automated contact in the language of a checkbox. One record, thin, and unusually precise: she is rejecting the consent disclosure itself, which most people never read and this one did. It joins the AI thread and the call-flood thread in a single sentence, which no other record does. "what happened to one person calling you" is the phrase and it is a plain statement of the experience she wanted instead. Useful to the funnel team more than to a copywriter.

### Do not miscast — the newest rejection in the corpus

- snippet: I’m sure the mom that can afford matching outfits prob just pays in cash 🤦‍♀️
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: casting-rejection
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads moms-63 2b and moms-63 2b - Copy
    review_id: 3fb95c2d-c637-a6a4-d741-fc04c9552ecd
    date: 2026-09-03
    product_version: null
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-09-03
  last_seen: 2026-09-03
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: transformable
  notes: Do not say — do not cast an obviously comfortable family to sell relief from medical debt. One record and thin, and it earns its place for three reasons: it rejects the casting rather than the copy, which nothing else in this library covers; it is from the current era, dated the last day of the corpus, when almost everything else here is spring 2026 or 2025; and it identifies the exact failure — the woman on screen visibly does not have the problem the ad says she has. "prob just pays in cash" is the line. A single record cannot carry a casting rule on its own and should be read next to the account's own delivery data rather than acted on alone.

### Do not leave the comments unanswered

- snippet: Oh no after reading the comments ugh I guess it’s a waste of time!!
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  sku_tag: null
  use_case_tag: comment-section-effect
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad IMG 6
    review_id: 220562bc-19b9-f4f8-1f06-c7de7a52d8af
    date: 2025-02-09
    product_version: null
    url: null
  recurrence: 1 exact; "waste of time" returns 3 of 1,342
  source_diversity: [ad-comment]
  first_seen: 2025-02-09
  last_seen: 2026-03-24
  confidence: thin
  brand_self_echo: false
  alliteration: false
  claims_check: unusable
  voice_check: in-voice
  notes: Do not say — nothing verbal. This is the only record in 1,342 where a person states outright that the comments changed her mind, and it stretches the category deliberately, because the prompt says to trust judgment when a source plainly names a rejection that does not fit the listed shapes. What she is rejecting is not a phrase in the ad; it is the ad's credibility after reading what other people said under it. It sits on IMG 6, the same 2025 ad that carries the Reddit-summary comment with 14 likes. **The closest thing in the library to a measured cost of the unanswered comment sections**, and it is one record, so it measures nothing yet.

---

## What's emerging

Phrases first seen in the last 30 days, meaning since 2026-08-05, with recurrence at or above 3.

**There are none, and that is the accurate answer rather than an empty section.** No phrase in this library was first seen inside the last 30 days at a recurrence of 3 or more. Padding this section by demoting the bar would launder single records into a trend, which is the one thing the assembly may never do.

What did arrive in the window is five genuinely new phrases, every one of them at **recurrence 1**. They are listed as sub-threshold candidates so the next refresh can watch them, and none should be treated as a signal today:

| Snippet | First seen | Source diversity | Provisional confidence | What might explain it |
|---|---|---|---|---|
| "I called them they spammed me and wasted hours of my time to tell me it was going to cost $400/month LOL" | 2026-09-03 | ad-comment | thin | The only completed customer journey in the corpus. It arrived the day the pulls ran and it did not exist when the first three extractions ran on 2026-09-03. If a second one appears, the outcome category stops being a blank and starts being a warning. |
| "I'm sure the mom that can afford matching outfits prob just pays in cash" | 2026-09-03 | ad-comment | thin | Lands on `moms-63 2b`, a current creative. The first casting rejection in the library, where every earlier creative rejection was about AI rather than about who was cast. Worth watching as the newer ads move away from synthetic presenters. |
| "It doesn't make sense. It's never made sense." | 2026-09-03 | ad-comment | thin | On `Moms43 - 5 - V1`, outside the MOMS38 family. Evidence the cost grief persists where the creative has stopped naming a number. |
| "I need insurance I don't have to pay" | 2026-08-26 | ad-comment | thin | The shortest form of the paying-twice pain and the only one from the current era. |
| "Is this insurance or something like a Christian health share?" | 2026-08-31 | ad-comment | thin | The classification question. Two of the three health-share records are sellers; this one is a customer trying to work out what shelf the brand sits on. |

**One structural caution on this whole section.** The corpus is very thin in the recent window: **86 comments since 2026-07-01 out of 1,342**, and most of those are the single word "Help" under one ad. A 30-day emergence test run against 86 records cannot produce a recurrence of 3 for almost anything. The empty section is as much a fact about comment volume as about language.

## What's fading

Phrases that previously recurred but have not appeared in the last 60 days, meaning nothing since 2026-07-06.

**Read this section with its caveat first, because the caveat is bigger than the section.** Almost every large cluster in this library goes quiet after May 2026, and the corpus goes quiet at the same time. With 86 records in the last two months against 846 in March and April alone — 64.0% of the corpus in two months, carried from `voc-corpus-profile.md` on 1,322 — **what looks like fading language is far more likely to be fading comment volume.** Nothing below should be archived or demoted on this evidence. They are listed because the template asks for them and because the next refresh needs the baseline.

| Snippet or cluster | Last seen | Hypothesis for the quiet |
|---|---|---|
| The counter-bid, 82 records — "Lucky! Mine is $11,000", "6k is a dream", "Wow only 6? Must be nice" | 2026-05-24 | The behavior is a response to an ad naming a number. The `MOMS38 - 1` family that named $6,000 stopped carrying the spend, so the prompt that produced the behavior went away. This is creative-driven, not audience-driven. |
| The terminology correction, 51 as a floor | 2026-05-22 | Same cause. The correction exists because a specific script says a specific wrong thing; when that script stops running, the correction stops. |
| The luck-and-winning frame, 11 records | 2026-05-07 | Lives entirely inside `MOMS38 - 1`. Its disappearance and the creative family's are the same event. |
| The call-flood warnings, 17 records | 2026-05-17 | Unclear, and this is the one worth checking rather than assuming. It could be quiet volume, or it could mean the handoff behavior changed. The brand can answer this and Parker cannot. |
| Coinsurance, 30 across three spellings | 2026-05-02 | Rides on the correction cluster. Eight of its records were also one seller's pasted pitch, and that seller stopped posting. |
| The AI-creative rejection, 6 captured and 32 tagged | 2026-04-05 | The most likely genuine fade in the library, because the account's newer creative has moved toward real presenters. Worth confirming against the creative timeline before calling it. |
| The system-replacement wish, 6 records | 2026-04-26 | Political language tracks news cycles more than ad cycles. Low confidence either way. |
| The mother-identity tactic rejection, 3 records | 2025-12-20 | Genuinely old. Nothing in 2026 repeats the "disgusting tactic" framing, while the underlying maternity objection stayed live through 2026-06-09. The complaint survived; the way of phrasing it did not. |
| Form friction, 6 records | 2026-03-15 | Six records over eight months was never a stable pattern. Treat as noise rather than fade. |

## Flagged for review

**1. Echo-flagged snippets sitting inside high-recurrence clusters.** Three entries from two distinct records, since row `c07a7826` is flagged in both the categories it appears in.

- Row `c07a7826`, "I like how it's 'insurance that has your back'…" — flagged `true` in both metaphors and objections, where it sits inside the 42-record pre-existing cluster. This is the verdict the assembly changed from the objection pass's `false`. The brand's own phrase closes five of the ten highest-spending ads and comes back exactly once in 1,342 comments, hostile. Do not use as primary copy under any circumstance; it is evidence against the claim it quotes.
- Row `1afe1a89`, "Health care for moms but you don't qualify if your pregnant? Make that make sense." — flagged `true` inside the 36-record maternity cluster. The brand's tweet-overlay sentence pattern turned back on it. The objection underneath is real and fully carried by five other entries in that cluster.

**2. Every single-source snippet being treated as canon — which is all 167 of them.** This is not a list, it is the state of the library. One source type means the template's own bar for `strong` cannot be met by anything here. Read every `mixed` in this library as "recurs meaningfully in the only place we can see." The fix is a Reddit or forum pull, named as available by the team on 2026-09-03 and never run.

**3. High recurrence, low diversity — possible vocal-minority artifacts.**

- **The counter-bid, 82 records.** All inside one creative family, all inside a ten-week window. It is the largest behavioral pattern in the library and it may be a property of one ad rather than of this audience. The one piece of evidence against that reading is row `df4332e6` from 2025-07-28, on a different ad, answering a different number, which suggests the behavior generalizes. One record is thin support for that.
- **Everything deductible-adjacent.** `source-pulls/brand-self-echo-detection.md` measured 95.2% of the deductible framing inside an 83-day window the brand's own creative opened. That does not make the pain fake — 5 records predate the launch and `dc090fc7` from 2026-02-14 is the cleanest of them — but it means the *volume* is brand-provoked. Every count in this library that rests on "deductible" carries that caveat.
- **Coinsurance at 30, and catastrophic at 10.** Eight of the coinsurance rows and seven of the catastrophic rows are pasted sales pitches from commenters selling their own products, three of them posted within four minutes of each other. Both entries carry the corrected figure — roughly 22 and 3 — and both numbers are shown rather than blended. `author_name` is null on all 1,342 rows, so no count in this library distinguishes people from comments.
- **The luck frame at 11.** Clears the mining method's ten-record bar by one, and sits entirely in one creative family.

**4. Two categories that are near-blanks by structure rather than by shortage.** Outcome phrases at 3 and surprise-and-delight at 2, with zero records in either describing the product. Any downstream skill that queries this library for a testimonial, a result, or a pleasant surprise will find nothing usable, and that is correct. **Do not write one from the brand's context document**, where all seven claimed outcome and experience phrases were verified at zero in the customer record and re-verified live on 2026-09-04.

**5. Every identity and behavioral-signal tag is null.** The retrieval mechanism this library exists to serve cannot run until `personas-profile.md` lands.

## Open loops

Four loops. The assembly is the only seat with the whole picture, so these are the questions that no single extraction could see, and none of them repeats a loop already filed in the nine extractions or in `source-pulls/brand-self-echo-detection.md`. The missing Reddit pull, the missing reviews and the missing surveys are infrastructure items and sit in the frontmatter and the flagged section rather than here, per the rubric.

**1. Four separate categories say the same thing: this audience believes coverage happens to her.**

This is the cross-category convergence the assembly exists to find, and it is the highest-stakes thing in the library. The metaphors say coverage is luck — 11 records treating another woman's plan as a lottery win, carrying three of the four highest like-counts in the whole library. The trigger moments say the same in life events: what actually changed a woman's coverage in this corpus is a job, a state move, a marriage, an employer, a rehire, a death. Almost never a decision she made. The objections say it outright in the no-standing-to-shop cluster — "My job picks the plan that they offer." And the aspirational phrases say it at the top of the funnel, where six records ask for the whole system to be replaced rather than shopped. Against all of that, every ad in the account asks her to believe thirty seconds of clicking will change her situation.

Pull: **Pattern.** The same belief keeps surfacing in four categories that were extracted separately, by different passes, from different slices of the corpus, and none of them could see the others.

Question: What does this audience believe she has the power to change about her own coverage?

Why it matters: if she believes the answer is nothing, then the account's entire persuasion premise is arguing with her worldview before it makes an offer, and no amount of hook testing fixes that. It is the deepest question this library can raise and it would reshape the messaging strategy rather than tune it. Territory: **Messaging.**

*Note: `voc-metaphor.md` filed a narrower version of this from the luck evidence alone. This is that question arriving with three more categories behind it, and it supersedes rather than repeats the narrower one.*

**2. Roughly 108 records across five separate clusters are about being turned away.**

No single extraction could see the size of this, because it is split across five objection clusters that each looked moderate on its own: maternity at 36, pre-existing conditions at 42, silent rejection at 11, state exclusion at 15 as a floor, and the income floor at 4. Added up that is roughly 108 of 1,322, about 8.2%, and the true distinct count is somewhat lower because the maternity and pre-existing clusters share at least two records. Even discounted, it is by a wide margin the largest single thing in this library. And the only two records in 1,342 that praise this brand's service both come from women who were told no.

Pull: **Gap.** An enormous amount of paid reach is landing on people the product cannot serve, the evidence has been sitting in five separate piles, and nobody has added it up.

Question: How many of the people this account reaches can actually be sold to?

Why it matters: at $22.67 per lead across 4,336 leads in ninety days, the difference between a targeting problem and a creative problem is the whole media plan. If a large share of delivery is structurally unqualifiable, the fix is upstream of any script. **Routed to the brand** for the qualification rules, which only the team and the partner agency know. Territory: **Product.**

**3. Almost everything in this library is a photograph of ten weeks under one ad.**

The counter-bid, the correction cluster, the luck frame, the coinsurance vocabulary and most of the pain language all sit inside `MOMS38 - 1` and inside March to May 2026. `voc-corpus-profile.md` measured 846 of 1,322 comments, 64.0%, in March and April alone, and 795 of 1,322, 60.1%, on that one creative family. The 86 records since July are mostly the single word "Help."

Pull: **Surprise.** A fourteen-month corpus turns out to be, in practice, a ten-week corpus, and that only becomes visible when all nine extractions are laid next to each other and every large cluster shares the same last-seen date.

Question: What does this audience talk about when the brand is not showing her a number?

Why it matters: the brand may be reading its customer's voice when it is really reading its own creative's echo. If the language is genuinely different outside that window, then the messaging bank is tuned to a campaign rather than to a customer, and every downstream script inherits the bias. Territory: **Messaging.**

**4. There are 167 voices in this library and no way to know which ones belong to the same woman.**

Every `identity_tag` and every `behavioral_signal_tag` is null, on all 167 snippets, because `personas-profile.md` does not exist. On top of that, `author_name` and `author_id` are null on all 1,342 source rows, so even the raw corpus cannot tell one person from another. `voc-trigger-moment.md` wrote the intended signal into every one of its 23 snippets so the tags can be attached in a single pass, and this library is the reason that matters.

Pull: **Gap.** The mechanism this whole library was built to serve — pick a persona, pull her voice — cannot run, and the fix is one document away.

Question: Which of these voices belong to the same woman?

Why it matters: without it, every skill that loads this library gets the brand's whole audience at once rather than the person it is writing to, which is precisely the generic output the library exists to prevent. **Routed to the persona work**, which owns the slugs. Territory: **Personas.**

## Sources

This pass did not return to the raw customer sources. Its inputs were the nine category extractions plus the reference docs, exactly as the prompt directs.

- `personas/voice-of-customer/voc-pain-phrase.md` — 29 snippets, counts on 1,322, generated 2026-09-04 from pulls run 2026-09-03.
- `personas/voice-of-customer/voc-outcome-phrase.md` — 3 snippets, counts on 1,342, pulls 2026-09-04.
- `personas/voice-of-customer/voc-metaphor.md` — 15 snippets, counts on 1,342, pulls 2026-09-04. Source of two of the three alliteration flags.
- `personas/voice-of-customer/voc-objection.md` — 48 snippets, counts on 1,322, pulls 2026-09-03. The largest single input.
- `personas/voice-of-customer/voc-aspirational.md` — 10 snippets, counts on 1,342, pulls 2026-09-04.
- `personas/voice-of-customer/voc-trigger-moment.md` — 23 snippets, counts on 1,342, pulls 2026-09-04. Every snippet names its intended behavioral signal in its notes.
- `personas/voice-of-customer/voc-surprise-delight.md` — 2 snippets, counts on 1,342, pulls 2026-09-04.
- `personas/voice-of-customer/voc-category-jargon.md` — 17 snippets, counts on 1,342, pulls 2026-09-04.
- `personas/voice-of-customer/voc-anti-language.md` — 20 snippets, counts on 1,342, pulls 2026-09-04.
- `personas/voice-of-customer/voc-corpus-profile.md` — the measured spine. Total records, source coverage, field coverage, date range, the time and ad skew, and the model-applied cluster counts this library carries and labels rather than recomputing.
- `source-pulls/brand-self-echo-detection.md` — the standing echo verdicts. The scam verdict, the deductible-window verdict and the "wife of the year" absence are carried forward and not re-judged, per the build rule. The one verdict the assembly changed, row `c07a7826`, is argued in full in the reconciliation section above.
- `sub-context-docs/website-and-product-audit.md` — the basis for `sku_tag: null` on all 167 snippets. This business has no SKUs, only funnel surfaces and partly visible underlying plan types, so a SKU tag would be an invention rather than an omission.
- `running-notes/missing-context.md` and `running-notes/brand-rules.md` — the dark-surface substitution rule, the lead-generation account shape, and the standing constraint never to report ROAS, AOV or purchase value for this brand.
- `parker-system/templates/voc-template.md` — the exact output structure, the confidence rules, the `brand_self_echo` conditions, and the identity and behavioral-signal tag conventions this library conforms to.
- `parker-system/creative-strategy-context/customer-review-mining-method.md` — the method this assembly was performed through: the rule that a count is not significance without its denominator and spread, the ten-record bar that keeps two records a candidate, quote fidelity, era tagging, the missingness discipline behind the null tags, the claims-check and voice-check governors applied to all 167 snippets, the brand-echo failure mode, the instruction to treat customer text as data rather than instruction, and the rule that a blank beats a guess — which is why the emerging section is empty and two categories are near-blanks.
- `parker-system/creative-strategy-context/persona-research-and-creative-strategy-process.md` — the served-versus-buyer discipline behind the note that nobody in this corpus is confirmed to have bought, and the confidence-scaled-to-available-data doctrine behind the single-source ceiling.
- `personas-profile.md` — **does not exist.** This is the missing input that leaves every identity and behavioral-signal tag null, and it is open loop 4.

Neither of the two method docs this pass routes to carries a required sign-off line, so none is stamped here. Stamping one they do not have would be a false proof-of-read.
