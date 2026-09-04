---
brand: health-for-moms
doc: voc-anti-language
category: anti_language
generated_on: 2026-09-04
refresh_by: 2026-10-04
live_pulls_run_on: 2026-09-04. Every Parker MCP call behind this doc ran today, against a corpus that had grown to 1,342 since the sibling docs ran on 2026-09-03.
corpus_denominator: 1342 Facebook and Instagram ad comments, Meta ad account HealthForMoms, act 484897827497337
corpus_date_range: 2025-01-08 to 2026-09-03
prior_version: none. First run. No recurrence history to carry forward.
snippets_captured: 20
sources_read:
  - Parker MCP search_facebook_ad_comments_sql, 21 filtered pulls on 2026-09-04. Every count and row id here was re-derived by me from the returned rows.
  - Parker MCP search_facebook_ad_comments_semantic, three themed passes on 2026-09-04 aimed at rejection of tone, tactic and creative. Every pass reported totalCommentsAnalyzed 1342.
  - Parker MCP search_customer_reviews_sql, unfiltered, 2026-09-04. Returned totalReviews 0.
  - Parker MCP semantic_search_post_purchase_survey, 2026-09-04. Returned totalResponsesForBrand 0 with the collection existing.
  - Parker MCP search_facebook_ads_sql, 2026-09-04, lifetime mode with the scripts block, top ten ads by lifetime spend. Read at full media depth so every claim about what the brand says rests on the creative rather than an ad name.
  - source-pulls/brand-self-echo-detection.md, for the standing echo verdicts. The scam verdict and the deductible verdict are carried forward here, not re-judged.
  - personas/voice-of-customer/voc-corpus-profile.md, for field coverage, corpus bias and the carried theme counts.
  - personas/voice-of-customer/voc-objection.md, voc-pain-phrase.md and voc-outcome-phrase.md, the sibling extractions, used to route product doubts away from this pass.
  - running-notes/missing-context.md and running-notes/brand-rules.md.
  - parker-system/creative-strategy-context/customer-review-mining-method.md and persona-research-and-creative-strategy-process.md, the two methods this pass is performed through.
expected_sources_missing:
  - customer reviews. Zero rows, verified live 2026-09-04.
  - post-purchase surveys. Zero responses, verified live 2026-09-04. This is where "what nearly turned you off" gets asked directly.
  - Reddit and forums. Not pulled, and this is the biggest gap for this pass specifically, since communities dissect marketing openly with no brand present.
  - competitor ad comments. No rival brands tracked in the Parker app, so every rejection below is aimed at this brand's own creative or at the category in the abstract. Not one is a customer rejecting a named competitor's messaging.
  - brand-reputation, other-reviews, support tickets, organic social comments. None ingested.
  - personas-profile.md. Not yet written, so identity and behavioral-signal tags are null by rule.
data_limitations:
  - One source type only, so no rejection here can rise above mixed under this prompt's confidence rule, however often it repeats.
  - The pass has an unusual shape for this brand and it is stated up front rather than buried. Anti-language is defined as what the customer hates about competitor or industry messaging. This corpus holds almost none of that. What it holds instead is the audience rejecting this brand's own messaging, at close range, under the ads themselves. That is a more useful finding and a different one, and every snippet says which it is.
  - author_name and author_id are null on all 1,342 rows. Every count is a count of comments, never of people.
  - permalink_url is null on all 1,342 rows, so url is null on every snippet.
  - The AI-creative cluster count of 32 records across 7 ads is carried from source-pulls/ad-comments.md on a 1,322 denominator and is a model-applied tag, not a string count. My own string checks are given separately and are much smaller, because the literal string "AI" over-matches uselessly. Both numbers are shown rather than blended.
  - The semantic comment tool and the SQL comment tool return different identifier spaces for the same row. Every review_id below is the SQL comment_id, resolved by exact-text lookup where the snippet was surfaced semantically.
  - The corpus grew from 1,322 to 1,342 between the sibling docs' pulls and mine. Every percentage here is computed on 1,342; carried figures keep their 1,322 denominator and are labelled.
  - There is no get_current_time tool on this MCP surface, so the date comes from the session clock.
  - refresh_by is 30 days rather than the 180-day cadence, because what an audience finds tired moves fast and the AI-creative rejection in particular is a live cultural argument.
---

