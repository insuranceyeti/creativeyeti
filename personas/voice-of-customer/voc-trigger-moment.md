---
brand: health-for-moms
doc: voc-trigger-moment
category: trigger_moment
generated_on: 2026-09-04
refresh_by: 2026-10-04
live_pulls_run_on: 2026-09-04. Every Parker MCP call behind this doc ran today. The sibling VoC docs ran theirs on 2026-09-03, and the corpus moved between the two runs. That is a finding, not a footnote, and it is worked through below.
corpus_denominator: 1342 Facebook and Instagram ad comments, Meta ad account HealthForMoms, act 484897827497337
corpus_date_range: 2025-01-08 to 2026-09-03
prior_version: none. First run. No recurrence history to carry forward.
snippets_captured: 23
sources_read:
  - Parker MCP search_facebook_ad_comments_sql, 24 filtered pulls on 2026-09-04. Every count and every row id in this doc came from these calls, not from an upstream doc.
  - Parker MCP search_facebook_ad_comments_semantic, five themed passes on 2026-09-04. Every pass reported totalCommentsAnalyzed 1342, which agrees with my own offset probe.
  - Parker MCP search_customer_reviews_sql, unfiltered, 2026-09-04. Returned totalReviews 0. Checked live by me.
  - Parker MCP semantic_search_post_purchase_survey, 2026-09-04. Returned totalResponsesForBrand 0 with the collection existing.
  - Parker MCP search_facebook_ads_sql, 2026-09-04, lifetime mode with the scripts block, top ten ads by lifetime spend. Full transcripts read to check what the brand's own creative opens on.
  - personas/voice-of-customer/voc-corpus-profile.md, for field coverage, corpus bias and the limits this pass inherits.
  - personas/voice-of-customer/voc-pain-phrase.md and voc-objection.md, the two sibling extractions, to route language that belongs to them rather than here.
  - source-pulls/ad-comments.md, the full-corpus persona read of the same rows.
  - source-pulls/brand-self-echo-detection.md, for the standing echo verdicts this pass honors rather than re-judges.
  - running-notes/missing-context.md and running-notes/brand-rules.md, for the dark-surface substitution rule and the standing constraints.
  - parker-system/creative-strategy-context/customer-review-mining-method.md, the canonical mining method applied here.
  - parker-system/creative-strategy-context/persona-research-and-creative-strategy-process.md, for the evidence ranking, the served-versus-buyer discipline and the rule that a trigger-anchored identity is the thing a persona is built on.
expected_sources_missing:
  - customer reviews. Zero rows, verified live 2026-09-04. This is where buyers normally recount what was going on when they finally bought.
  - post-purchase surveys. Zero responses, verified live 2026-09-04. The "why now" question lives here and this brand does not ask it.
  - Reddit and forums. Named by the team as the substitute source on 2026-09-03, still not pulled.
  - competitor and category reviews. No rival brands tracked in the Parker app. Branch deferred by the user 2026-09-03.
  - brand-reputation, other-reviews, support tickets, organic social comments. None ingested.
  - agent call notes and the qualifier's own screens. The purchase happens on a phone call Parker cannot see, which is the single largest gap for this pass specifically.
  - personas-profile.md. Not yet written, so no identity or behavioral-signal slug exists to tag with.
data_limitations:
  - One source type only. Under this prompt's confidence rule, cross-source recurrence is what earns strong, so no snippet in this doc can rise above mixed no matter how often it repeats.
  - The behavioral-signal tag is null on all 23 snippets. This prompt says that tag is load-bearing here and should rarely be null, and it also says this pass never invents a slug that personas-profile.md has not defined. The second rule wins. Every snippet names in its notes what the signal would be, so the assembly pass can attach the slug in one edit once personas-profile.md lands.
  - Not one commenter here is confirmed to have bought anything, so strictly these are moments that pushed people to comment, not moments that pushed people to buy. The whole doc is read down one notch for that, and the distinction is argued in full below.
  - author_name and author_id are null on all 1,342 rows. Every recurrence figure is a count of comments, never a count of people.
  - permalink_url is null on all 1,342 rows, so url is null on every snippet. Verification runs through the row id and the Parker tool.
  - The semantic comment tool and the SQL comment tool return different identifier spaces for the same row. Every review_id below is the SQL comment_id, resolved by exact-text lookup where the snippet was first surfaced semantically. Seventeen of the 23 were resolved that way and not one semantic id matched its SQL id.
  - The corpus grew from 1,322 to 1,342 between the sibling docs' pulls and mine. Every percentage in this doc is computed on 1,342. Percentages quoted from upstream docs are on 1,322 and are labelled as carried.
  - Heavy time skew. 16 of the 23 moments below are dated between 2026-03-10 and 2026-05-31, which is the window the MOMS38 creative opened.
  - There is no get_current_time tool on this MCP surface, so the date comes from the session clock.
  - refresh_by is set 30 days out rather than the 180-day voice-of-customer cadence in parker-system/system/refresh-cadence.md. Two triggers have fired: the corpus is actively growing, and personas-profile.md will land soon and fill the null tags on every snippet here.
---

# Trigger moments — Health For Moms

## The honest headline before any moment

