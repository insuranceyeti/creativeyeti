---
brand: health-for-moms
doc: voc-pain-phrase
category: pain_phrase
generated_on: 2026-09-04
refresh_by: 2026-10-04
corpus_denominator: 1322
snippets_captured: 29
sources_read:
  - Parker MCP search_facebook_ad_comments_sql, Meta ad account HealthForMoms, act 484897827497337. Ran 18 filtered pulls on 2026-09-03. Corpus end re-confirmed by my own offset probe, not carried from upstream. Offset 1300 returned exactly 22 rows, which pins the total at 1,322.
  - Parker MCP search_facebook_ad_comments_semantic, four themed passes on 2026-09-03. Every pass reported totalCommentsAnalyzed 1322, which agrees with the SQL denominator.
  - Parker MCP search_customer_reviews_sql, unfiltered, 2026-09-03. Returned totalReviews 0. Checked live by me, not assumed from a note.
  - Parker MCP semantic_search_post_purchase_survey, 2026-09-03. Returned totalResponsesForBrand 0 with the collection existing.
  - Parker MCP search_facebook_ads_sql, 2026-09-03, keyword MOMS38, lifetime mode, with the scripts block. Full transcripts read on the six highest-spend variants of the creative family that produced most of this language.
  - personas/voice-of-customer/voc-corpus-profile.md, 2026-09-03, for the denominators, the field coverage and the data limits this pass inherits.
  - source-pulls/ad-comments.md, 2026-09-03, the full-corpus persona read of the same rows.
  - source-pulls/brand-self-echo-detection.md, 2026-09-03, for the standing echo verdicts this pass must honor.
  - running-notes/missing-context.md and running-notes/brand-rules.md, for the dark-surface substitution rule and the standing constraints.
  - parker-system/creative-strategy-context/customer-review-mining-method.md, the canonical mining method applied here.
  - parker-system/creative-strategy-context/persona-research-and-creative-strategy-process.md, for the evidence ranking and the served-versus-buyer discipline.
expected_sources_missing:
  - customer reviews. Zero rows, verified live 2026-09-03.
  - post-purchase surveys. Zero rows, verified live 2026-09-03.
  - Reddit and forums. Named by the team as the substitute source on 2026-09-03, not yet pulled.
  - competitor and category reviews. No rival brands tracked in the Parker app. Branch deferred by the user 2026-09-03.
  - brand-reputation, other-reviews, support tickets, organic social comments. None ingested.
  - personas-profile.md. Not yet written, so no identity or behavioral-signal slug exists to tag with.
data_limitations:
  - One source only. Facebook and Instagram ad comments are the whole first-party record of how this customer talks. The mining method ranks survey and review evidence at the top and public comments near the bottom, so the confidence ceiling on every snippet here is mixed, never strong, no matter how often a phrase recurs.
  - No cross-source recurrence is possible. The prompt's own bar for strong confidence is a phrase showing up in several kinds of source. This brand has one kind. So no snippet in this doc earns strong, and that is a fact about the corpus rather than a fact about the phrases.
  - Not one commenter is confirmed to have bought anything. Every phrase here comes from someone the algorithm served, not from a buyer.
  - author_name and author_id are null on all 1,322 rows. Recurrence counts are counts of comments, never counts of people. One person posting five times reads as five.
  - permalink_url is null on all 1,322 rows, so the url field is null on every snippet. Verification runs through the row id and the Parker tool, not through a link.
  - Severe time skew, and it bites this doc harder than most. 202 of the 207 comments containing the word "deductible" sit between 2026-03-10 and 2026-05-31. Almost all the pain language in this corpus is a spring 2026 event.
  - Severe ad skew. Most of the language below sits under one creative family, MOMS38 - 1, whose six highest-spend variants all run the same script.
  - No identity or behavioral-signal slugs exist. identity_tag and behavioral_signal_tag are null on every snippet by rule, not by oversight.
  - The Parker comment tool returns an unreliable total when no text filter is applied. An unfiltered call returned total 0 while returning rows. Every count in this doc came from a text-filtered call, where the total is correct, or from an offset probe I ran myself.
  - There is no get_current_time tool on this MCP surface, so the date comes from the session clock. Worth naming plainly: every Parker pull behind this doc ran on 2026-09-03, which is also the corpus end date and the stamp on every sibling doc in this build, and the clock rolled to 2026-09-04 while the doc was being written. generated_on carries the write date and the sources_read entries carry the pull date, so the two never have to be guessed apart.
  - refresh_by is set 30 days out rather than the 180-day voice-of-customer cadence in parker-system/system/refresh-cadence.md. Two triggers have already fired. Comments accrue daily while campaigns are live, and personas-profile.md will land soon and will fill the null tags on every snippet here.
---

# Pain phrases — Health For Moms

## The honest headline before any phrase

This brand has no customer reviews and no post-purchase surveys. I checked both live on 2026-09-03 rather than trusting the note. `search_customer_reviews_sql` returned `totalReviews: 0` and `semantic_search_post_purchase_survey` returned `totalResponsesForBrand: 0`. So every phrase below comes from Facebook and Instagram ad comments, and nothing here may ever be described as this brand's review corpus. `verified`.

That single fact sets the ceiling. The mining method ranks evidence with survey and review data at the top and public comments near the bottom, and the persona method says the same thing in different words. This brand holds only the bottom rank. The prompt's rule is that cross-source recurrence earns strong confidence and single-source recurrence earns mixed. There is one source. So **no snippet in this doc is marked strong**, and any downstream doc that rounds one up is inventing certainty that does not exist.