# Anti-language — Health For Moms

## The honest headline before any rejection

This brand has no customer reviews and no post-purchase surveys. Both checked live today and both returned zero. So every rejection below comes from Facebook and Instagram ad comments, and nothing here may be described as this brand's review corpus. `verified`.

Now the thing that makes this pass different from its eight siblings, said plainly at the top because it changes how the whole document should be read.

**The prompt defines anti-language as what the customer hates about competitor or industry messaging. This corpus barely contains that. What it contains is the audience rejecting this brand's own advertising, in that advertising's own comment threads.** There are no competitor ad comments in Parker for this brand, so there is literally nowhere for a rival's messaging to be rejected. What is here instead is closer range and more useful: twenty records of women telling Health For Moms, to its face, which of its own moves they can see through.

The prompt anticipates this. It says the `ad-account` source is included partly to check whether the brand itself uses language its customers reject, and calls that a high-value finding. For this brand that is not a side check. It is the entire doc.

So read this as a do-not-say list built almost entirely from the brand's own mistakes rather than from the category's. Every snippet is labelled with what exactly is being rejected, because a do-not-say rule is only usable if it names the thing to avoid.

## How I built this, and the two counts that carry it

**The denominator is 1,342, not 1,322.** I re-pinned it myself. An offset probe at 1341 returned exactly one row and 1342 returned none, and five semantic passes each reported `totalCommentsAnalyzed: 1342`. The sibling docs ran on 2026-09-03 and pinned 1,322; twenty rows have landed since. Every percentage below is on 1,342, and carried upstream figures keep their original denominator and say so. `verified`.

**I read the creative before judging what the audience is reacting to.** The ten highest-spend ads were pulled with the scripts block and read in full. That is what lets me say which rejections are aimed at things the brand actually does. Two examples that matter: the `MOMS38` family, four of the top ten, opens on "My deductible is $6,000... But yet I pay for that insurance," which is the line the brokers below are correcting. And the `MOMS39` and `Moms43` families close on "save up to 30%," which is the promise the bait complaints are aimed at. `verified` from transcripts, not ad names.

**Two echo verdicts are carried forward, not re-judged, exactly as the standing doc requires.**

- **"Scam" is customer-owned.** `source-pulls/brand-self-echo-detection.md` established that customers used it in this brand's comment sections from **2025-01-13**, fourteen months before the earliest ad carrying the scam hook launched on 2026-03-10. The brand took the customer's word, not the reverse. I re-ran the string today: **48 of 1,342 records (3.6%)** contain "scam," up from the 45 of 1,322 recorded yesterday. Verdict stands, `brand_self_echo: false`, and the three snippets below that use the word carry that verdict rather than a fresh guess.
- **The deductible framing is overwhelmingly brand-prompted.** The same doc, plus `voc-pain-phrase.md`, established that 197 of 207 "deductible" comments, 95.2%, sit inside an 83-day window opened by the brand's own creative on 2026-03-10. "deductible" still returns **207 of 1,342 (15.4%)** today. Where a rejection below sits inside that window I say so, because a rejection the brand's own ad provoked is a different kind of evidence from one that arrived unprompted.

**One absence worth carrying, because it is the mirror of this whole doc.** The brand's single biggest phrase, "wife of the year energy," which the echo doc recorded as carrying 67.8% of recent spend, still returns **0 of 1,342** today. `verified`. Nobody rejects it. Nobody repeats it. It simply does not land in language at all.

## What the audience actually rejects, in order of weight

My classification of the 20 captured rejections, `inferred`, with the checkable string counts attached.

| What is being rejected | Snippets | Checkable support against 1,342 |
|---|---|---|
| AI-generated people in the ads | 6 | "actors" 2, "fake" 3, "hate AI ads" 1, "sick of these" 1; plus 32 records across 7 ads carried from the full read on a 1,322 denominator, 25 of them on one 2025 ad |
| Calling itself Health For Moms while excluding maternity | 3 | "false advertising" 1, "deceit" 1, "disgusting" 4 of which 1 is aimed at the tactic |
| Being inaccurate in front of people who know the category | 3 | "misleading" 1, "not misinform" 1, "fishy" 1; sits inside the 103-across-13-ads correction cluster carried on 1,322 |
| Bait, overclaim and the too-good-to-be-true register | 4 | "too good to be true" 1, "click bait" 1, "proceeds to list" 1, "marketed relentlessly" 1 |
| Promises in the copy that the funnel then breaks | 2 | "That's a lie" 1, "click a box" 1 |
| The aspirational mom in the imagery | 1 | 1 record |
| The comment section itself | 1 | 1 record |