This brand has no customer reviews and no post-purchase surveys. I checked both live today rather than trusting the note. `search_customer_reviews_sql` returned `totalReviews: 0` unfiltered, and `semantic_search_post_purchase_survey` returned `totalResponsesForBrand: 0` with the collection existing and empty. `verified`.

So every moment below comes from Facebook and Instagram ad comments, and nothing here may ever be described as this brand's review corpus. The honest sentence downstream is "commenters under the brand's paid ads said," never "customers said."

That sets the ceiling. The mining method ranks survey and review data at the top of the evidence order and public comments near the bottom. The persona method says the same thing and adds that post-purchase survey data is the gold standard precisely because it ties a real buyer to **why and when** they bought. That is this exact category. The single best source for a trigger moment is the one source this brand does not have. So **no snippet in this doc is marked strong**, and any downstream doc that rounds one up is inventing certainty that does not exist.

There is a second discount on top of the first, and it is specific to this pass. A trigger moment is supposed to be what was happening when the customer decided to **buy**. Nobody in this corpus is confirmed to have bought anything. What I can honestly give you is the moment that pushed someone to stop scrolling and type under an insurance ad. Those two moments overlap, and they are not the same. I have kept the distinction live on every snippet rather than quietly collapsing it.

## How I built this, and what I checked

I did not take the upstream numbers on faith, and it is a good thing, because one of them has moved.

**The denominator is no longer 1,322. It is 1,342.** Every sibling doc in this build ran on 2026-09-03 and pinned the corpus at 1,322 comments. I re-ran the probe today. An unfiltered call sorted by `created_time` descending at offset 1300 returned **42** rows, not the 22 the sibling docs recorded. Offset 1341 returned exactly one row, the oldest comment in the corpus, dated 2025-01-08. Offset 1342 returned nothing. That pins the end at **1,342**. Five semantic passes each reported `totalCommentsAnalyzed: 1342`. Two tools, same number. `verified`.

The twenty new rows are not new days. The newest record is still dated 2026-09-03, at 20:46 UTC, where the sibling docs' newest was 13:58 the same day. So a later snapshot of the same day caught rows the earlier one missed. Nothing upstream is wrong. It is just slightly behind, and a pass that quoted "1,322" today would be quoting a number that no longer holds. **Every percentage below is computed on 1,342.** Where I carry a figure from an upstream doc I say so and leave its 1,322 denominator attached rather than silently rebasing it.

**The two comment tools disagree about row identity, and I resolved every case.** A snippet surfaced by `search_facebook_ad_comments_semantic` comes back with an `id` that is not the `comment_id` the SQL tool uses for the same row. The hysterectomy comment is the clearest example: semantic id `2ebf4bfe-3dab-5470-ba70-62fe54cd3f8d`, SQL `comment_id` `1f6f1f3e-b0ed-117f-6b73-2cc3090e019e`. Same text, same timestamp, same ad, two different handles. Seventeen of the 23 snippets below were first surfaced semantically, and I re-found each one by exact-text substring search through the SQL tool before writing its `review_id`. Not one semantic id matched. `verified`, and a later pass that pastes a semantic id into `review_id` will produce a row nobody can look up.

**I pulled the creative rather than reading ad names.** The prompt is strict that a creative claim needs full media, so I pulled the ten highest-spend ads through `search_facebook_ads_sql` in lifetime mode with the scripts block and read the transcripts. That read is the basis for the section below, and it turned out to matter more than I expected.

**A note on what the account looks like from up here.** Lifetime across 1,558 ads: $743,218.09 spend, 39,569 leads, $18.78 cost per lead, zero purchases, because there is no purchase event. 96.1% of spend delivers to women, 44.5% to ages 35 to 44, 99.3% mobile. `verified` from the lifetime summary.

## The thing this pass found first: no ad in this account opens on a moment

I read the transcripts of all ten highest-spend ads. **Not one of them opens on something happening in a woman's life.** `verified`, from the scripts themselves.

Every single one opens on a standing condition or a category claim. The MOMS38 family, which is four of the ten and launched 2026-03-10, opens: "My deductible is $6,000. I have to spend $6,000 in medical expenses before everything is taken care of and there's no copays. But yet I pay for that insurance." That is a state she is in, not an event that happened. The MOMS39 and Moms43 families open on "This is why you can't simply just say oh I have insurance I'm covered," which is an argument. The oldest big spender, `B1 samar- Copy` at $61,237.93 lifetime, opens "Moms, imagine an insurance policy that actually has your back," then reaches for a statistic: "Every three minutes, an American family files for medical bankruptcy even with insurance because they weren't protected when they thought they were." That is a scripted catastrophe in the abstract, aimed at nobody's particular Tuesday.

This matters for two reasons, and they pull in opposite directions.

It is good news for the echo flag. The brand has never scripted a precipitating moment, so no moment below can be the audience repeating one back. **Every snippet in this doc carries `brand_self_echo: false`, and for once that is a clean call rather than a judgment.** `verified` against the full media, not against ad names.

It is also the largest gap this pass found. The account has spent three quarters of a million dollars opening on a number, and the moments that actually move this audience are sitting unused in its own comment threads. That is the first open loop.