## How I built this, and what I checked

I did not take the upstream numbers on faith. Here is the trail.

**I re-pinned the denominator myself.** An unfiltered call to `search_facebook_ad_comments_sql` at offset 1300 returned exactly 22 rows. That puts the end of the corpus at 1,322 and matches the `totalCommentsAnalyzed: 1322` that all four of my semantic passes reported. So 1,322 is the denominator behind every count below. `verified`.

**I re-derived the pattern I was asked to test rather than repeat it.** The upstream read says roughly 160 comments across 17 ads post the commenter's own deductible figure. I could not recount a model-applied tag through the tool, so I went at it with a structural string instead, which is checkable by anyone. The string "mine is" appears in **82 of 1,322 comments, or 6.2%**. I read all 82 in full. **76 of the 82 post a specific dollar figure for the commenter's own plan.** Of those 76, **64, or 84%, name a number higher than the $6,000 the ad states.** They sit on 8 distinct ad names: MOMS38 - 1 - V1, V2, V3, V5, V8, V9 and V10, plus MOMS39 - 2 - V2. `verified`, string count and my own read of every row.

That is a narrower slice than the upstream 160, because "mine is" is only one of the ways a person posts her number. Others write "My deductible is $10k" or "I pay 6,000" or just "$8000." The wider count of 160 is consistent with what I see. The direction of the finding survives my recount, and it survives it on a number a skeptic can re-run in one call.

**I pulled the creative itself rather than reading the ad name.** The prompt is strict that a creative claim needs full media, so I pulled the MOMS38 family through `search_facebook_ads_sql` with the scripts block. All six highest-spend variants launched 2026-03-10 and run the same words. The opening is: "My deductible is $6,000. I have to spend $6,000 in medical expenses before everything is taken care of and there's no copays. But yet I pay for that insurance." The family carries $178,097.18 lifetime spend and 8,078 leads at a $22.05 cost per lead, with V1 alone at $54,322.63 and 2,693 leads at $20.17. `verified`, read from the transcripts and the lifetime metrics, not from labels.

That matters for two reasons. It confirms the $6,000 is the brand's number, not the customer's. And it shows the ad already contains the paying-twice frame in its own voice, which is exactly the thing the echo governor exists to catch.

## Testing the reading: is the pain being uninsured, or being insured and still broke?

I was asked to test whether the dominant pain is not being uninsured but being insured and still broke. I ran it as a head-to-head string check against the full 1,322.

| What I looked for | Comments | Share of 1,322 |
|---|---|---|
| "mine is", the counter-figure disclosure | 82 | 6.2% |
| "deductible" | 207 | 15.7% |
| "premium" | 46 | 3.5% |
| "afford" | 46 | 3.5% |
| "a month", almost always a premium being paid | 45 | 3.4% |
| "I pay" | 22 | 1.7% |
| "we pay" | 16 | 1.2% |
| "no insurance" | 11 | 0.8% |
| **"uninsured"** | **2** | **0.15%** |

All `verified` string counts, case-insensitive, against the full corpus.

The reading holds, and the gap is not close. The word "uninsured" appears **twice in 1,322 comments**. The word "deductible" appears **207 times**. People here are not saying they have no coverage. They are saying they have coverage and it is not doing anything for them. One comment says it in nine words, and it is the cleanest statement of the whole pattern in the corpus: "Why we have insurance and still have a damn bill when we go to the doctor." `verified`, row `fd6d3fb4-3868-cc4d-1ebe-ca2e8ef40dc8`, MOMS38 - 1 - V8, 2026-04-15.

The most-liked comment in the corpus checks out too. I sorted on `like_count` and read the top of the list myself. Row `b7aa4d37-2243-d0fe-03e6-50c8b7d495ca` on MOMS38 - 1 - V1, dated 2026-03-22, carries 47 likes and 9 replies, the highest in 1,322 records. It ends "I want the 1990’s back." She is not uninsured. She opens by saying she pays over $1,000 a month. `verified`.

**But the reading needs one correction, and it is a real one.** The upstream framing treats this as the brand's dominant customer pain. What the dates show is narrower. Of the 207 comments containing "deductible", only **5 predate 2026-03-10**, the day the MOMS38 family launched, and only **5 came after 2026-06-01**. So **197 of 207, or 95.2%, land inside an 83-day window that starts the day this creative went live**. `verified` by two date-bounded pulls.

So this is not a pain the brand discovered sitting in the wild. It is a pain the brand's own ad went and struck, hard, in one campaign window. That is a compliment to the creative and a warning about the corpus at the same time. The pain is real and the volume is prompted. `inferred`, and the two date pulls are the whole basis.

The pain does predate the ad, which is what keeps these phrases out of the echo bin. Two comments prove it. On 2025-11-28, eight months before MOMS38 launched, someone wrote "making a 6000 deductible before my insurance will pay for anything we barely go to the doctor as is." On 2026-02-14 someone wrote "the premium for that policy costs more than my house note... either way people are screwed. Broken system." And on 2025-07-28, under a completely different ad with a completely different number, someone was already bidding the ad's figure up: "600? Try 1000+, then this ad would be more realistic." That last one matters most, because it shows the counter-bid behavior is not an artifact of the $6,000 creative. It is how this audience answers any number an insurance ad puts on screen. `verified`, all three rows pulled and dated.