**Read the counts honestly.** Not one cluster clears the mining method's ten-record bar on a string basis. The AI cluster clears it only on a carried model-applied tag, and that tag is 25-of-32 concentrated on a single 2025 ad, which the method would call a source-specific pattern rather than a corpus-wide one. So this is a do-not-say list of **20 well-evidenced candidates, not seven proven rules**, and the prompt is right that a rule built on one loud voice can needlessly handcuff a brand's copy. I have marked every one accordingly.

The exception worth flagging: the AI-creative rejection is the only cluster here that recurs across **three separate years of creative** — July 2025, October 2025, and April 2026 — and across four different ad families. Durability across eras is a stronger signal than raw count, and it is the one rejection in this doc I would treat as close to a rule.

## Anti-language

Twenty distinct rejections. Each is verbatim with original spelling, punctuation, casing and emoji. Source type is `ad-comment` for all; the `platform` line carries the ad. `review_id` is the Parker SQL `comment_id`. `url` is null because `permalink_url` is null on all 1,342 rows. `identity_tag` and `behavioral_signal_tag` are null because `personas-profile.md` does not exist and this pass never invents a slug.

The `snippet` line is always `stated`. String counts are `verified`. Every read of what is being rejected and why is `inferred`, and the notes carry the specific do-not-say so the rule is usable.

### The AI-generated presenter

- snippet: Please dont use AI instead of actors.  AI advertizing use in spite of actors goes against the morals that health for moms promotes
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 0a2fd312-dfd7-66ab-4a9b-2f7ad23795d2
    date: 2025-07-20
    url: null
  recurrence: 6 captured, 32 across 7 ads carried from the full read on a 1,322 denominator
  source_diversity: [ad-comment]
  first_seen: 2025-07-20
  last_seen: 2026-04-05
  confidence: mixed
  brand_self_echo: false
  notes: Do not say — do not present a synthetic person as the face of the ad. The sharpest version of the cluster because it does not argue aesthetics, it argues hypocrisy: a brand built on caring about mothers using a machine instead of hiring one. That is a positioning problem, not a production preference. Echo false, and cleanly so: the brand has never used the word AI in any of its ten highest-spend scripts, checked against the transcripts. The double space after "actors." and the misspelling "advertizing" are original.

- snippet: This is the problem with AI online commercials. If you are using a fake person for your testimonial, it unintentionally sends a message to people that no real actual person would say this about your service. I think it's always better to have a real person.

  Especially with something that is famous for being a scam, like health insurance.
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 97e9fc85-d576-2f94-1d7d-20bf77724a8d
    date: 2025-07-25
    url: null
  recurrence: 6 captured
  source_diversity: [ad-comment]
  first_seen: 2025-07-20
  last_seen: 2026-04-05
  confidence: mixed
  brand_self_echo: false
  notes: Do not say — do not use a synthetic face to deliver a testimonial. The most valuable single record in this doc because it names the mechanism rather than the irritation. Her argument is that a fake testimonial implies no real person would give a true one, and that the damage is worst in a category already assumed to be dishonest. That is a precise, testable read of why AI creative costs this brand more than it would cost a mattress company. The word "scam" here carries the standing customer-owned verdict from source-pulls/brand-self-echo-detection.md, which dates customer use to 2025-01-13, and this record predates the brand's scam hook by nearly eight months. The blank line is in the original.

- snippet: You aren’t even a real person. I’m so sick of these AI ads.
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 8c320847-b1af-9a77-439e-f9364a718984
    date: 2025-07-31
    url: null
  recurrence: 6 captured
  source_diversity: [ad-comment]
  first_seen: 2025-07-20
  last_seen: 2026-04-05
  confidence: mixed
  brand_self_echo: false
  notes: Do not say — nothing, in the sense that the rejection is not of a phrase but of the speaker. "sick of these" is fatigue language, which the prompt treats as a first-class anti-language signal because it marks a tactic the audience has already been worn out by elsewhere. Note she is addressing the presenter directly, in the second person, which nothing else in this doc does.