## What a trigger looks like when the corpus is a comment section

Before the bank, the honest frame for reading it.

In a review corpus a trigger moment arrives as memory: she bought, and she is telling you why she bought then. In this corpus a trigger moment arrives as **a live situation she is currently stuck in**. She is not reporting a completed decision. She is standing in the middle of one, in public, usually asking a question at the end. The hysterectomy comment ends "I don't have that kind of money laying around." The surgery comment opens "how can I get that." These are people at the moment of the want, which is exactly the moment creative wants to catch, and they are the closest thing to a trigger this surface can produce.

That has one genuinely useful consequence. Because the moment is live rather than remembered, the language has no hindsight polish on it. A review saying "I finally switched because my premium went up" has been tidied by the telling. "My was $7000 they are now raising to $9000" has not.

**The six shapes that actually recur.** These are my classification of the 23 captured moments, `inferred`, with the structural string counts that support each one attached.

| Trigger shape | Moments captured | Supporting string count against 1,342 |
|---|---|---|
| A medical event with a date on it — surgery scheduled, diagnosis just received, a child's procedure blocked | 5 | "surgery" 6 (0.45%), "just found out" 2 (0.15%), "diagnos" 2 (0.15%) |
| The bill or the number landing — she hits the deductible, the bill arrives, the renewal reprices, she does the arithmetic | 6 | "hit my deductible" 1, "blood work" 2, "went up" 1, plus the counter-bid family carried from voc-pain-phrase |
| A household change — a birth coming, a death, a marriage, aging off a parent's plan, a move, children leaving | 5 | "moved" 2 (0.15%), "aging out" 1 |
| A change in work or benefits — rehired, back to work, job hunting for the coverage | 3 | "employer" 24 (1.8%, carried on 1,322), "my job" 7 (carried) |
| An enrollment window, or a switch already under way — locked out until November, or mid-move to a former carrier | 3 | "open enrollment" 1 (0.07%), "until November" 1 |
| The ad itself doing the reminding | 1 | 1 record, quoted in full below |

Read the right-hand column twice, because it is the real finding. **Every one of these counts is tiny.** The largest single trigger word in the corpus is "surgery" at six records. There is no trigger in this corpus that clears the mining method's ten-record bar for a stable pattern. Not one.

So this bank is **23 candidates and zero verified patterns**, and I would rather say that plainly than dress six surgery mentions up as a theme. What makes them worth capturing anyway is the mining method's own rule that usability and count are different questions. These are vivid, dated, specific, and several of them are the only evidence of their kind that exists anywhere for this brand.

**One structural absence worth stating.** The classic insurance triggers are missing outright. "laid off" returns **0** of 1,342. "cobra" returns **0**. "divorce" returns **0**. "turning 26" returns **0**. `verified`, all four. Either this audience does not arrive through those doors, or they arrive through them and never say so under an ad. A Reddit pull would separate those two, and this brand has not run one.

## Trigger moments

Twenty-three distinct accounts. Each is verbatim, with the original spelling, punctuation, casing and emoji preserved exactly. Source type is `ad-comment` for all of them, and the `platform` line carries the ad the comment sits under, because that is the only placement handle these rows have. It reads Facebook or Instagram rather than one of the two, because the corpus does not record which. `review_id` carries the Parker SQL `comment_id`. `url` is null on every one because `permalink_url` is null on all 1,342 records.

**How the claim marks work across all 23.** The `snippet` line is always `stated` — the customer's words, checked character for character against the row the tool returned, typos and all. Every string-based `recurrence` figure is `verified`, because it is a case-insensitive match anyone can re-run against the same 1,342. Every grouping of a snippet into a trigger shape, and every read of which behavioral signal it would map to, is `inferred` and the notes say so. Nothing is `verified` at the level of being a real cross-source pattern, because that needs more than one source type and this brand has one.

**Why `behavioral_signal_tag` is null on all 23.** This prompt says the signal tag is load-bearing here and should rarely be null. It also says the pass never invents a slug that `personas-profile.md` has not defined, and `personas-profile.md` does not exist yet. The second rule wins, so every tag is null by rule rather than by oversight, and each snippet's notes name the signal it would take. That is the fastest possible handoff: when the persona doc lands, the assembly pass reads the notes and fills the field without re-reading a single row.

- snippet: This is what I'm afraid of. Just found out I desperately need a hysterectomy. My husband is looking into insurance for me so that I can get it done. They told him we don't have to meet the deductible which is $7500 but that's hard to believe. I'm worried that when I finally get the surgery scheduled  that I'm gonna have to come up with thousand before it can be done. I don't have that kind of money laying around.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: 1f6f1f3e-b0ed-117f-6b73-2cc3090e019e
    date: 2026-04-14
    url: null
  recurrence: 2 for the exact "just found out" opening, 6 for the scheduled-medical-event shape
  source_diversity: [ad-comment]
  first_seen: 2026-04-10
  last_seen: 2026-05-04
  confidence: mixed
  brand_self_echo: false
  notes: The single richest trigger moment in 1,342 records and the one I would build a brief on first. It carries a diagnosis just received, a procedure not yet scheduled, a husband already shopping on her behalf, and the exact fear that stops the purchase, all in one comment. Signal would be a newly diagnosed condition forcing a coverage decision. Denominator is 1,342, and "just found out" returns 2, so this is a candidate rather than a pattern by the ten-record bar. Note the buying is being done by her husband, which lines up with the corpus's separate finding that the woman in this audience is often the household's insurance shopper and sometimes is not. The double space before "that I'm gonna" is in the original.