**One more check on the echo governor.** The word "scam" appears in 45 of 1,322 comments, and **15 of those 45, or 33%, predate the MOMS38 launch**, the earliest on 2025-07-28. Compare that to "deductible" at 5 of 207, or 2.4%. So the scam framing is genuinely the customer's own and the brand borrowed it, while the deductible framing is overwhelmingly the brand's prompt coming back. Both are useful. They are not the same kind of evidence, and every snippet below says which it is. `verified`.

## What is fading, and what is live right now

This is the part a writer needs before pulling any phrase, so it goes before the bank rather than after.

The pain language is quiet now. Since 2026-07-01 the corpus holds only **86 comments**, and a large share of them are the single word "Help" under one ad, `Moms43 - 4 - V3`. The current creative generates eligibility questions, state complaints and pre-existing condition objections, not the raw cost grief that fills March through May. `verified`, from a date-bounded pull I read in full.

Two live pain phrases did surface in the last stretch, and I have kept both. "It doesn't make sense. It's never made sense." from 2026-09-03, which is the newest record in the whole corpus. And "I need insurance I don't have to pay" from 2026-08-26. Thin, and marked thin. But they are the only current-era evidence there is.

So the honest note for a writer: this bank is a rich photograph of one spring. Every snippet carries first-seen and last-seen so you can see for yourself whether the phrase you are reaching for is live or historical.

## Pain phrases

Twenty-nine distinct phrasings. Each is verbatim, with the original spelling, punctuation, casing and emoji preserved exactly. Source type is `ad-comment` for all of them, and the `platform` line carries the ad the comment sits under, because that is the only placement handle these rows have and a reader needs it to know which creative provoked the phrase. It reads Facebook or Instagram rather than one of the two, because the corpus does not record which of the two a given comment came from. `review_id` carries the Parker `comment_id`, which is the only stable handle these rows have. `url` is null on every one because `permalink_url` is null on all 1,322 records. `identity_tag` and `behavioral_signal_tag` are null on every one because `personas-profile.md` does not exist yet and this pass never invents a slug.

**How to read the three claim marks on these blocks, since they work the same way on all 29.** The `snippet` line itself is always `stated`. It is what the customer wrote and I am recording it as she said it, checked character for character against the row the tool returned, down to the curly and straight apostrophes, the double space and the misspelled drug name. Every `recurrence` figure that comes from a string count is `verified`, because it is a case-insensitive match anyone can re-run against the same 1,322 and get the same number. Every `recurrence` figure I describe as a family, and every grouping of two differently worded snippets into one pain, is `inferred`, and the notes say so and give the basis. Nothing here is `verified` at the level of the phrase being a real cross-source pattern, because that mark requires more than one kind of source and this brand has exactly one. That is why the confidence column tops out at mixed.

- snippet: I want the 1990’s back.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: b7aa4d37-2243-d0fe-03e6-50c8b7d495ca
    date: 2026-03-22
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-22
  last_seen: 2026-03-22
  confidence: mixed
  brand_self_echo: false
  notes: One instance in 1,322, so by the letter of the rule this is a candidate and not a pattern. It is kept and marked mixed rather than thin for one reason that is checkable. It sits inside the single most-liked record in the entire corpus, at 47 likes and 9 replies, which I confirmed by sorting on like_count and reading the top of the list. Roughly 70% to 75% of this corpus carries no likes at all, so 47 is agreement on a scale nothing else here reaches. The full comment opens "This sounds too good to be true. I pay over $1,000 a month for a premium. We have to pay an $8000 deductible per family member or up to $17,000 for the entire family." She is insured and paying, which is why this line anchors the whole doc.

- snippet: Why we have insurance and still have a damn bill when we go to the doctor.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V8
    review_id: fd6d3fb4-3868-cc4d-1ebe-ca2e8ef40dc8
    date: 2026-04-15
    url: null
  recurrence: 1 exact, roughly 20 as a family
  source_diversity: [ad-comment]
  first_seen: 2025-11-28
  last_seen: 2026-05-26
  confidence: mixed
  brand_self_echo: false
  notes: The tightest statement of the corpus's central pain. The exact wording appears once. The idea behind it recurs across the paying-twice snippets below and in the 45 comments containing "premium" and the 46 containing "afford". First_seen is set to 2025-11-28 for the family rather than for this row, because that is the earliest dated instance I found of the same idea, on row d12d9274-ff4e-6ca8-37c3-9f4b9d262f90. Echo flagged false because the frame predates the MOMS38 creative by eight months, though the ad does carry its own version of it in the line "But yet I pay for that insurance."

- snippet: Lucky! Mine is $11,000
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: aa3d6d52-d3a5-63ad-78bb-570b4939eb59
    date: 2026-03-17
    url: null
  recurrence: 82
  source_diversity: [ad-comment]
  first_seen: 2026-03-13
  last_seen: 2026-05-24
  confidence: mixed
  brand_self_echo: false
  notes: The single best exemplar of the counter-bid, at 19 likes and 4 replies. Recurrence 82 is my own string count for "mine is" against the full 1,322, or 6.2%, and I read all 82 rows. 76 of the 82 post a specific figure, and 64 of those, or 84%, name a number above the ad's $6,000. The 82 spread across 8 distinct ad names. Every one of the 82 is dated between 2026-03-13 and 2026-05-24, so this exact behavior is a spring 2026 event on one creative family and a writer should know that before treating it as evergreen. Echo false because the number is hers, not the brand's, but the disclosure was plainly prompted by the ad naming a number first.