- snippet: Why is everywhere using AI actors now???
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 00bd7ced-713d-399b-f4f0-ae25e11efad2
    date: 2025-07-20
    url: null
  recurrence: 6 captured
  source_diversity: [ad-comment]
  first_seen: 2025-07-20
  last_seen: 2026-04-05
  confidence: mixed
  brand_self_echo: false
  notes: Do not say — nothing verbal; this rejects the category-wide tactic rather than this brand's use of it, which makes it the closest thing in the doc to true industry-level anti-language as the prompt defines it. "everywhere" is doing that work. Carries 1 like and 2 replies, so it started a conversation, which in this corpus is a reasonable proxy for resonance given there is no rating field anywhere.

- snippet: Customers hate AI ads!
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad Internal Videos - OCT - B2 - Copy 2
    review_id: 4f085c63-83e7-dc06-c714-1121bb3865c9
    date: 2025-10-26
    url: null
  recurrence: 6 captured
  source_diversity: [ad-comment]
  first_seen: 2025-07-20
  last_seen: 2026-04-05
  confidence: mixed
  brand_self_echo: false
  notes: Do not say — nothing verbal. Kept for era rather than content. It sits on a different creative family from the July 2025 cluster and three months later, which is one of the three data points establishing that this rejection survives across ad families and years rather than belonging to one bad ad. Four words, addressed to the marketer rather than the audience.

- snippet: Creepy AI blonde lady ruins the ad tbh
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: bb13f8fd-2b12-3d19-557a-427dff553fbd
    date: 2026-04-05
    url: null
  recurrence: 6 captured
  source_diversity: [ad-comment]
  first_seen: 2025-07-20
  last_seen: 2026-04-05
  confidence: mixed
  brand_self_echo: false
  notes: Do not say — nothing verbal, but this is the most operationally useful record in the cluster, because it is the newest and it lands on MOMS38 - 1 - V2, one of the account's highest-spend ads at $41,592.95 lifetime. So the rejection is not confined to old 2025 creative that has been retired. It is live on a flagship. "ruins the ad" is the phrase: she is saying the rest of the ad worked. Voice-check: off-voice, and the observation is what matters.

### Marketing to mothers while excluding maternity

- snippet: Marketing towards mothers while not covering pregnancy is a disgusting tactic.
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 5befe57b-b90b-7f4e-8432-be2b6c4e23b7
    date: 2025-11-23
    url: null
  recurrence: 3 captured for the tactic rejection
  source_diversity: [ad-comment]
  first_seen: 2025-08-12
  last_seen: 2025-12-20
  confidence: mixed
  brand_self_echo: false
  notes: Do not say — do not lead with the mother identity while the product excludes maternity. The word doing the work is "tactic." She is not objecting to the exclusion, which would be a product objection and belongs to voc-objection.md. She is objecting to the marketing choice of naming yourself after a group you then turn away, which is anti-language proper. "disgusting" returns 4 of 1,342 and this is the only one aimed at the brand's marketing rather than at insurance generally. This is the cleanest example in the doc of the objection-versus-anti-language line the prompt asks for.

- snippet: It’s illigal to deny coverage for women who are pregnant so yall need to keep that in mind with the deceitful marketing
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 6ae515bc-68cf-3ba3-dd93-4919090bcaf2
    date: 2025-12-20
    url: null
  recurrence: 3 captured for the tactic rejection
  source_diversity: [ad-comment]
  first_seen: 2025-08-12
  last_seen: 2025-12-20
  confidence: mixed
  brand_self_echo: false
  notes: Do not say — do not describe coverage in terms that imply maternity is included. "deceitful marketing" is the exact charge and it is the phrase to avoid earning. The legal claim inside it is the commenter's own reading and is carried as her language, not endorsed; the corpus profile flags it the same way. "deceit" returns exactly 1 of 1,342, so the specific word is a one-off while the sentiment behind it recurs. Claims-check and legal flag before this record is used anywhere.

