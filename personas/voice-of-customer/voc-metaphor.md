---
brand: health-for-moms
doc: voc-metaphor
category: metaphor
generated_on: 2026-09-04
refresh_by: 2026-10-04
live_pulls_run_on: 2026-09-04. Every Parker MCP call behind this doc ran today, against a corpus re-pinned live at 1,342 by my own offset probe. The earliest sibling docs ran on 2026-09-03 against 1,322 and say so; carried figures keep their 1,322 denominator and are labelled.
corpus_denominator: 1342 Facebook and Instagram ad comments, Meta ad account HealthForMoms, act 484897827497337
corpus_date_range: 2025-01-08 to 2026-09-03
prior_version: none. First run. No recurrence history to carry forward.
snippets_captured: 15
alliteration_flags_set: 2
sources_read:
  - Parker MCP search_facebook_ad_comments_sql, 26 filtered pulls on 2026-09-04, including the ten zero-return searches that are the evidence for what this corpus does not reach for. Every count and every row id below was re-derived by me from the returned rows.
  - Parker MCP search_facebook_ad_comments_semantic, three themed passes on 2026-09-04 aimed at comparison, simile and figurative framing. Every pass reported totalCommentsAnalyzed 1342, which agrees with my own offset probe.
  - Parker MCP search_customer_reviews_sql, unfiltered, 2026-09-04. Returned totalReviews 0. Checked live by me, not assumed from a note.
  - Parker MCP semantic_search_post_purchase_survey, 2026-09-04. Returned totalResponsesForBrand 0 with the collection existing.
  - Parker MCP search_facebook_ads_sql, 2026-09-04, lifetime mode with the scripts block, top ten ads by lifetime spend. Read at full media depth, because the brand runs a metaphor of its own and this pass cannot judge echo from an ad name.
  - source-pulls/brand-self-echo-detection.md, for the standing echo verdicts. The scam verdict is carried forward here, not re-judged.
  - personas/voice-of-customer/voc-corpus-profile.md, for field coverage, corpus bias and the carried theme counts.
  - personas/voice-of-customer/voc-pain-phrase.md, voc-objection.md, voc-outcome-phrase.md, voc-trigger-moment.md and voc-anti-language.md, the sibling extractions, used to route literal language away from this pass.
  - running-notes/missing-context.md and running-notes/brand-rules.md.
  - parker-system/creative-strategy-context/customer-review-mining-method.md and persona-research-and-creative-strategy-process.md, the two methods this pass is performed through.
expected_sources_missing:
  - customer reviews. Zero rows, verified live 2026-09-04.
  - post-purchase surveys. Zero responses, verified live 2026-09-04.
  - Reddit and forums. Not pulled, and this is the single biggest gap for this pass. Peer-to-peer explanation runs on analogy, which is exactly what metaphor extraction wants and exactly what a comment section under a paid ad suppresses.
  - competitor and category reviews. No rival brands tracked in the Parker app.
  - brand-reputation, other-reviews, support tickets, organic social comments. None ingested.
  - personas-profile.md. Not yet written, so identity and behavioral-signal tags are null by rule, not by oversight.
data_limitations:
  - One source type only, so no snippet here can rise above mixed under this prompt's confidence rule, however often it repeats. Cross-source recurrence is what earns strong and this brand has one kind of source.
  - This is a thin category and the thinness is a finding rather than a miss. The full argument is in the second section. Ten metaphor families that a health-insurance corpus would be expected to carry returned zero records each.
  - author_name and author_id are null on all 1,342 rows. Every count is a count of comments, never of people.
  - permalink_url is null on all 1,342 rows, so url is null on every snippet.
  - The semantic comment tool and the SQL comment tool return different identifier spaces for the same row. Every review_id below is the SQL comment_id, resolved by exact-text lookup where the snippet was first surfaced semantically. The racquet snippet is the clearest case: the semantic tool returned dc84e8fd for it and the SQL comment_id is dea2d778. A later pass must never paste a semantic id into review_id.
  - The database stores curly apostrophes. A substring search written with a straight apostrophe will silently miss rows. Every search behind this doc was written to avoid apostrophes for that reason.
  - The SQL search is a plain case-insensitive substring match, which I verified rather than assumed. A search for "racket" returns one row whose word is actually "bracket". Word-boundary counts here were hand-checked against the returned rows, not read off the total field.
  - Severe ad skew, and it bites the strongest find in this doc. The luck-and-winning frame sits entirely inside the MOMS38 - 1 creative family. That is argued rather than hidden.
  - refresh_by is 30 days rather than the 180-day voice-of-customer cadence in parker-system/system/refresh-cadence.md, matching the sibling docs. Metaphor is the category most likely to be reshaped the moment a Reddit pull lands, because that is where analogy actually lives.
  - There is no get_current_time tool on this MCP surface, so the date comes from the session clock.
---

# Voice of Customer — metaphors — Health For Moms

## What this pass read, and the one thing to hold before the first quote