- snippet: Wow only 6? Must be nice
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 22fc32bf-dfce-3e9f-59ca-4f44df9c9493
    date: 2026-03-27
    url: null
  recurrence: 3
  source_diversity: [ad-comment]
  first_seen: 2026-03-20
  last_seen: 2026-04-10
  confidence: thin
  brand_self_echo: false
  notes: Marked thin because "must be nice" appears in only 3 of 1,322 comments, which is under the ten-record bar the mining method sets. Kept because it is the sharpest short form of the counter-bid and it carries 13 likes, which puts it inside the top fifteen most-agreed-with records in the corpus. The other two instances are "Must be nice. I was told I would have to spend $15,000" on 2026-03-20 and "Yes, 6000 must be nice. Mine is 9000" on 2026-04-10. Use it as a hook candidate, not as a pattern claim.

- snippet: Mine is a 20k deductible before insurance helps with anything. 6k is a dream
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: c28373d7-0028-0042-fc87-1cc7e3858509
    date: 2026-03-21
    url: null
  recurrence: 82 as part of the counter-bid family
  source_diversity: [ad-comment]
  first_seen: 2026-03-13
  last_seen: 2026-05-24
  confidence: mixed
  brand_self_echo: false
  notes: Carries 7 likes and 6 replies. "6k is a dream" is the phrase to keep. It does the whole job in four words and it names the ad's own number as the fantasy, which is the exact inversion the brand should know about. Denominator is the same 82-row family described above.

- snippet: 600? Try 1000+, then this ad would be more realistic. American healthcare and insurance is a scam. Americans can’t even afford to die either.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: df4332e6-35fe-5247-4cfe-78ae66601144
    date: 2025-07-28
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-07-28
  last_seen: 2025-07-28
  confidence: mixed
  brand_self_echo: false
  notes: The most load-bearing single record in this doc, which is why it is kept despite a recurrence of 1. It is dated 2025-07-28, sits on a different ad called B1 samar- Copy, and answers a different number, a $600 premium rather than a $6,000 deductible. That makes it proof that the counter-bid is how this audience answers any number an insurance ad shows, not a quirk of the MOMS38 creative. It also carries the corpus's strongest standalone line, "Americans can't even afford to die either." Marked mixed rather than thin on the strength of what it establishes about era, not on its own count.

- snippet: Paying a deductible plus paying for a monthly fee is such a scam
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: fc4a4b8f-e082-a311-ba58-0bc592068e09
    date: 2026-04-06
    url: null
  recurrence: 1 exact, roughly 20 as a family
  source_diversity: [ad-comment]
  first_seen: 2025-11-28
  last_seen: 2026-05-26
  confidence: mixed
  brand_self_echo: false
  notes: The plainest naming of the paying-twice pain. Echo needs care here and the call is still false. The word "scam" is customer-owned, which I checked rather than assumed. It appears in 45 of 1,322 comments and 15 of those 45, or 33%, predate the MOMS38 launch on 2026-03-10, the earliest on 2025-07-28. Compare "deductible" at 5 of 207, or 2.4%, predating. So the scam vocabulary came from the audience and the deductible framing came from the ad. Treat the whole scam cluster as mixed echo risk per the standing verdict in source-pulls/brand-self-echo-detection.md.

- snippet: Mine is $10,000 and pay $1,200 a month in premiums. Total. Scam.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: d635af48-3b6d-4b5e-0320-08a671f85c33
    date: 2026-04-08
    url: null
  recurrence: 82 as part of the counter-bid family
  source_diversity: [ad-comment]
  first_seen: 2026-03-13
  last_seen: 2026-05-24
  confidence: mixed
  brand_self_echo: false
  notes: Sits in both families at once. It posts the counter-figure and it names the premium in the same breath, which is the shape most of the 82 take when they run past three words. The clipped ending, "Total. Scam.", is the rhythm to keep.

- snippet: We pay $40,000 a year in premiums. Doesn’t include anything. We still pay deductible and pay for services
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: 3f89f249-7ea8-6751-8cde-95fb64c13bc7
    date: 2026-04-12
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-12
  last_seen: 2026-04-12
  confidence: thin
  brand_self_echo: false
  notes: One record in 1,322, so thin by the rule and kept as a quote candidate rather than a pattern. It is the largest premium figure disclosed anywhere in the corpus. The mining method flags specific numbers as a qualifying signal and this is the extreme end of the range. Useful as an outlier that shows the ceiling, never as a typical customer.

- snippet: I still pay full price for everything all year until I pay $6k which has been never. They have never helped me pay for anything, but I give them thousands a year for what?
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V5
    review_id: be59e705-66a5-1215-96a0-bdd826f0f68c
    date: 2026-04-08
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-08
  last_seen: 2026-04-08
  confidence: thin
  brand_self_echo: false
  notes: Thin on count and high on usability, which the mining method says are different questions. It names a pain nothing else in the corpus names as clearly, which is that she never reaches the deductible at all, so the coverage is theoretical every single year. "which has been never" is the phrase. The full record also says her plan costs $645 a month for her and her kid and her out-of-pocket max is $15k.