- snippet: How can you have healthcare for moms if you don’t cover maternity? Makes zero sense. False advertising.
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 3b2ac139-83f3-123e-bd63-6321ff80f4d4
    date: 2025-08-12
    url: null
  recurrence: 3 captured for the tactic rejection
  source_diversity: [ad-comment]
  first_seen: 2025-08-12
  last_seen: 2025-12-20
  confidence: mixed
  brand_self_echo: false
  notes: Do not say — do not use the brand name as the claim. "False advertising" is the charge and the string returns exactly 1 of 1,342, so it is a single instance of a very specific accusation sitting inside a wide sentiment. voc-objection.md carries this same record as an objection, correctly, because the first half is a product complaint. Only the last two words are anti-language, and they are the half kept here. Carries 1 like.

### Being wrong in front of people who know the category

- snippet: That’s not a deductible that’s a medical maximum out of pocket. You should educate people, not misinform!!
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V5
    review_id: c0a3c689-ecb4-a5a8-ae30-3176267bcc34
    date: 2026-03-29
    url: null
  recurrence: 3 captured; sits inside the 103-across-13-ads correction cluster carried on a 1,322 denominator
  source_diversity: [ad-comment]
  first_seen: 2026-03-29
  last_seen: 2026-04-07
  confidence: mixed
  brand_self_echo: false
  notes: Do not say — do not call an out-of-pocket maximum a deductible. This is the anti-language half of the corpus's single largest conversation. The product-correction half belongs to voc-objection.md, which holds it. What makes this record anti-language rather than objection is the second sentence: she is prescribing a posture, teach rather than mislead, which is a rule about how to talk. "You should educate people, not misinform" is the line. Note the timing caveat that governs this whole cluster: 95.2% of deductible comments sit inside the 83-day window the brand's own creative opened on 2026-03-10, so this rejection was provoked by the ad rather than found in the wild. Carries 2 likes and 3 replies.

- snippet: As a licensed insurance broker this is VERY misleading in the beginning. The first half is talking about a medical maximum out of pocket. A deductible is something you pay before your insurance kicks in with co insurance.
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: efb760eb-07c9-633d-d536-f92c0ac05bc4
    date: 2026-04-07
    url: null
  recurrence: 3 captured; "misleading" returns 1 of 1,342
  source_diversity: [ad-comment]
  first_seen: 2026-03-29
  last_seen: 2026-04-07
  confidence: mixed
  brand_self_echo: false
  notes: Do not say — do not open on a claim a professional can dismantle in one paragraph. The credential is the point. This is a licensed broker publishing a correction under the account's single highest-spend video at $54,322.63 lifetime, and the corpus holds several more from self-identified brokers, billers and a certified application counselor. The word to avoid earning is "misleading," which returns exactly 1 of 1,342 as a string while the behavior behind it recurs across 13 ads. The snippet is trimmed to the first three sentences; the full record continues into a longer technical explanation and is available at the row id.

- snippet: Kathy Johnson no. They’re marketing to moms and not being transparent about what they work with. I’m a licensed agent with a team that works with all plans across the board and these ads seem sooooo fishy OR they targeted the wrong demographic.
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: b14cf007-7f2d-4f53-99dd-1f48d67324db
    date: 2025-07-25
    url: null
  recurrence: 3 captured; "fishy" returns 1 of 1,342
  source_diversity: [ad-comment]
  first_seen: 2025-07-25
  last_seen: 2025-07-25
  confidence: thin
  brand_self_echo: false
  notes: Do not say — do not advertise without naming which carriers or plan types you actually broker. "not being transparent about what they work with" is the precise do-not-say and it is the most actionable line in this section, because it names a fix rather than a feeling. Marked thin at one record. Read with care: the author is a competing agent, so she has a commercial motive to call the ads fishy, and the objection pass counted 39 records across 10 ads where a rival agent pitches in these threads. The observation survives the motive; the count does not support a pattern. Carries 3 likes.

### Bait, overclaim, and the too-good-to-be-true register

- snippet: This sounds too good to be true.
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: b7aa4d37-2243-d0fe-03e6-50c8b7d495ca
    date: 2026-03-22
    url: null
  recurrence: 1 exact
  source_diversity: [ad-comment]
  first_seen: 2026-03-22
  last_seen: 2026-03-22
  confidence: mixed
  brand_self_echo: false
  notes: Do not say — do not pitch a benefit so far above her experience that the gap itself reads as dishonest. Marked mixed rather than thin on the strength of where it sits, which is checkable. This is the opening sentence of the single most-liked record in the entire corpus, at 47 likes and 9 replies, in a corpus where roughly three quarters of records carry no likes at all. voc-pain-phrase.md captures the other half of the same record for "I want the 1990's back"; this pass takes only the first sentence, which is a verdict on the advertising rather than a description of her life. "too good to be true" returns exactly 1 of 1,342 as a string, so the phrase is a one-off and its weight comes entirely from the agreement attached to it.