- snippet: how can I get that because I pay $1000 a month for my insurance and tomorrow I have surgery
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS39 - 2 - V2 and MOMS39 - 2 - V2 - Copy
    review_id: c1478851-ccf4-9289-116a-345c3d6a8f51
    date: 2026-05-04
    url: null
  recurrence: 6 for the scheduled-medical-event shape
  source_diversity: [ad-comment]
  first_seen: 2026-03-31
  last_seen: 2026-05-04
  confidence: mixed
  brand_self_echo: false
  notes: The tightest deadline anywhere in the corpus. "tomorrow I have surgery" is a trigger with a clock on it, and it opens with "how can I get that," which is intent stated outright rather than inferred. Signal would be an imminent scheduled procedure. Useless as a sale, since no plan starts overnight, and that is exactly why it is worth knowing: the moment she is most motivated is the moment the product can least help her, and the creative has never spoken to the window before it.

- snippet: Our deductible is $10,500 😭
  And I have to have surgery in June
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V10
    review_id: cb09b87a-d42c-d3f0-b5d7-72ade82bee9b
    date: 2026-04-02
    url: null
  recurrence: 6 for the scheduled-medical-event shape
  source_diversity: [ad-comment]
  first_seen: 2026-03-31
  last_seen: 2026-05-04
  confidence: mixed
  brand_self_echo: false
  notes: The same shape as the one above with two months of runway instead of one night, which makes it the more useful version commercially. She names the number and the date in two lines. Signal would be a scheduled procedure with a known cost ahead of it. The line break is in the original and should be kept if this is lifted, because the beat between the figure and the deadline is the whole effect.

- snippet: It's still sucks! My deductible is $5000 and my out of pocket maximum is $7500. I owe that from a total emergency hysterectomy last year and starting over, cancelled all my prescriptions and just can't afford it.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V5
    review_id: eebbfee2-c611-c8e0-2218-05237293d1f5
    date: 2026-03-31
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-31
  last_seen: 2026-03-31
  confidence: thin
  brand_self_echo: false
  notes: One record, so thin by the rule, and kept because it is the only place in the corpus where the trigger is the aftermath rather than the event. The emergency was last year. What is happening now is that she is still paying for it and has stopped taking her medication because of it. Signal would be carrying medical debt from a past emergency into a new plan year. "cancelled all my prescriptions" is the phrase, and it is the sharpest consequence stated anywhere in 1,342 records. Carries 2 likes.

- snippet: Tried to look into it because I'm having my baby within the next month and I am still a dependent on my parents coverage so she will not be covered. I will be aging out of their insurance in Nov. I put in my information and they said there's no plans available for me...
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: c40131c5-d9af-f066-e301-0f1fe281755b
    date: 2025-07-23
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-07-23
  last_seen: 2025-07-23
  confidence: thin
  brand_self_echo: false
  notes: Thin at one record and the most load-bearing snippet in the doc after the hysterectomy one. Three triggers are stacked in a single comment: a birth inside a month, a baby who will have no coverage, and her own coverage ending in November. It is also the only snippet in the corpus where a commenter states the causal chain outright, "Tried to look into it because," which is a trigger and an attribution in the same clause. Signal would be aging off a parent's plan with a dependent arriving. It ends in the funnel turning her down, so it belongs half to the objection pass, and voc-objection.md has that half. Dated 2025-07-23, eight months before the MOMS38 wave, which makes it era evidence that these moments predate the campaign that produced most of the corpus. Carries 1 like and 6 replies.

- snippet: My Mom needs coverage, my Dad died end of June & the insurance Co called her 5 days after the e passed to tell her she won't have coverage after end of July
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B2 - 10TH JUNE - Copy 16
    review_id: 4b95ef6b-b643-590c-cc9e-5a8e6a257d34
    date: 2025-07-10
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2025-07-10
  last_seen: 2025-07-10
  confidence: thin
  brand_self_echo: false
  notes: One record, thin, and the hardest one in the corpus to read. A death, a phone call five days later, and a coverage termination date, all with dates attached. Signal would be losing coverage through a spouse's death. Two things make it worth carrying past its count. It is a daughter shopping for her mother, which is the buying-on-behalf-of pattern the corpus profile flagged as a persona signal. And it is the only bereavement trigger in 1,342 records, which is itself information about who this creative reaches. The typo "the e passed" is in the original and preserved. Carries 2 replies. Flag for the claims-check governor before any use, since a bereavement story lifted into insurance copy is a judgment the brand should make deliberately.