- snippet: And then it's the end of the year, and we start all over. I literally hate NYE for this reason!
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: 78af9428-b3e7-a3d2-cc23-87e43de0db3a
    date: 2026-04-04
    url: null
  recurrence: 5
  source_diversity: [ad-comment]
  first_seen: 2026-03-24
  last_seen: 2026-05-13
  confidence: thin
  brand_self_echo: false
  notes: Carries 6 likes. Recurrence 5 is my count of the reset idea surfaced by a semantic pass and confirmed row by row, so it is a classification read rather than a string count and it is under the ten-record bar. The others are terse, such as "And it starts over yearly" and "And it resets every year." This one is the only version with a feeling attached to it, and tying the dread to a specific date on the calendar is the reason to keep it. Note the reset is a January and December event, so this phrase is seasonal by nature and a spring-heavy corpus almost certainly undercounts it.

- snippet: This year it took 35 days to hit our 8k OOP. Next year it could take as few as 1 depending on how prescriptions hit.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS39 - 2 - V2 and MOMS39 - 2 - V2 - Copy
    review_id: b3e776b8-a237-3d00-f3ad-8cbf4cf4f298
    date: 2026-03-31
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-31
  last_seen: 2026-03-31
  confidence: thin
  brand_self_echo: false
  notes: Thin at one record and worth every line of it. The mining method names specific, odd numbers as the top qualifying signal, and "35 days" and "as few as 1" are exactly that. It also carries the category's own vocabulary, OOP, which is the audience showing fluency the creative does not assume. The full record goes on to name three prescription costs of $2,600, $1,800 and $3,200 and a child's med at $3,600 per fill.

- snippet: my deductible is $4500 and I can’t afford it so I can’t go to the doctor.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V5
    review_id: 7fb10e8d-9947-c623-ef23-1612cfd63b5c
    date: 2026-04-10
    url: null
  recurrence: 7
  source_diversity: [ad-comment]
  first_seen: 2025-11-28
  last_seen: 2026-06-28
  confidence: mixed
  brand_self_echo: false
  notes: The pain where the money problem becomes a health problem. Recurrence 7 is my string count for "go to the doctor" against the full 1,322, and I read all 7. Small, but it spreads across four different ads and across three eras from November 2025 to June 2026, which is the kind of durability this corpus can rarely show. The rest of the record says she is not a mom and never will be, which is an eligibility problem for the objection pass rather than a pain, so only the pain half is captured here.

- snippet: I don't want to go to the doctor because the copay alone is $65 and the doctor isn't really listening to me most of the time 😭
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: c045c882-291f-e8d6-3039-8471b635fb4c
    date: 2026-04-12
    url: null
  recurrence: 7 as part of the avoided-care family
  source_diversity: [ad-comment]
  first_seen: 2025-11-28
  last_seen: 2026-06-28
  confidence: mixed
  brand_self_echo: false
  notes: Kept alongside the one above because it names a second reason on top of the money, which is not being listened to. That is the only place in 1,322 records where the cost pain and the care-quality pain are said in one sentence, and it is the more human of the two. Same 7-record denominator.

- snippet: This is me. Im on moujaro for diabetes and now I can't afford it because they want me to pay $1000 a month till my deductible is met. Im lost, can't afford it now.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 6c7fc8bc-6da9-09e3-2684-a4225d319004
    date: 2026-03-30
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-30
  last_seen: 2026-03-30
  confidence: thin
  brand_self_echo: false
  notes: One record, so thin, and it is here for two words. "Im lost" is the only time in 1,322 comments that anyone names the feeling rather than the figure, and the mining method says emotive and visceral language is a qualifying signal in a way that a number is not. It opens "This is me," which is the recognition the rest of the corpus almost never gives. The misspelling of the drug name is preserved exactly as written.

- snippet: Mine is $6k per person too but since it’s thru my job I don’t really have a choice
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS39 - 2 - V2 and MOMS39 - 2 - V2 - Copy
    review_id: 33936dcd-893a-25ec-3240-bd21906f0e5a
    date: 2026-03-17
    url: null
  recurrence: 24 as the employer family, 82 as the counter-bid family
  source_diversity: [ad-comment]
  first_seen: 2026-03-13
  last_seen: 2026-08-16
  confidence: mixed
  brand_self_echo: false
  notes: The pain of having no choice, which is a different pain from having a high number. The employer denominator of 24 is the string count for "employer" carried from voc-corpus-profile.md, and I confirmed the shape myself across several rows including one from 2026-08-16 that reads "If your job offers insurance you have to pick an insurance. They make you pay for one." That August date is what makes this family the most durable in the doc, since almost everything else went quiet after May. "I don't really have a choice" is the phrase.

- snippet: Insurance through employer we pay $250/week and still have copay of $50. Individual deductible is $15,000. They don’t even want to cover an MRI so I had to pay out of pocket anyway.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: 1e315434-c861-3f23-4fae-2a38acd72263
    date: 2026-03-13
    url: null
  recurrence: 24 as the employer family
  source_diversity: [ad-comment]
  first_seen: 2026-03-13
  last_seen: 2026-08-16
  confidence: mixed
  brand_self_echo: false
  notes: The fullest version of the employer pain, and it stacks four costs in one sentence, which is how this audience actually experiences the bill. Note the weekly framing rather than monthly. That is her real unit of pain and no ad in the account uses it. Dated 2026-03-13, three days after the MOMS38 launch, so it is early in the wave rather than independent of it.