This is a hunt for the pictures this customer draws in her head when she tries to make sense of health insurance. The prompt is right that it is the deepest category in the library. An analogy a person reaches for on her own shows the frame she is already using, and copy that lands inside a frame she already accepts does not have to build one.

The reading surface is one thing only: **1,342 Facebook and Instagram ad comments** from Meta ad account `HealthForMoms`, act `484897827497337`, running 2025-01-08 to 2026-09-03. I re-pinned that total myself today with an offset probe rather than carrying it from a sibling doc, and the semantic tool independently reports `totalCommentsAnalyzed 1342` on every pass. `verified`. Customer reviews returned zero rows live today. Post-purchase surveys returned zero responses live today. Reddit, forums, third-party reviews and competitor reviews are not pulled.

That single-source reality sets a hard ceiling that no amount of recurrence can lift. The mining method's rule and this prompt's rule agree: cross-source presence is what turns a striking image into a shared mental model, and **the strongest mark available in this doc is `mixed`**. Nothing below is `strong`, and that is a fact about the corpus, not about the phrases.

One more thing to hold. Not one commenter here is confirmed to have bought anything. The account is lead generation — 39,569 leads lifetime on $743,218.09 of spend at $18.78 each, and zero purchases, because no purchase event exists. `verified` from the lifetime pull I ran today. So these are the images of people the algorithm served, standing outside the product, not the images of people who have used it.

## The shape of metaphor in this corpus, and why the category is thin

The honest headline first: **this audience mostly does not speak in metaphor. It speaks in arithmetic.**

That is not a soft impression. Here is what the corpus reaches for instead. `voc-pain-phrase.md` found 207 of 1,322 comments carrying the word "deductible," and the dominant move in this corpus is a woman answering an ad by posting her own number: $6,000, $8,400, $10,000, $11,000, $15,000, $15,800, $16,000. She does not say the deductible is *like* anything. She says what it is and how much it costs her. The mining method calls specific numbers the top qualifying signal for realness, and by that measure this corpus is unusually rich. By the metaphor measure it is unusually poor, and those two facts are the same fact seen from two sides.

**The zero sweeps, run live today.** I went looking for the metaphor families a health-insurance audience would plausibly reach for. Each of these is a case-insensitive substring search across all 1,342 records, and each returned nothing:

| String searched | Records |
|---|---|
| "gamble" | **0** |
| "ponzi" | **0** |
| "hostage" | **0** |
| "bleed" | **0** |
| "rigged" | **0** |
| "hoops" | **0** |
| "trapped" | **0** |
| "legalized" | **0** |
| "bankrupt" | **0** |
| "racket" (as its own word) | **0** |
| "feels like" | **0** |

That last row is the one that should stop a reader. **"Feels like" — the plainest simile-builder in English — appears zero times in 1,342 comments.** The single near-miss is one woman writing "I feel like," and she uses it to hedge an opinion, not to draw a picture: "I feel like with what you pay between the monthly payment and your deductible you might as well just have no insurance and pay out of pocket?" That is row `a39791c9-fbbb-3c9a-961f-d413c27216c3`, ad `MOMS38 - 1 - V2` family, 2026-05-17. `verified`.

"Bankrupt" returning zero deserves its own line, because the brand's highest-spending ad opens on it. `B1 samar- Copy` — $61,237.93 lifetime, the account's top spender — says at 0:04, "Every three minutes, an American family files for medical bankruptcy even with insurance." `verified` from the transcript. The audience has never once used the word back.

**Why the thinness is structural, `inferred` from three things I can point at.** One, the format. A comment under a paid ad is a short public reply, and the corpus profile measured what that does: most rows are a sentence or two. Metaphor takes room to build. Two, the prompt in front of them. The winning creative opens by naming a number and asking the viewer to react to it, so the audience answers in the same currency it was addressed in. Three, the missing surface. Reddit is where people explain insurance to each other, and explanation between peers is where analogy lives. That pull has been named as available since 2026-09-03 and has never been run.

**So the finding is not "this customer has no mental model."** It is that her mental model is arithmetic, and the few genuine images she does reach for are worth more because they are rare. Fifteen of them are captured below.

## The four images that actually recur

Four frames carry essentially all the real figurative language in this corpus. They are laid out here before the snippets so a reader sees the shape rather than assembling it from a list.

### 1. The category is a crime. The most-used image in the corpus by a distance.

"Scam" appears in **48 of 1,342 records, 3.58%, across 15 distinct ad names**, first on 2025-01-13 and most recently on 2026-09-03. `verified` — I pulled all 48 rows sorted oldest-first and read every one. The sibling echo doc measured 45 of 1,322, 3.4%, on 2026-09-03; the cluster has grown by three records in a day and the share is essentially unchanged.