- snippet: Ive never had insurance through work and i just found out what tf a deductible is(mines $12,000) and now i have a 2000$ hospital bill that if id had known id have just suffered.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS39 - 2 - V2 and MOMS39 - 2 - V2 - Copy
    review_id: 1fd0a565-7a47-d657-98fe-a75e65f0d6a0
    date: 2026-04-10
    url: null
  recurrence: 2 for "just found out", 5 for the bill-landing shape
  source_diversity: [ad-comment]
  first_seen: 2026-03-26
  last_seen: 2026-05-11
  confidence: mixed
  brand_self_echo: false
  notes: The moment of discovery, which is a distinct trigger from the moment of cost. She did not know what a deductible was until a bill taught her. Signal would be a first encounter with the real cost of a plan she already held. "if id had known id have just suffered" is the line to keep and it is the bleakest sentence in the doc: the lesson she took is to avoid care, not to switch plans. The mining method flags emotive and visceral language as a qualifying signal separate from the number, and this carries both.

- snippet: I about hit my deductible last month just getting blood work done. So dumb.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 893b21cf-2a53-935d-6fb2-0d5401f82354
    date: 2026-03-31
    url: null
  recurrence: 1 exact, 5 as the bill-landing shape
  source_diversity: [ad-comment]
  first_seen: 2026-03-26
  last_seen: 2026-05-11
  confidence: thin
  brand_self_echo: false
  notes: Thin at one record and short enough to be a hook as written. The trigger is the smallness of the thing that did it. Not a surgery, blood work. Signal would be routine care exposing the plan's real cost. "So dumb." is the rhythm to keep. Verified as a string: "hit my deductible" returns exactly 1 of 1,342 and "blood work" returns 2, of which this is one and the other is a commenter arguing the opposite case.

- snippet: Mine is $8,000 and I hit it in the beginning of march 🤣😭
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V8
    review_id: 3561c1ce-a975-6929-7316-36feaea03697
    date: 2026-03-26
    url: null
  recurrence: 1 exact, 5 as the bill-landing shape
  source_diversity: [ad-comment]
  first_seen: 2026-03-26
  last_seen: 2026-05-11
  confidence: thin
  brand_self_echo: false
  notes: Thin on count. Kept because it dates the trigger inside the calendar year, which nothing else here does as cleanly: eight thousand dollars gone by early March. Signal would be exhausting the deductible early in the plan year. The two emoji together, laughing and crying, are the corpus's default register for this and should not be cleaned up in a lift. Carries 2 likes. Note this snippet also sits inside the counter-bid family that voc-pain-phrase.md counted at 82 records for the string "mine is" against 1,322; that count is the pain pass's and I have not rebased it here.

- snippet: I had my son schedule for tubes bc he keeps getting ear infections.  He is autistic.  They called me a week before his appointment and said they need 1500 down.... I was like how.  Our deductible is 4500. I told her I guess I'll call back after we meet our deductible.  So I guess my son will have to suffer from ear pain till then.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: d0a0a016-0f7f-7069-7cca-2829b3891982
    date: 2026-04-11
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-11
  last_seen: 2026-04-11
  confidence: thin
  brand_self_echo: false
  notes: One record and the most producible story in the doc, because it is a scene with a phone call, a number, a decision and a consequence, which is exactly the whole-review-concept shape the mining method says is rare and high leverage. The trigger is a call a week before a child's procedure. Signal would be a child's scheduled care blocked by an up-front payment. It is also the only moment in the corpus where the person who goes without care is the child rather than the mother, and for a brand called Health For Moms that is worth noticing. The full record continues that she and her husband's employer pay about $1,000 a month between them. The four-dot ellipsis and double spaces are original. Flag for the claims-check governor.

- snippet: My was $7000 they are now raising to $9000
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: cd97741c-695c-8ada-8c99-357297a77607
    date: 2026-04-09
    url: null
  recurrence: 1 exact, 2 for the renewal-hike shape
  source_diversity: [ad-comment]
  first_seen: 2026-04-09
  last_seen: 2026-04-16
  confidence: thin
  brand_self_echo: false
  notes: Thin at one record and structurally important out of proportion to its size. This is the renewal increase, which in most insurance categories is the single biggest switching trigger there is, and in 1,342 comments it appears about twice. The other is "Britt Johnson cost went up." on 2026-04-16, row 324e9b13-f8c6-a223-adb7-7aa619d18c23. Signal would be a renewal repricing. The near-absence is the finding: either the brand's ads never run when renewal letters land, or this audience does not narrate that moment publicly. The typo "My was" is original.

- snippet: When i realized the premium was NOT part of the deductible I was flabbergasted what the point if ill spend more on a premium than I will in routine visits and even if I need a big time care the hospital will charge less than I spent all year on paying premium+deductible 🫠
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: 0691ad4c-2fd7-6109-3b4f-290b377b39e9
    date: 2026-04-13
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-13
  last_seen: 2026-04-13
  confidence: thin
  brand_self_echo: false
  notes: One record. The trigger is a realization rather than an event, which stretches the category, and I kept it because the prompt is explicit that judgment beats the shape list when a source plainly names the moment something tipped. "When i realized" is a moment in time with a before and an after. Signal would be understanding the premium and deductible stack for the first time. Note the conclusion she reaches is that coverage is not worth buying at all, which is the same exit the corpus profile counted at 33 records across 10 ads on a 1,322 denominator. The brand's own hook opens that door.