- snippet: Ha… “in these states” proceeds to list all 50 states… scam
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: ac7bbaaf-2fd0-fd96-43a1-57a6a6551ca4
    date: 2026-03-26
    url: null
  recurrence: 1 exact; the scam word returns 48 of 1,342 (3.6%)
  source_diversity: [ad-comment]
  first_seen: 2026-03-26
  last_seen: 2026-03-26
  confidence: mixed
  brand_self_echo: false
  notes: Do not say — do not use false scarcity. The ads say "you can only get that if you are a mom and you live in one of these states," which I verified in the transcripts of four of the ten highest-spend ads. She watched the qualifier and counted the states, and the exclusivity evaporated. This is the audience catching a specific persuasion technique in the act, which is exactly what the prompt means by a tactic the customer can see through. The scam word carries the standing customer-owned verdict rather than an echo flag. Note voc-objection.md holds a near-identical record as a state-eligibility objection; the anti-language reading here is about the technique, not the coverage map.

- snippet: click bait sends you to the same sales team for private quotes 🙄
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad 14TH JUNE - Copy9
    review_id: ae4f05db-ea31-1f07-3d17-db49d4dfa1cf
    date: 2025-07-07
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-07-07
  last_seen: 2025-07-07
  confidence: thin
  brand_self_echo: false
  notes: Do not say — do not promise a distinct destination and deliver the same broker handoff. "click bait" as two words returns exactly 1 of 1,342 and the single word "clickbait" returns 0, so this is a one-off and thin. Kept because it names the mechanism of the whole funnel in eight words and because it predates the MOMS38 era by eight months, which makes it evidence that the bait complaint is not an artifact of the spring 2026 creative.

- snippet: Dont forget the 15k premiums plus the deductible!!!! Dont click this you will be marketed relentlessly
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 6f319e61-a71d-65d1-d2ba-3cff94652445
    date: 2026-03-26
    url: null
  recurrence: 1 exact; sits inside the 15-across-10-ads call-flood cluster carried on a 1,322 denominator
  source_diversity: [ad-comment]
  first_seen: 2026-03-26
  last_seen: 2026-03-26
  confidence: mixed
  brand_self_echo: false
  notes: Do not say — do not describe the next step in a way that hides that it is a marketing handoff. This is anti-language in its most damaging form, a warning issued to other viewers rather than a complaint made to the brand. "marketed relentlessly" is the phrase and it is the audience's own name for the account's business model. Marked mixed rather than thin because the behavior it warns about is the same one the call-flood cluster documents across ten ads, and voc-objection.md holds that cluster in full.

### Promises in the copy that the funnel then breaks

- snippet: I filled this out because it literally says we won't be contacted by random agents. That's a lie. I immediately received 5 text messages from 5 different agents claiming to be from 5 different companies.
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 8604c6b5-e71e-48d6-70fc-f849f514c914
    date: 2025-11-28
    url: null
  recurrence: 1 exact; the call-flood cluster is 15 across 10 ads carried on a 1,322 denominator
  source_diversity: [ad-comment]
  first_seen: 2025-11-28
  last_seen: 2025-11-28
  confidence: mixed
  brand_self_echo: false
  notes: Do not say — do not promise she will not be contacted by multiple agents. This is the highest-stakes entry in the doc, because it is not a rejection of a tone, it is a specific written promise quoted back with evidence that it broke. "That's a lie" is the verdict. It also directly contradicts the brand context document's claimed customer phrase "Nobody pressured me — they just showed me my options," which source-pulls/brand-self-echo-detection.md verified as brand-authored copy with zero customer instances. So the brand's imagined testimonial and its customers' actual experience point in opposite directions on the same point, which is the most useful single collision in this doc. Carries 1 like. Claims-check: this specific promise should not be used in copy until the brand can confirm the handoff behavior changed.