The word does two different jobs here and the split matters, so I made it and marked it as mine. `inferred`, from reading all 48: roughly two thirds — about 31 records — use "scam" for the whole insurance category, and roughly one third — about 16 — accuse this specific brand of literal fraud. **Only the first group is a metaphor.** Calling a licensed, regulated, legally mandated product a con is a comparison: the customer is likening insurance to a crime she knows it technically is not. The second group is a literal accusation and belongs to `voc-objection.md` and `voc-anti-language.md`, which already hold it.

The tell that the first group is figurative and not a mistake is that the customers say so themselves. Two of them sharpen the word with a qualifier that concedes the legality in the same breath:

- "Health and Car insurance are the biggest **legal scams** that are RDQUIRED to be payed into." — 2026-04-14
- "Insurance is the BIGGEST **forced scam** in the entire world" — 2026-03-30, and this one carries 10 likes, which puts it in the top tier of a corpus where roughly three quarters of rows have none.

"Legal scam" and "forced scam" are the customer doing the strategist's work out loud. She knows it is not a crime. She is telling you it feels like one anyway. That is the metaphor, stated as plainly as a customer ever states one.

Nearby wordings in the same crime frame, each appearing once: **robbery** ("All insurance is a scam and robbery," 2026-04-10), **stealing** ("It is stealing!!!!", 2025-11-27), and **racquet** ("health insurance is a racquet," 2026-03-26 — her spelling, and the only mafia-adjacent word in the whole corpus).

**Echo verdict: false, carried forward, not re-judged.** `source-pulls/brand-self-echo-detection.md` settled this on 2026-09-03 and I am honoring it rather than re-running the argument. Customer use begins 2025-01-13 under the ad `IMG 6`; the earliest brand ad carrying the scam hook is `MOMS38 - 1 - V5`, created 2026-03-10. Fourteen months. The brand took the customer's word, which is the healthy direction.

### 2. The category is a joke. The second-most-used image, and it is the funnier cousin of the first.

"A joke" appears in **8 of 1,342 records, 0.60%, across 6 distinct ads**, first 2025-07-23, last 2026-08-31. `verified`. Same split as scam and I made it the same way: **5 aim at the category or the system, 3 aim at this brand's offer**. `inferred`.

The category-facing ones are a real image with a specific meaning. A joke is something not meant seriously, so calling a $15,000 deductible a joke says the number is too absurd to be a real request. "$15,000 is our deductible for the insurance we can't afford... Insurance is a joke…." carries 4 likes. Another woman does the arithmetic for a full paragraph, ending on "It is a joke all around."

Worth noticing that scam and joke are the same accusation at two temperatures. Scam is angry. Joke is exhausted. The account's creative currently runs on the angry one.

### 3. Your coverage is luck, not a choice. The most useful image here, and the one nobody has done anything with.

This is the find of the pass, and it is not a phrase — it is a frame the audience builds together in the replies.

The word "lucky" or "luck" appears in 14 records. Read in place, **9 of them, 0.67% of 1,342, use luck to describe somebody else's coverage**, and the other 5 are the farewell idiom "good luck" or a job hunt. `verified` by reading all 14. Alongside them sit **2 records using "I win"**. So the frame runs to **11 records across 5 distinct ads**, all inside the `MOMS38 - 1` family, 2026-03-17 to 2026-05-07.

What makes it worth more than its count is where the likes are. In a corpus where most rows have zero:

- "Lucky! Mine is $11,000" — **19 likes, 4 replies**. 2026-03-17.
- "I guess we're lucky our insurance through my husband's employer is free and our deductible is only $400 each" — **11 likes, 7 replies**. 2026-03-29.
- "You are lucky. Mine is over $10k" — **10 likes**. 2026-04-15.
- "I think I win mine is $9000" — 3 likes, **5 replies**. 2026-03-30.

Three of the four highest-liked rows in this whole doc sit in one frame. `verified`.

**The underlying image, `inferred`:** health coverage is a hand you were dealt, not a purchase you made. Under it runs a second move — the comment thread turns into a contest where the *worst* number wins. "I win, we pay $1500 a month and still have $2500 deductible 😞" is that said out loud, sad-face and all. A woman with good coverage is not a smart shopper in this frame, she is a lottery winner, and the correct response to her is congratulations plus your own worse number.

**Why this matters more than the scam cluster.** The brand's entire pitch asks a woman to believe her situation is a choice she can change in thirty seconds. The most engaged image in her own comment section says the opposite: coverage is luck, and the reason yours is bad is that you drew badly. Those two frames do not fit together, and the audience is repeating hers under an ad running his. This is the deepest cross-category agreement in the library — it lines up with the correction cluster in `voc-objection.md`, where commenters keep telling the brand that the terms are not what it says, and with the trigger evidence in `voc-trigger-moment.md`, where the things that actually change a woman's coverage are a job, a state move, or an employer, never a decision she made.