- snippet: This is me. Im on moujaro for diabetes and now I can't afford it because they want me to pay $1000 a month till my deductible is met. Im lost, can't afford it now.
  category: trigger_moment
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
  notes: One record, and it is the only one in the corpus that opens with recognition and then supplies its own trigger. "This is me" appears in exactly 1 of 1,342 comments, which I checked as a string. The trigger is a drug cost changing under her. Signal would be a medication becoming unaffordable mid-treatment. "Im lost" is the phrase and voc-pain-phrase.md also carries this record for that reason; the pain half and the trigger half are different halves of the same sentence and both passes should hold it. The misspelled drug name is preserved exactly.

- snippet: A mom with no job..... when I was a SAHM free insurance. Got a job after kids got school aged.... no free insurance anymore
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad Yeti State Angle - 1 - V1
    review_id: b0f32883-685f-fdd1-378e-39cf37d68f54
    date: 2026-04-06
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-06
  last_seen: 2026-04-06
  confidence: thin
  brand_self_echo: false
  notes: One record and a genuinely counterintuitive trigger: going back to work is what cost her the coverage. Signal would be a return to work ending subsidized eligibility. Worth flagging to the persona work, because it names a moment in a mother's life the brand's creative has never touched and it maps onto the life stage the account already targets hardest, ages 35 to 44 at 44.5% of lifetime spend. It sits on Yeti State Angle - 1 - V1, one of the few records outside the MOMS38 family. The five-dot and four-dot ellipses are original.

- snippet: I'm heading in to work so couldn't really look at this.
  And with bring a new rehiring I'm able to enroll into insurance. Not sure if I want to.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: c3a8a407-abdd-ffe1-25af-b9e556bafa04
    date: 2026-04-30
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-30
  last_seen: 2026-04-30
  confidence: thin
  brand_self_echo: false
  notes: One record, thin, and the only live enrollment window in the corpus. A rehire opens a special enrollment period and she is standing inside it, undecided. Signal would be a special enrollment window opened by a job change. It is also a small usability finding the brand should have: she says outright she could not look at the offer because she was leaving for work, which is a mobile audience at 99.3% of spend being asked to complete a form on the way out the door. The typo "with bring" is original.

- snippet: Holly Jamison thanks. Currently looking for a new job with better insurance, but not having the best luck
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: fcf8227e-e6cc-7489-aaf0-73589b463a71
    date: 2026-03-28
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-28
  last_seen: 2026-03-28
  confidence: thin
  brand_self_echo: false
  notes: One record. The trigger is an active job hunt undertaken for the coverage rather than the work, which inverts the usual order and is the strongest single piece of evidence in the corpus that this audience treats insurance as the thing worth changing your life around. Signal would be job searching in order to solve coverage. The record opens with another commenter's name, which is how replies render in this corpus; the name is preserved because the snippet rule is verbatim, and a writer lifting it would drop it.

- snippet: Had a similar conversation recently with my soon to be former insurance company.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 2 - V4
    review_id: 8eab4c8b-250f-7eda-5c90-294f5c168bb6
    date: 2026-03-23
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-23
  last_seen: 2026-03-23
  confidence: thin
  brand_self_echo: false
  notes: One record and the closest thing in 1,342 comments to someone announcing they are mid-switch. "soon to be former" is doing all the work and it is the most quotable four words in the doc. Signal would be an in-progress decision to leave a current carrier. Where it sits matters as much as what it says: MOMS38 - 2 - V4 is the skit family where one woman plays both the frustrated mom and the claims rep, which the corpus profile identified as the only creative in the account that draws agreement instead of argument. So the one person announcing a switch is answering the one ad that dramatizes an experience rather than a bill.

- snippet: What if I have an insurance plan that is too expensive but want to change it? Can I apply?
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: e9635fa0-755d-a07e-d415-00ea106aaa34
    date: 2026-03-23
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-23
  last_seen: 2026-03-23
  confidence: thin
  brand_self_echo: false
  notes: One record, thin, and it sits right on the line between a trigger and an objection. I kept it here because it names a decision she has already made, the plan is too expensive and she wants out, and asks only whether the door is open. Signal would be an active intent to switch pending eligibility. It belongs to the wider eligibility-question cluster that voc-corpus-profile.md counted at 166 records containing a question mark on a 1,322 denominator, and that cluster is the largest untouched demand signal in the account.

- snippet: Does this work in Louisiana? Because they wouldnt let me apply for good insurance here until November.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad Moms43 - 4 - V3
    review_id: 746bf70c-d78f-a999-85c6-e7873b195657
    date: 2026-05-27
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-05-27
  last_seen: 2026-05-27
  confidence: thin
  brand_self_echo: false
  notes: One record. The trigger here is a window she has been locked out of, which is the timing objection the brand says it has, arriving as a live situation instead of a stated hesitation. Signal would be being blocked from enrolling until the next window. This is the sharpest evidence available on that question and it is one comment, which is exactly the point of open loop four in voc-corpus-profile.md. Verified as a string: "open enrollment" returns 1 of 1,342 and it is a different record, someone explaining the rule to a stranger. The full record continues into a real anti-language complaint about smaller insurers costing more, and voc-anti-language.md carries that half.