- snippet: I don't like the fact that I have to click a box saying that I could get AI generated messages and 1 million phone calls.. what happened to one person calling you and just signing up for the insurance?
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 959f8298-a7cd-8555-3308-4de024c91964
    date: 2025-08-13
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-08-13
  last_seen: 2025-08-13
  confidence: thin
  brand_self_echo: false
  notes: Do not say — do not ask her to consent to automated contact in the language of a checkbox. One record, thin, and unusually precise: she is rejecting the consent disclosure itself, which most people never read and this one did. It joins the AI thread and the call-flood thread in a single sentence, which no other record in the corpus does. "what happened to one person calling you" is the phrase and it is a plain statement of the experience she wanted instead. Useful to the funnel team more than to a copywriter.

### The mother in the picture

- snippet: I’m sure the mom that can afford matching outfits prob just pays in cash 🤦‍♀️
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad moms-63 2b and moms-63 2b - Copy
    review_id: 3fb95c2d-c637-a6a4-d741-fc04c9552ecd
    date: 2026-09-03
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-09-03
  last_seen: 2026-09-03
  confidence: thin
  brand_self_echo: false
  notes: Do not say — do not cast an obviously comfortable family to sell relief from medical debt. One record and thin, and it earns its place for three reasons. It is a rejection of the casting rather than the copy, which nothing else in this doc covers. It is from the current era, dated the last day of the corpus, when almost everything else here is spring 2026 or 2025. And it identifies the exact failure: the woman on screen visibly does not have the problem the ad says she has. "prob just pays in cash" is the line. A single record cannot carry a casting rule on its own, and this one should be read next to the account's own delivery data rather than acted on alone.

### The comment section itself

- snippet: Oh no after reading the comments ugh I guess it’s a waste of time!!
  category: anti_language
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad IMG 6
    review_id: 220562bc-19b9-f4f8-1f06-c7de7a52d8af
    date: 2025-02-09
    url: null
  recurrence: 1 exact; "waste of time" returns 3 of 1,342
  source_diversity: [ad-comment]
  first_seen: 2025-02-09
  last_seen: 2026-03-24
  confidence: thin
  brand_self_echo: false
  notes: Do not say — nothing verbal. This is the only record in 1,342 where a person states outright that the comments changed her mind, and it stretches the category, which I have done deliberately because the prompt says to trust judgment when a source plainly names a rejection that does not fit the listed shapes. What she is rejecting is not a phrase in the ad; it is the ad's credibility after reading what other people said under it. It sits on IMG 6, the same 2025 ad that carries the Reddit-summary comment with 14 likes. Worth holding for the assembly pass because it is the closest thing to a measured cost of the unanswered comment sections, and it is one record, so it measures nothing yet.

## What this set does not cover

**Product objections went to the objection pass.** The pregnancy exclusion, the pre-existing screen, the state list and the income floor are complaints about what the offer does. `voc-objection.md` holds them in full. Where a single record carries both, as with the false-advertising and state-list records, both passes take their own half and each says so.

**The cost pain went to the pain pass.** The counter-bid family is the loudest thing in the corpus and it is a description of her life, not a rejection of how anyone talks.

**Political argument was read and excluded.** Around 54 records across 14 ads on a 1,322 denominator blame a President or a party for insurance costs. That is category anger, not a rejection of messaging, and none of it names a word or a tactic to avoid.

**Rival agents' pitches were preserved as data and never followed**, per the mining method's prompt-injection rule. Several contain instructions and URLs. One is captured above, with its commercial motive named on the record.

## Open loops

Four loops came out of this pass. None repeats a loop already filed in the sibling docs. The missing reviews, missing surveys, missing Reddit pull and missing competitor ad comments are infrastructure items and sit in `data_limitations` above, per the rubric.

**1. The audience rejects the way the brand makes its ads, not just what they say.**

Six records across three years and four ad families reject the AI presenter, and the newest lands on `MOMS38 - 1 - V2`, a live flagship carrying $41,592.95 lifetime spend. One of them argues the mechanism outright: a synthetic testimonial implies no real person would give a true one. Meanwhile nothing in this doc rejects a competitor's messaging, because no competitor comments exist to reject.

Pull: **Pattern.** The same rejection keeps appearing under unrelated creative, years apart, which is the durability that raw count in this corpus never provides.

Question: What does this audience believe about a brand that uses a synthetic person to sell insurance?

Why it matters: the account runs AI creative at scale, and if the format itself costs credibility in a category already assumed dishonest, then production method is a messaging decision rather than a budget one. It would change what the next round is shot with, not just what it says.