**The honest limit on it.** Eleven records is a candidate, not a movement, and the mining method's bar is explicit that a theme resting on fewer than ten records is a quote candidate rather than a stable pattern. Eleven clears that bar by one. Worse, every record sits in a single creative family, which makes it a source-specific pattern until something outside `MOMS38 - 1` corroborates it. I have marked all three snippets `mixed` and said so in the notes on each.

### 4. The brand's own metaphor, handed back with a knife in it.

The brand has a metaphor. It is "has your back," and it is everywhere: five of the ten highest-spending ads close on "Finally, insurance that actually feels like it has our back," and the top spender opens on "imagine an insurance policy that actually has your back." `verified` from the transcripts I pulled today.

**In 1,342 comments, the phrase "your back" or "our back" appears exactly once.** `verified`. And here it is:

> "I like how it's "insurance that has your back" but apparently there's no plans for someone who's pregnant with type one diabetes. Yeah, totally has my back on the condition that I'm healthy before getting the insurance"

Row `c07a7826-7f12-090e-db52-0b8ff04c4abb`, ad `MOMS38 - 1 - V3`, 2026-04-12, 4 likes and 3 replies.

She quotes the brand's line in quotation marks and then turns it. That is echo — she got the phrase from the ad, there is no question about the direction — but it is the hostile kind, which the assembly pass needs to see rather than have folded into a count. `brand_self_echo: true`, and the snippet is captured for exactly that reason.

This mirrors the finding already standing in the echo doc about "wife of the year energy," the text hook that carried most of the last 90 days of spend and appears zero times in 1,342 comments. The pattern across both, `inferred`: **the brand's coined images do not spread. Its borrowed ones do.** The word it took from the customer, scam, now recurs 48 times. The phrases it wrote for itself recur zero times or once with a knife in it.

## Metaphors

Fifteen snippets. Source type is `ad-comment` on every one, because it is the only source that exists. The `platform` line carries the ad the comment sits under. `review_id` is the Parker SQL `comment_id`, resolved by exact-text lookup wherever a row was first surfaced semantically. `url` is null on all fifteen because `permalink_url` is null on all 1,342 records. `identity_tag` and `behavioral_signal_tag` are null on all fifteen because `personas-profile.md` does not exist yet and this pass never invents a slug.

Every `snippet` line is `stated` and exact. Every count is `verified` as a string check anyone can re-run through the same tool. Every read of what a snippet means is `inferred` and says so. Nothing is `strong`, per the single-source ceiling.

- snippet: Insurance is the BIGGEST forced scam in the entire world
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: 3c25dae8-59c4-b8fe-5911-08d1153d6401
    date: 2026-03-30
    url: null
  recurrence: 48 for the scam cluster, of which roughly 31 use it for the category rather than for this brand
  source_diversity: [ad-comment]
  first_seen: 2025-01-13
  last_seen: 2026-09-03
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  notes: The clearest metaphorical use of scam in the corpus, because "forced" concedes that the thing is legal and mandatory in the same breath that calls it a crime. Denominator is 1,342 and the cluster is 3.58%, spread across 15 distinct ad names, which makes it the widest-spread language this brand owns. Carries 10 likes in a corpus where roughly three quarters of rows carry none. The full comment names her own situation first, which is why it reads as felt rather than performed - she works in special education and her last check was $2.64 after family premiums. Echo verdict carried forward from source-pulls/brand-self-echo-detection.md, not re-judged: customer use begins 2025-01-13, fourteen months before the earliest brand ad carrying the scam hook. Claims-check clear, since it describes the category rather than this product. Voice-check off-voice as written - the brand guidelines forbid scare tactics - but the observation is fully usable at a lower temperature.

- snippet: Health and Car insurance are the biggest legal scams that are RDQUIRED to be payed into. Nobody benefits from either except the insurance providers
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: 85ad24c4-1ffa-c22c-da1c-617049382bcf
    date: 2026-04-14
    url: null
  recurrence: 1 exact, 2 for the qualified-scam wording that concedes legality
  source_diversity: [ad-comment]
  first_seen: 2026-03-30
  last_seen: 2026-04-14
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  notes: Same underlying image as the snippet above and captured separately because the wording is the more precise one. "Legal scam" is the customer naming the exact shape of her grievance: not that anyone broke a law, but that the law permits this. Typo preserved verbatim. The second half is a separate and reusable idea - that the only party the arrangement serves is the seller - which the brand could speak to directly since it positions itself against big insurance. Claims-check clear as a category read. Denominator 1,342.

- snippet: All insurance is a scam and robbery but a high DED and OPM  with high coinsurance rates is absolutely outrageous. You are better off being self pay and asking for selfpay pricing than using insurance.
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: e8dab1a2-dfb3-1d0d-9026-2342a40768de
    date: 2026-04-10
    url: null
  recurrence: 1 for "robbery" in the whole corpus
  source_diversity: [ad-comment]
  first_seen: 2026-04-10
  last_seen: 2026-04-10
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  notes: The only appearance of "robbery" in 1,342 records, verified by substring search. Captured because it sits at the sharpest end of the crime frame and because the speaker is plainly fluent - she uses DED and OPM as abbreviations without explaining them, which voc-category-jargon.md picks up separately. Double spacing preserved verbatim. The recommendation at the end, that self-pay beats insurance, is the same exit-the-category move that voc-objection.md tracks as a cluster. Marked mixed rather than thin because the image it belongs to is the corpus-wide crime frame rather than a lone flourish, though the exact word appears once.