- snippet: Insurance companies LOVEEEEE to take money from people YET will do everything they can to not pay out for stuff that its suppose to cover. Nightmare and mind blowing how they play games  and give the big run around.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad OMC - C11 - 2b
    review_id: 59d80f5f-496d-7d55-08c2-1492fca4c32d
    date: 2026-03-19
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-19
  last_seen: 2026-03-19
  confidence: thin
  brand_self_echo: false
  notes: Thin at one record. Kept because it is the only place in the corpus where the pain is named as an adversary doing something to her on purpose rather than as a number that is too big. "they play games and give the big run around" is the usable half. It sits on a different creative, OMC - C11 - 2b, which is one of the few pain records outside the MOMS38 family. The double space before "and" is in the original and is preserved.

- snippet: I literally was just on the phone for hours today figuring out something eith insurance...and still no answer.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 2 - V1
    review_id: 622cb438-d58d-9f87-f722-59a7c197eccf
    date: 2026-04-04
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-04
  last_seen: 2026-04-04
  confidence: thin
  brand_self_echo: false
  notes: The time cost rather than the money cost, and the corpus has almost none of it. Kept because of where it sits. This is on MOMS38 - 2 - V1, the skit creative where one woman plays both the mom and the claims rep, which is the one creative family in the whole account that draws agreement instead of argument. So this is a person answering a piece of creative that named her experience rather than her bill. The typo "eith" is preserved.

- snippet: girl, we pay $2,200 a month and its a battle for them to cover anything. I have MS so I NEED to be covered for my treatments
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: cf52967d-33bb-3f5d-ed9d-138895e40607
    date: 2026-03-23
    url: null
  recurrence: 7 for the string "cover anything", roughly 20 for the chronic-condition family
  source_diversity: [ad-comment]
  first_seen: 2026-03-23
  last_seen: 2026-05-26
  confidence: mixed
  brand_self_echo: false
  notes: Carries 4 likes. "its a battle for them to cover anything" is the phrase, and "battle" is the closest thing to a metaphor the pain language in this corpus offers, which the mining method flags as one of the two highest-value signals most passes miss. The chronic-condition family is small by count and the loudest by intensity, and the persona method is explicit that volume and intensity are two separate rankings that must not be flattened.

- snippet: so by December just hit it...oh but its Jan. Now so it starts over...and they still never cover anything.... insurance is the biggest scam 😒
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: b74814f1-85d4-8eec-8ccb-8f62e9df0b1f
    date: 2026-03-24
    url: null
  recurrence: 5 for the reset family, 45 for the scam word
  source_diversity: [ad-comment]
  first_seen: 2026-03-24
  last_seen: 2026-05-13
  confidence: mixed
  brand_self_echo: false
  notes: The reset pain told by someone with a medical reason to hit it every year. The full record says she pays 16,000 before anything is covered, her husband pays over 300 a week, and she is in cancer remission needing CT scans every six months. The run-on punctuation is the rhythm of the pain and should not be cleaned up if this is lifted. Echo on the word "scam" is mixed per the standing verdict, and the surrounding sentence is unmistakably hers.

- snippet: Don’t bother looking into it if you’re diabetic . I’ll be uninsured until I die.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 01b5ff6d-1ea1-b12f-fe1f-136348d8c40b
    date: 2025-08-14
    url: null
  recurrence: 2
  source_diversity: [ad-comment]
  first_seen: 2025-08-14
  last_seen: 2026-04-03
  confidence: thin
  brand_self_echo: false
  notes: Thin, and the reason it is here is the reason the whole doc exists. "uninsured" appears in only 2 of 1,322 comments, or 0.15%, and this is one of the two. So the single most quotable line about being uninsured in this entire corpus is also proof of how rare that state is here. Note the first clause is an objection to this brand's underwriting and belongs to the objection pass. Only the second sentence is the pain, and it is the pain of the category as she expects to live it, not of this product.

- snippet: There is no middle class on the marketplace unfortunately. You either pay next to nothing or almost all of it with no subsidy.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 8a885e35-71be-e442-a0da-f462b6eb3e9f
    date: 2025-08-09
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-08-09
  last_seen: 2025-08-09
  confidence: thin
  brand_self_echo: false
  notes: One record, from 2025, so it is thin and historical. Kept because it explains the money pain rather than just reporting it, and because it names a structural gap that the brand's own stated persona Courtney sits inside. It is also useful as era evidence, since it predates the MOMS38 creative by seven months and shows the cost grief was live before this campaign lit it up.

- snippet: I’m self employed and can’t find anything that doesn’t have at least $5k deductible
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS39 - 2 - V2 and MOMS39 - 2 - V2 - Copy
    review_id: 2c7f384f-cae6-a020-456c-e5534a427218
    date: 2026-04-02
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-02
  last_seen: 2026-04-02
  confidence: thin
  brand_self_echo: false
  notes: Carries 7 likes, which is high for a record this quiet. Thin on count. The string "self employed" returns only 2 records and the other is a rival agent's sales pitch, so this is the only genuine instance. It is kept because it is the one snippet in this doc that lines up with a persona the brand has already stated, and the persona method says corroborating a stated persona is a different and useful result from surfacing a new one.