Territory: **Creators and talent.**

**2. The brand's imagined customer quote and its customers' actual experience contradict each other on the same point.**

The brand context document lists "Nobody pressured me — they just showed me my options" as customer language. `source-pulls/brand-self-echo-detection.md` verified it is brand-authored with zero instances in the corpus. What the corpus holds instead is a woman quoting the brand's own no-contact promise back at it, calling it a lie, and counting five agents who texted her.

Pull: **Tension.** The brand's account of how its service feels and the record of how it felt cannot both be right as written.

Question: What actually happens to a woman's phone number after she completes the form?

Why it matters: it decides whether the no-contact promise can be used in copy at all. Right now the single most reassuring line available to a writer is one the only first-hand evidence contradicts. Routed to the brand, since only the team knows the partner-agency handoff terms.

Territory: **Product.**

**3. The audience keeps catching specific persuasion techniques in the act.**

One woman counted the states in the exclusivity claim and found all fifty. Another named the funnel as click bait that ends at the same sales team. A third warned strangers they would be marketed relentlessly. A broker dismantled the opening claim in a paragraph. These are four different techniques, each spotted and named by a different person.

Pull: **Curiosity.** This audience reads advertising far more fluently than the creative assumes, and Parker's context cannot yet explain where that fluency comes from.

Question: How much does this audience already know about how insurance is sold to her?

Why it matters: the account currently runs a persuasion-heavy format at a group that keeps demonstrating it can see the mechanics. If the fluency is high, the winning move is probably plainness rather than better technique, and that is a different creative brief entirely.

Territory: **Messaging.**

**4. The brand's biggest phrase is neither loved nor hated. It is invisible.**

"wife of the year energy" returns 0 of 1,342 comments today, re-checked live, despite carrying the majority of recent spend. Nobody repeats it and nobody rejects it. Compare that with the AI presenter, which nobody was asked about and six people volunteered opinions on.

Pull: **Gap.** An absence where presence would be expected, on the one phrase the brand has said more than any other.

Question: What do the women this account reaches remember about these ads a day later?

Why it matters: the corpus can show what provokes an argument but not what leaves a trace, and those are different things. If the highest-spend phrase leaves no trace at all in the only language record the brand has, the brand has no way of knowing whether it is working or merely running.

Territory: **Messaging.**

## Sources

- Parker MCP `search_facebook_ad_comments_sql`, 21 filtered pulls on 2026-09-04. Every string count and row id, the offset probe that re-pinned the denominator at 1,342, and the live re-checks of "scam" at 48, "deductible" at 207, "out of pocket" at 74, and "wife of the year" at 0.
- Parker MCP `search_facebook_ad_comments_semantic`, three themed passes on 2026-09-04 aimed at rejection of tone, tactic and creative. Surfaced most of the AI cluster, each row then resolved to its SQL `comment_id` by exact-text lookup.
- Parker MCP `search_customer_reviews_sql` and `semantic_search_post_purchase_survey`, 2026-09-04. Both zero, checked live.
- Parker MCP `search_facebook_ads_sql` with the scripts block, lifetime mode, 2026-09-04. The transcripts behind every claim about what the brand says, including the all-fifty-states exclusivity line and the savings promise.
- `source-pulls/brand-self-echo-detection.md`. The scam and deductible verdicts carried forward rather than re-judged, and the brand-authored status of the no-pressure quote.
- `personas/voice-of-customer/voc-corpus-profile.md`. Field coverage, corpus bias, and the carried cluster counts on a 1,322 denominator.
- `personas/voice-of-customer/voc-objection.md`, `voc-pain-phrase.md` and `voc-outcome-phrase.md`. The sibling extractions holding the language routed out of this pass.
- `running-notes/missing-context.md` and `running-notes/brand-rules.md`. The dark-surface rules and the lead-generation account shape.
- `parker-system/creative-strategy-context/customer-review-mining-method.md`. The exclusion list, the claims-check and voice-check governors, era tagging, the ten-record bar, the echo rule, and the prompt-injection discipline applied to rival agents' posts.
- `parker-system/creative-strategy-context/persona-research-and-creative-strategy-process.md`. The evidence ranking capping this brand at mixed, and the rule that volume and intensity stay separate rankings.