- snippet: Lol!!! Sooooo......health insurance is a racquet.
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V10
    review_id: dea2d778-1d23-a7c4-a4b1-43c79be3f9ed
    date: 2026-03-26
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-26
  last_seen: 2026-03-26
  confidence: thin
  brand_self_echo: false
  alliteration: false
  notes: Her spelling, kept exactly. The word she means is racket, the organized-crime sense, and a substring search for "racket" returns zero real instances - the one row it matches contains "bracket" - so this is the only mafia-flavored image in the corpus. Thin because one record is a candidate, not a pattern. Snippet is trimmed to the metaphor itself; the rest of her comment describes refusing to pay medical bills because she knows the industry loopholes, which belongs to the objection and jargon passes rather than here. This is also the clearest case of the identifier trap in this doc: the semantic tool returned dc84e8fd for this row and the SQL comment_id is dea2d778.

- snippet: $15,000 is our deductible for the insurance we can’t afford... Insurance is a joke….
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V5
    review_id: 800d9f1a-cbb6-e7af-963c-93ee3e5eed4b
    date: 2026-03-31
    url: null
  recurrence: 8 for "a joke", of which 5 aim at the category and 3 at this brand's offer
  source_diversity: [ad-comment]
  first_seen: 2025-07-23
  last_seen: 2026-08-31
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  notes: The cleanest example of the joke frame, and it shows the frame's grammar - a number first, then the verdict. Calling something a joke says it is not a serious request, which is a different accusation from scam: scam is angry, joke is exhausted. Carries 4 likes. Denominator 1,342, so the joke cluster is 0.60% against the scam cluster's 3.58%. Curly apostrophes and the four-dot ellipsis preserved as stored. Claims-check clear. Voice-check transformable - the observation lands, the wording is flatter than the brand's register.

- snippet: I have a $6k deductible and my out of pocket maximum is $15k 😂 my kid and I are on a plan that is $645 a month. I still pay full price for everything all year until I pay $6k which has been never. They have never helped me pay for anything, but I give them thousands a year for what? Once I pay the $6k, they pay a portion and I STILL have to pay lmao. It’s a joke all around.
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V5
    review_id: be59e705-66a5-1215-96a0-bdd826f0f68c
    date: 2026-04-08
    url: null
  recurrence: 8 for "a joke", 5 in the category sense
  source_diversity: [ad-comment]
  first_seen: 2025-07-23
  last_seen: 2026-08-31
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  notes: Kept whole rather than trimmed, because the structure is the asset and the mining method flags exactly this shape as a whole-review concept candidate: four specific numbers, a rhetorical question in the middle, and the image only at the end. "Which has been never" is the sharpest line in it - she has never once reached her own deductible. The metaphor is the last sentence; everything before it is the arithmetic that earns it. This is the single best raw material in the corpus for a script that does not have to invent anything.

- snippet: Lucky! Mine is $11,000
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: aa3d6d52-d3a5-63ad-78bb-570b4939eb59
    date: 2026-03-17
    url: null
  recurrence: 11 for the luck-and-winning frame, 9 of them using luck for someone else's coverage
  source_diversity: [ad-comment]
  first_seen: 2026-03-17
  last_seen: 2026-05-07
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  notes: Six words, and the highest-engagement row in this whole doc at 19 likes and 4 replies. The image is implied rather than spelled out, which this prompt explicitly allows: coverage is a hand you were dealt. Calling another woman lucky for having a $6,000 deductible reframes the entire category as chance rather than choice, and it is the exact opposite of what the ad above it is arguing. Denominator 1,342, so 0.67% for the luck half alone. The honest limit is that all 11 records sit inside the MOMS38 - 1 creative family, so this is a source-specific pattern until something outside that family corroborates it. Claims-check clear. Voice-check in-voice - it is short, warm and unpolished, which is the register the brand says it wants.

- snippet: I think I win mine is $9000
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V8
    review_id: d7812c81-61d4-be87-5b79-dd0914a0ea7e
    date: 2026-03-30
    url: null
  recurrence: 2 exact for "I win", 11 for the wider luck-and-winning frame
  source_diversity: [ad-comment]
  first_seen: 2026-03-30
  last_seen: 2026-04-09
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  notes: The contest half of the same frame, and the more revealing half. She is treating the comment thread as a competition in which the worst deductible wins, which is a real image and a strange one: the prize for winning is that your life is worse. Carries 3 likes and drew 5 replies, so it did what a contest does - it pulled other people in to top it. Shares its underlying image with the two luck snippets and with the "I win" snippet below; a writer may want this specific wording while the assembly pass needs to know the image recurs 11 times.