- snippet: That reminds me my sons insurance has been bullshit I need to call them again
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad OMC - C11 - 2b
    review_id: 999a381a-b982-0b4b-b33a-96861545d9e5
    date: 2026-03-05
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-05
  last_seen: 2026-03-05
  confidence: thin
  brand_self_echo: false
  notes: One record and the only one where the ad itself is the trigger. "That reminds me" is the moment a dormant problem gets reactivated by a piece of creative, which is the exact job a top-of-funnel ad is supposed to do, and it is the single clearest evidence in 1,342 records that this account's creative can do it. Signal would be a dormant coverage problem reactivated by an ad. It is also a reminder that the thing she goes to do is call her existing insurer, not click. Voice-check flag, since the wording will not survive a lift as written; the observation survives.

- snippet: Moved from NY to GA. Went from $6500 deductible to $250 🙌🏼
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS39 - 2 - V2 and MOMS39 - 2 - V2 - Copy
    review_id: 67902773-6f7b-9c0a-4dc3-42d08a70c586
    date: 2026-08-14
    url: null
  recurrence: 2 for "moved", 1 for this shape
  source_diversity: [ad-comment]
  first_seen: 2026-04-26
  last_seen: 2026-08-14
  confidence: thin
  brand_self_echo: false
  notes: One instance of the shape, thin, and kept for two reasons. It is the only geographic trigger in the corpus, a state move that changed her deductible by a factor of twenty-six. And it is one of the few records from the quiet current era rather than the spring wave. Signal would be a move across state lines resetting plan options. Careful routing: the result she reports is real but it came from moving, not from this brand, so it is not an outcome phrase for Health For Moms and voc-outcome-phrase.md records it as a non-brand outcome rather than a brand one. The other "moved" record is a woman whose children have moved out, a different trigger entirely.

- snippet: This is why I didn't have health insurance until I got married
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: d289a474-90d4-a87b-906a-57fa89cfcb79
    date: 2026-03-27
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-27
  last_seen: 2026-03-27
  confidence: thin
  brand_self_echo: false
  notes: One record, thin, and historical rather than live. She is describing a trigger that already fired, marriage being what finally got her covered. Signal would be gaining coverage through a spouse. It is the only marriage trigger in 1,342 records and it is worth carrying precisely because it shows a route into coverage the brand cannot compete with. She did not buy insurance. She married into it.

- snippet: OK, this is great for mom's of young children. What about the rest of us? What about those of us who got screwed by Obama's healthcare system, and have to pay all that money out before anything is covered. What about those of us whose children are grown and moved out of the house now?  My deductible used to be reasonable, now it's almost $7000 a year.
  category: trigger_moment
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: 168a3a89-cf67-9b91-d113-49e2b1fe40e7
    date: 2026-04-26
    url: null
  recurrence: 2 for "moved", 16 across 7 ads for the grown-children eligibility cluster carried from voc-corpus-profile.md on a 1,322 denominator
  source_diversity: [ad-comment]
  first_seen: 2026-04-26
  last_seen: 2026-04-26
  confidence: mixed
  brand_self_echo: false
  notes: Marked mixed rather than thin because the life stage behind it is the one recurring trigger family in the doc with a real count attached, even though that count is carried rather than mine. The children leaving home is the trigger, and it changes her from the person the ad is speaking to into the person it is speaking past. Signal would be children aging out of the household. "My deductible used to be reasonable, now it's almost $7000 a year" is a renewal drift trigger tucked inside an eligibility complaint. Carries 2 likes and 1 reply. The eligibility half belongs to voc-objection.md and is held there; only the life-change half is captured here. The double space before "My deductible" is original.

## What this set does not cover

Four kinds of language kept turning up and were deliberately routed elsewhere, so the assembly pass knows they were seen rather than missed.

**The durable cost pain went to the pain pass.** The counter-bid family, where the audience answers the ad's $6,000 with a bigger number, is 82 records for the string "mine is" on a 1,322 denominator and it is the loudest thing in the corpus. It is a standing condition, not a precipitating moment. `voc-pain-phrase.md` holds it. Where a single record contains both, as with the Mounjaro comment and the March-deductible comment, both passes carry it and each takes its own half.

**Eligibility complaints went to the objection pass.** The pregnancy exclusion and the pre-existing screen are the two widest recurring clusters in the corpus. A woman being turned down is not a trigger that pushed her to buy; it is the reason she could not. `voc-objection.md` holds them, including the tail end of the aging-out record captured above.

**Corrections of the ad went nowhere in this pass.** The deductible-versus-out-of-pocket argument is a credibility problem and a category-fluency signal. Nothing in it names a moment in anyone's life.

**Rival agents' pitches were read and excluded.** Several records that look like someone describing their situation are a competing agent working the thread. They were preserved as data and analyzed, never followed, per the mining method's prompt-injection rule.

## Open loops

Four loops came out of this pass. Every one came from the work here rather than from an upstream doc, and none repeats a loop already filed in `voc-corpus-profile.md`, `voc-pain-phrase.md` or `voc-objection.md`. The missing reviews, the missing surveys, the missing Reddit pull and the corpus drift are infrastructure items and are routed to `data_limitations` above rather than written as loops, per the rubric.