- snippet: I pay $400 a month, my deductible is 13,000 I make 12700 in a year on disability. Cuz this makes sense.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 6510e12d-3ac0-df2d-1b6b-af541fcbb690
    date: 2026-04-08
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-08
  last_seen: 2026-04-08
  confidence: thin
  brand_self_echo: false
  notes: One record, and it holds the most arresting number relationship in the corpus. Her deductible of 13,000 is larger than her annual income of 12,700. The sarcasm at the end, "Cuz this makes sense," is doing the emotional work. Flag for the claims-check governor before any use, since the figures are self-reported by an anonymous commenter and cannot be verified.

- snippet: shoot im just trying to figure out on how to pay the monthly charges to get health insurance let alone the charges they dont cover with copays its annoying when im barely making it
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS39 - 2 - V2 and MOMS39 - 2 - V2 - Copy
    review_id: aaefb729-af45-6ee5-6dd0-c9017487a6bc
    date: 2026-03-22
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-22
  last_seen: 2026-03-22
  confidence: thin
  brand_self_echo: false
  notes: Thin at one record. "im barely making it" is the phrase, and it is the only line in the corpus that names the household's overall financial state rather than an insurance figure. Voice-check flag. The all-lowercase, unpunctuated register will not survive a lift into brand copy as written, so treat it as transformable rather than in-voice per the mining method's governor.

- snippet: Except the premium for that policy costs more than my house note. Who can afford that? If you get a lower premium then your deductible is much higher and no one can afford the higher deductible so either way people are screwed. Broken system
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS33 - N3 - V2
    review_id: dc090fc7-be0b-3156-eaaa-efcdc96f62c6
    date: 2026-02-14
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-02-14
  last_seen: 2026-02-14
  confidence: mixed
  brand_self_echo: false
  notes: Marked mixed rather than thin on era value. It is dated 2026-02-14, twenty-four days before the MOMS38 family launched, and it is one of only 5 comments in the whole corpus that use the word "deductible" before that launch. So it is the cleanest single proof that the cost pain is the customer's own and not something the ad taught her. It also carries the corpus's best comparison, "costs more than my house note," and its best two-word summary, "Broken system." The trap it describes, where a lower premium buys a higher deductible, is the exact bind the brand's offer claims to solve and the creative never names it.

- snippet: It doesn't make sense. It's never made sense.
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad Moms43 - 5 - V1
    review_id: f1f160d4-9962-e98e-eece-5b9bde1234e2
    date: 2026-09-03
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-09-03
  last_seen: 2026-09-03
  confidence: thin
  brand_self_echo: false
  notes: One record, and it is the single newest record in the corpus, dated the same day the pulls ran. Kept for freshness rather than for weight. The corpus holds only 86 comments since 2026-07-01 and most of them are the single word "Help" under one ad, so pain language in the current era is nearly absent. This is the live end of the bank. It sits on Moms43 - 5 - V1, not on the MOMS38 family, which makes it evidence that the pain persists even where the creative has stopped naming a number.

- snippet: I need insurance I don’t have to pay
  category: pain_phrase
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad Moms43 - 4 - V3
    review_id: 1693a793-1dcb-5945-d2e6-958e69a70fd3
    date: 2026-08-26
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-08-26
  last_seen: 2026-08-26
  confidence: thin
  brand_self_echo: false
  notes: One record, thin, and kept for the same freshness reason. It is the shortest statement of the paying-twice pain in the corpus and the only one from the current era. Note it points at a want rather than only at a hurt, so a reader could reasonably route it to the aspirational pass instead. It stays here because the sentence is built on the present grievance of paying, not on a future self.

## What this set does not cover

Three kinds of language kept turning up and were deliberately left out, so the assembly pass knows they were seen and routed rather than missed.

**Objections to this product went to the objection pass.** The pregnancy exclusion, at 42 comments across 15 ads, and the pre-existing condition denial, at 55 comments across 17 ads, are the two widest recurring complaints in the corpus. They are objections to what this brand's offer does, not the customer's language for the problem she had before it. The one exception is the second sentence of the diabetic record above, where the phrasing describes a lived state rather than a product rule. Both counts are quoted from `source-pulls/ad-comments.md`; a stricter independent re-derivation in `personas/voice-of-customer/voc-objection.md`, run on the same 1,322-row corpus the same day, returns 36 and 42 instead of 42 and 55 because it drops rows that mention pregnancy or a condition while describing the commenter's own existing plan, and the ad spreads, 15 and 17, agree exactly — both are kept visible here because the gap is a classification choice, not a data conflict.

**Corrections of the ad went nowhere in this pass.** 103 comments across 13 ads argue that the ad is using the word deductible when it means out-of-pocket maximum. That is a credibility problem and a category-fluency signal. It is not a pain phrase, because the pain in those comments is with the ad rather than with the customer's life.

**Recognition of the skit creative is an outcome-adjacent signal, not a pain phrase.** The lines on the MOMS38 - 2 family, such as "TRUTH! A SAD TRUTH." and "Absolutely accurate," name that the ad got it right. Only one of them, the phone-call record captured above, names the underlying pain in the commenter's own words, so only that one is here.

## Open loops

Five loops came out of this pass. Every one of them came from the counting work here rather than from the upstream docs, and none of them repeats a loop already filed in `voc-corpus-profile.md` or `source-pulls/ad-comments.md`. The missing reviews, the missing surveys and the missing Reddit pull are infrastructure gaps and are routed to the `data_limitations` field above rather than written as loops, per the rubric.

**1. The audience answers any number an insurance ad puts on screen by naming a bigger one.**