- snippet: I win, we pay $1500 a month and still have $2500 deductible 😞
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V8
    review_id: 8e64382e-a644-c112-a9e4-220c94726675
    date: 2026-04-09
    url: null
  recurrence: 2 exact for "I win", 11 for the wider frame
  source_diversity: [ad-comment]
  first_seen: 2026-03-30
  last_seen: 2026-04-09
  confidence: mixed
  brand_self_echo: false
  alliteration: false
  notes: The same contest image with the emotion left visible. "I win" and a sad face in the same eleven words is the whole frame compressed: she is claiming a victory she does not want. Second of the two exact uses. Captured separately from the snippet above because the wording carries something the other does not, which is the tone break at the end.

- snippet: I like how it’s "insurance that has your back" but apparently there’s no plans for someone who’s pregnant with type one diabetes. Yeah, totally has my back on the condition that I’m healthy before getting the insurance
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: c07a7826-7f12-090e-db52-0b8ff04c4abb
    date: 2026-04-12
    url: null
  recurrence: 1, and it is the only appearance of "your back" or "our back" in 1,342 records
  source_diversity: [ad-comment]
  first_seen: 2026-04-12
  last_seen: 2026-04-12
  confidence: thin
  brand_self_echo: true
  alliteration: false
  notes: Echo true, and the direction is not in doubt - she puts the brand's line in quotation marks before turning it. The brand's metaphor is "has your back" and it closes five of the ten highest-spending ads, verified from the transcripts, including "Finally, insurance that actually feels like it has our back" and, on the top spender B1 samar- Copy, "imagine an insurance policy that actually has your back." Against that volume the phrase comes back exactly once in customer language, sarcastically, from a woman who was excluded. Captured rather than discarded because the assembly pass needs to see hostile echo as its own thing rather than as a count. Carries 4 likes and 3 replies. Claims-check: this snippet is evidence against the has-your-back claim as currently written, and it should route to the claims-check governor as a live risk on the account's most repeated line. Not liftable in any form.

- snippet: We’re health poor, house poor, vehicle poor, Walmart addicted, stuck in a rut people.
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 0bb56fef-8bb4-8bf6-1cce-06a292d0bb80
    date: 2025-07-23
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-07-23
  last_seen: 2025-07-23
  confidence: thin
  brand_self_echo: false
  alliteration: true
  notes: The best-written sentence in 1,342 records and the reason this pass sets an alliteration flag at all. "Health poor, house poor" is a genuine alliterative pair, and the escalating list is a customer doing copywriting in her own words - she takes an existing phrase, house poor, and extends it into a whole identity. "Stuck in a rut" is the metaphor proper. One record, so thin, and it must never be presented as a pattern. Its value is as a single voice, not a movement. Claims-check clear as customer self-description. Voice-check off-voice - the brand cannot call its own audience Walmart addicted - but the health-poor construction is transformable and is the strongest candidate in this doc for a headline.

- snippet: It’s not insurance, yet they pass it off as if it is. Buyer beware!
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: a69e2ffe-d4f2-cd89-49ef-b130b136cb2b
    date: 2025-07-29
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-07-29
  last_seen: 2025-07-29
  confidence: thin
  brand_self_echo: false
  alliteration: true
  notes: Captured for the alliteration flag more than for the image. "Buyer beware" is a stock phrase rather than an invented one, but the phonetic pair is real and the mining method treats alliteration as one of the two highest-priority signals most passes miss. This is aimed at this brand rather than the category, so its argumentative content belongs to voc-anti-language.md and voc-objection.md, which hold it; only the phrasing is captured here. Thin, and one record. Claims-check unusable as written - it is an accusation against the brand.

- snippet: Insurance companies LOVEEEEE to take money from people YET will do everything they can to not pay out for stuff that its suppose to cover. Nightmare and mind blowing how they play games  and give the big run around.
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad OMC - C11 - 2b
    review_id: 59d80f5f-496d-7d55-08c2-1492fca4c32d
    date: 2026-03-19
    url: null
  recurrence: 1 for "play games", 1 for "run around", 1 for "nightmare" - all three appear only in this single record
  source_diversity: [ad-comment]
  first_seen: 2026-03-19
  last_seen: 2026-03-19
  confidence: thin
  brand_self_echo: false
  alliteration: false
  notes: Three separate images stacked in one comment, which is why it is captured whole. The game frame says the insurer is playing while she is not; the run-around says the process is designed to exhaust her; nightmare says the whole thing has the logic of a bad dream. Each returns exactly one record across 1,342 in its own substring search, verified, so none is a pattern and the stack is one person being unusually vivid. Sits on a different creative family from the luck frame, which is worth noting since almost nothing else here does. Voice-check transformable.