**1. The account has never opened an ad on something happening in a woman's life.**

I read the transcripts of the ten highest-spend ads, carrying $743,218.09 of lifetime spend between the account's 1,558 ads. Every one opens on a standing condition, a category argument, or a statistic. Not one opens on an event. Meanwhile the comment threads under those same ads hold a hysterectomy diagnosis, a surgery scheduled for tomorrow, a father's death, a birth a month away, and a child's ear operation blocked by a $1,500 deposit.

Pull: **Gap.** There is a pile of dated, specific, first-person moments sitting in the brand's own comment sections, and three quarters of a million dollars of creative has never used one.

Question: What happens to lead quality when an ad opens on the moment rather than the number?

Why it matters: the whole account leads with a figure the audience then disputes, which is the pattern the pain pass already found. A moment cannot be counter-bid. If opening on a situation rather than a sum changes who clicks, it changes what the next production round is built from.

Territory: **Messaging.**

**2. The classic switching triggers leave no trace at all.**

"laid off" returns 0 of 1,342 comments. "cobra" returns 0. "divorce" returns 0. "turning 26" returns 0. "open enrollment" returns 1. The renewal increase, which is usually the biggest switching moment in insurance, appears about twice. Yet these are the moments the category is built around.

Pull: **Surprise.** For a product whose entire market is people changing plans, finding essentially none of the standard reasons people change plans is not what the setup would predict, and the size of that gap is the signal.

Question: Where do the women who actually switch plans talk about the moment they decided to?

Why it matters: if those conversations happen somewhere this brand has never looked, then the brand's only listening post is systematically deaf to its own buying moment. That would make a Reddit or forum pull worth more than another month of comment reading.

Territory: **Messaging.**

**3. The most motivated person in the corpus is the one the product can help least.**

The woman with surgery tomorrow asks "how can I get that." The woman with a hysterectomy pending says her husband is already shopping. The woman whose son needs ear tubes was asked for $1,500 a week before the appointment. In each case the want is at its peak and the timeline is far too short for any plan to start.

Pull: **Tension.** The moment this audience is most ready to act and the moment the product can actually serve them cannot both be the same moment, and right now the creative behaves as though they are.

Question: How far ahead of a medical event does a woman start looking for different coverage?

Why it matters: it decides whether the brand should be catching her at the crisis or at the calm before it, and those are two completely different ads. Right now the account runs one message at every stage.

Territory: **Personas.**

**4. Going back to work is what cost her the coverage.**

One woman writes that she had free insurance as a stay-at-home mother, took a job once her children were school-aged, and lost it. Another says a rehire has just opened an enrollment window she is not sure she wants. A third is job hunting specifically to get better insurance. All three are moments where work and coverage move together, and the brand's creative treats employment as a fixed background condition.

Pull: **Curiosity.** Three different women describe work and coverage changing hands at the same moment, in three different directions, and the rest of Parker's context on this brand cannot explain what that means for who the buyer is.

Question: What happens to a mother's coverage when she goes back to work?

Why it matters: the account targets women 35 to 44 with 44.5% of its lifetime spend, which is exactly the return-to-work window. If that transition reliably breaks coverage, it is a named moment with a predictable date, and nothing in the account speaks to it.

Territory: **Personas.**

## Sources

- Parker MCP `search_facebook_ad_comments_sql`, 24 filtered pulls on 2026-09-04. Every count, every row id, and the offset probe that re-pinned the denominator at 1,342.
- Parker MCP `search_facebook_ad_comments_semantic`, five themed passes on 2026-09-04. Surfaced seventeen of the 23 moments, each then resolved to its SQL `comment_id` by exact-text lookup.
- Parker MCP `search_customer_reviews_sql` and `semantic_search_post_purchase_survey`, 2026-09-04. Both zero, checked live.
- Parker MCP `search_facebook_ads_sql` with the scripts block, lifetime mode, 2026-09-04. The ten highest-spend ads read at full media depth, which is the basis for the claim that no ad opens on a moment.
- `personas/voice-of-customer/voc-corpus-profile.md`. Field coverage, corpus bias, and the carried theme counts that still sit on a 1,322 denominator.
- `personas/voice-of-customer/voc-pain-phrase.md` and `voc-objection.md`. The two sibling extractions, used to route language out of this pass and into theirs.
- `source-pulls/ad-comments.md`. The full-corpus persona read of the same rows.
- `source-pulls/brand-self-echo-detection.md`. The standing echo verdicts honored rather than re-judged.
- `running-notes/missing-context.md` and `running-notes/brand-rules.md`. The dark-surface substitution rule, the lead-generation account shape, and the standing constraints.
- `parker-system/creative-strategy-context/customer-review-mining-method.md`. The three-way hunt, the qualifying signals, the exclusion list, the claims-check and voice-check governors, era tagging, the denominator discipline and the ten-record bar.
- `parker-system/creative-strategy-context/persona-research-and-creative-strategy-process.md`. The evidence ranking that caps this brand at mixed, the trigger-anchored definition of a persona, and the served-versus-buyer distinction.