The ad states $6,000. 82 comments answer with "mine is," 76 of them with a specific figure, and 64 of those, or 84%, name a number higher than $6,000. That behavior is not new to this creative. On 2025-07-28, under a different ad naming a $600 premium, a commenter wrote "600? Try 1000+, then this ad would be more realistic."

Pull: **Pattern.** The same reflex shows up under two unrelated creatives, eight months and two different numbers apart, which is what turned a single vivid thread into a question about how this audience reads numbers at all.

Question: What does this audience do with a specific dollar figure in an ad?

Why it matters: the whole account leads with a number. If a stated figure reliably invites a bigger one, then the brand's central creative device is handing the comment section a reason to disqualify the offer as unrealistic before anyone clicks. Knowing this would change whether the next round leads with a number, a range, or no figure at all.

Territory: **Messaging.**

**2. Almost every word of pain this brand has ever heard arrived in one 83-day window.**

Of the 207 comments containing "deductible," only 5 predate 2026-03-10, the day the MOMS38 family launched, and only 5 came after 2026-06-01. So 197 of 207, or 95.2%, land inside 83 days. Since 2026-07-01 the corpus holds 86 comments and most are the single word "Help."

Pull: **Surprise.** For a brand advertising since at least January 2025, finding that 95% of its customer pain language sits inside a single spring window is not what the setup would predict, and the size of that gap is the signal.

Question: What is different about the creative running now that the audience no longer tells it anything?

Why it matters: comment sections are this brand's only source of customer language, and they have gone quiet. If the current creative simply does not invite disclosure, the brand is losing its one listening post while still spending. That is a research pipeline problem dressed as a creative choice.

Territory: **Messaging.**

**3. The word "uninsured" appears twice in 1,322 comments.**

"deductible" appears 207 times, "premium" 46 times, and "uninsured" twice, or 0.15%. The people showing up are not without coverage. They are paying for coverage that does not function.

Pull: **Gap.** The absence is the whole finding. An entire category of buyer the offer is presumably built for leaves almost no trace in the only customer-language source the brand has.

Question: Is the buyer the woman who already pays for coverage she cannot use?

Why it matters: this is the persona question the account cannot currently answer, and it routes everything downstream. If the buyer is the insured and broke woman, then the offer, the proof and the whole message have to speak to someone who already pays every month and is being asked to switch, which is a completely different sell from signing up someone with nothing.

Territory: **Personas.**

**4. She says she cannot switch, and one commenter has to tell her she can.**

24 comments mention an employer, and the ones I read say plainly that the job picks the plan. One from 2026-08-16 reads "If your job offers insurance you have to pick an insurance. They make you pay for one." This family is also the most durable in the corpus, running from March through August while everything else went quiet after May.

Pull: **Tension.** The ad assumes the viewer can shop, and a recurring group of viewers says she is not allowed to, and both cannot be true for the same person.

Question: How many of the women this account reaches actually have the freedom to change their plan?

Why it matters: if a real share of the audience is locked into an employer plan, then part of the spend is buying attention from people who cannot act no matter how good the offer is. Knowing the size of that share would change targeting, and it would tell the brand whether a message naming the employer trap is a new lane or a niche.

Territory: **Personas.**

**5. The one creative that got agreement never mentioned a number.**

Nearly all the recognition in this corpus sits on the MOMS38 - 2 skit family, where one woman plays both the frustrated mom and the claims rep denying a claim over a hallway. The one pain phrase I found on that family names time and exhaustion rather than money: "I literally was just on the phone for hours today figuring out something eith insurance...and still no answer."

Pull: **Resonance.** The comments under that skit read completely differently from the comments under everything else in the account, and I want to know what that creative is doing that the rest is not.

Question: What is the pain that this audience recognizes without being shown a price?

Why it matters: the account's whole pain vocabulary is financial, and the only creative earning agreement instead of argument is the one that dramatizes an experience rather than a bill. If the recognizable pain is the fight and the phone call rather than the deductible, the brand has a second messaging lane it has barely used.

Territory: **Messaging.**

## Sources

- Parker MCP `search_facebook_ad_comments_sql`, 18 filtered pulls on 2026-09-03. Every count in this doc and every row id.
- Parker MCP `search_facebook_ad_comments_semantic`, four themed passes on 2026-09-03. Surfaced the pain families that no single keyword would have found.
- Parker MCP `search_customer_reviews_sql` and `semantic_search_post_purchase_survey`, 2026-09-03. Both zero, checked live.
- Parker MCP `search_facebook_ads_sql` with the scripts block, 2026-09-03. The MOMS38 transcripts and lifetime metrics behind every claim about what the ad says.
- `personas/voice-of-customer/voc-corpus-profile.md`. The denominators, field coverage and limits this pass inherits.
- `source-pulls/ad-comments.md`. The full-corpus persona read whose deductible pattern this pass re-derived independently.
- `source-pulls/brand-self-echo-detection.md`. The standing echo verdicts honored on every snippet.
- `running-notes/missing-context.md` and `running-notes/brand-rules.md`. The dark-surface substitution rule and the standing constraints.
- `parker-system/creative-strategy-context/customer-review-mining-method.md`. The three-way hunt, the qualifying signals, the exclusion list, the claims-check and voice-check governors, era tagging, the denominator discipline and the ten-record bar.
- `parker-system/creative-strategy-context/persona-research-and-creative-strategy-process.md`. The evidence ranking that caps this brand at mixed, the served-versus-buyer distinction, and the rule that volume and emotional intensity stay two separate rankings.