- snippet: Yep but what if you don’t have kids... Just another crack I slip through
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 0998c107-008d-4faf-2a24-995e4ad699f9
    date: 2025-07-28
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-07-28
  last_seen: 2025-07-28
  confidence: thin
  brand_self_echo: false
  alliteration: false
  notes: A real metaphor and an unusually good one - she turns the stock phrase about people falling through the cracks into something she does personally and repeatedly, which is what "another" is doing in that sentence. Aimed at the qualifier that excluded her for not having children, so the exclusion complaint itself belongs to voc-objection.md. Only the image is captured here. One record, thin. Notable that the corpus contains a second, unrelated use of falling through the cracks, in a long comment about Texas school funding, which suggests the image is category-standard rather than invented here.

- snippet: makes me feel like a pile of shit
  category: metaphor
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V9
    review_id: 39142f88-ca24-f10f-ebc6-e0918d2d82b4
    date: 2026-04-04
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-04
  last_seen: 2026-04-04
  confidence: thin
  brand_self_echo: false
  alliteration: false
  notes: The only simile in the corpus that describes the speaker rather than the industry, and it is the emotional low point of 1,342 records. The speaker is a father, which matters twice: this brand advertises to mothers and 96.1% of its lifetime spend delivers to women, so he is off-persona, and the fact that the only self-directed image in the corpus comes from the one demographic the brand is not addressing is a finding rather than a footnote. The whole comment is worth reading in place - spinal fusion, lost the good job with good insurance, back in school, and in the meantime the one racking up medical debt for his family. Snippet is trimmed to the image. Voice-check off-voice, not liftable. The observation - that being the sick one in a family reads to that person as being the burden - is a genuine angle nothing in the account touches.

## Images this corpus contains that are not this brand's metaphors

Recorded so a later pass sees that they were found and correctly routed, rather than assuming they were missed.

- **"a bad diagnosis won't steal everything you and your loved ones have built"** — row `4da1389b-0d84-386d-1dac-89a3a877597a`, ad `MOMS38 - 1 - V3`, 2026-03-25, 1 like. A theft image pointed the other way: here the thief is the illness and insurance is the defense. It is the most eloquent pro-insurance comment in the corpus, written by a woman whose own bills "ended in million." Not captured as a Health For Moms metaphor because it argues against the account's whole premise, and the echo doc already flagged her "peace of mind" phrasing as category-standard rather than lifted.
- **"the overhead paying these people is killing us"** — row `b71b7dfb-45a7-99dd-bada-0f1284f81e60`, ad `Y2 - MOMS25 - 5TH DEC - Copy 6`, 2025-12-08. A real figure of speech, but the target is the layers of middlemen in the insurance market, not a product experience. Left here rather than captured because "killing us" is close to dead as an idiom and one record cannot lift it.
- **"Looks like another dead end."** — row `5ea888ae-0841-4a4b-82f1-1ca8d2d774c5`, ad `B1 samar- Copy`, 2025-08-12. The journey-as-maze image, and it is about this brand's funnel rejecting her. It belongs to `voc-objection.md` as a disqualification record. Noted here because if a Reddit pull ever shows the maze image recurring, this row is where it started in this corpus.
- **"this is def screaming SCAM"** — row `cb20aa0a-116e-fd0b-ce75-ae1df055950b`, ad `B1 samar- Copy`, 2025-10-03, 1 like. Personification, and a vivid one, but the accusation is literal and specific: a rep took her information and ghosted her. That is a service complaint and it lives in the objection and anti-language passes.
- **"These mthfkers are scamming us to our faces and we have to act like it's peachy"** — row `513a4d2e-54fb-21fb-c39c-e10b6cd3a14f`, ad `MOMS38 - 1 - V3`, 2026-04-13, 1 like. "To our faces" and "act like it's peachy" are both real images and the sentence is one of the angriest in the corpus. Not captured as its own snippet because the metaphor doing the work is scam, which is already held above; this is a wording of it rather than a new image. Logged because "we have to act like it is peachy" names a social pressure — that complaining is not permitted — which nothing else in the library captures.

## What the alliteration sweep found

The prompt asks this pass to set the cross-category alliteration flag when it sees one during metaphor extraction, not to hunt alliteration everywhere. Two flags are set, both above: **"health poor, house poor"** and **"Buyer beware"**. One near-miss was considered and rejected — "mind blowing" in the nightmare snippet is a single compound rather than a pair, so that snippet carries `alliteration: false`.

The honest read on it, `inferred`: this corpus has almost no phonetic play. That is consistent with the arithmetic finding above. People typing a dollar figure into a comment box are not reaching for rhythm. A later pass should not treat two flags in 1,342 records as coverage of the brand's alliteration picture, because the surface that would carry it — reviews, where people write longer and revise — does not exist here.

## Open loops

Three loops. None repeats a loop already filed in `voc-corpus-profile.md`, `voc-pain-phrase.md`, `voc-objection.md`, `voc-trigger-moment.md`, `voc-outcome-phrase.md`, `voc-anti-language.md` or `source-pulls/brand-self-echo-detection.md`. The missing Reddit pull, the missing reviews and the missing surveys are infrastructure items and sit in `data_limitations` above rather than here, per the rubric.

**1. The most engaged image in the comment sections says coverage is luck, and the ads say it is a choice.**

Eleven records treat someone else's good coverage as luck or as winning, and three of the four highest-liked rows in this doc sit in that frame — 19 likes on "Lucky! Mine is $11,000," 11 on "I guess we're lucky," 10 on "You are lucky. Mine is over $10k." The creative running above them asks a woman to believe thirty seconds of clicking will change her situation.

Pull: **Tension.** Two accounts of how a person ends up with the coverage she has cannot both be true as stated, and the audience's version is the one drawing the likes.

Question: What does this audience believe actually determines the coverage a family ends up with?

Why it matters: if she believes coverage is dealt rather than chosen, every ad built on "you are overpaying, switch" is arguing with her worldview before it makes its offer, and the account has never tested creative that starts from hers instead. Territory: **Messaging.**

**2. The brand's own metaphor has been said millions of times and come back once, with a knife in it.**

"Has your back" closes five of the ten highest-spending ads. In 1,342 comments it appears exactly once, from a woman quoting it in scare quotes to point out that she was excluded for being pregnant with type one diabetes. Meanwhile the word the brand borrowed from customers, scam, now recurs 48 times across 15 ads.

Pull: **Gap.** An enormous amount of paid repetition has produced one hostile trace and nothing else, and nothing has been done with that fact.

Question: What image do the moms who actually get through to an agent use for what this company did for them?

Why it matters: it decides whether the brand keeps writing its own metaphors or goes back to borrowing them, which is the choice that separates the language carrying this account from the language sitting unused in its context document. **Routed to the brand**, because answering it needs agent call notes or a survey no tool can reach. Territory: **Messaging.**

**3. Fifteen images in 1,342 records, and every one of them is about the problem.**

Not a single metaphor in this corpus describes a solved situation, a good plan, or relief. Scam, joke, robbery, racquet, dead end, a crack to slip through, a pile of shit, a nightmare, a game somebody else is playing. The whole figurative vocabulary this audience owns points at what is wrong.

Pull: **Pattern.** The same absence keeps holding across every ad family, every month of the corpus, and every one of the four frames.

Question: What does this audience picture on the other side of the problem being fixed?

Why it matters: the brand has no customer-built image of the good outcome to write toward, so it is currently inventing one, and `voc-outcome-phrase.md` already showed that the outcome language in its context document is its own copy filed under a customer heading. Territory: **Messaging.**

## Sources

- Parker MCP `search_facebook_ad_comments_sql`, 26 filtered pulls on 2026-09-04. Every count, every row id and every ad name here. Includes the eleven zero-return searches in the table above, which are the evidence for the thinness finding, and the offset probe that re-pinned the corpus at 1,342.
- Parker MCP `search_facebook_ad_comments_semantic`, three themed passes on 2026-09-04 aimed at comparison and figurative framing, each reporting `totalCommentsAnalyzed 1342`. These surfaced the racquet and robbery rows that no string search would have found first.
- Parker MCP `search_customer_reviews_sql` and `semantic_search_post_purchase_survey`, both 2026-09-04, both zero, both checked live rather than carried from a note.
- Parker MCP `search_facebook_ads_sql`, lifetime mode with the scripts block, 2026-09-04. The full transcripts behind the "has your back" echo verdict and the medical-bankruptcy zero, plus the lifetime lead and spend figures.
- `source-pulls/brand-self-echo-detection.md`. The scam verdict, carried forward and not re-judged, and the standing finding about "wife of the year energy" that this doc's fourth frame extends.
- `personas/voice-of-customer/voc-corpus-profile.md`. Field coverage, corpus bias and the carried theme counts on a 1,322 denominator.
- `personas/voice-of-customer/voc-pain-phrase.md`, `voc-objection.md`, `voc-outcome-phrase.md`, `voc-trigger-moment.md`, `voc-anti-language.md`. The sibling extractions that hold the literal language routed out of this pass.
- `running-notes/missing-context.md` and `running-notes/brand-rules.md`. The dark-surface substitution rule and the lead-generation account shape.
- `parker-system/creative-strategy-context/customer-review-mining-method.md`. The method this pass was performed through: the metaphor and alliteration signals it names as the two highest-priority ones most passes miss, the denominator discipline, the ten-record bar, the claims-check and voice-check governors, the brand-echo failure mode, and the rule that a blank beats a guess.
- `parker-system/creative-strategy-context/persona-research-and-creative-strategy-process.md`. The evidence ranking that puts survey and review data above public comments, and the served-versus-buyer discipline behind the note that every voice here belongs to someone the algorithm served rather than someone who bought.

Neither of the two method docs this pass routes to carries a required sign-off line, so none is stamped here. Stamping one they do not have would be a false proof-of-read.
