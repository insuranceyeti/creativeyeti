---
brand: health-for-moms
doc: voc-surprise-delight
category: surprise_delight
generated_on: 2026-09-04
refresh_by: 2026-10-04
live_pulls_run_on: 2026-09-04. Every Parker MCP call behind this doc ran today, against a corpus re-pinned live at 1,342 by my own offset probe. The earliest sibling docs ran on 2026-09-03 against 1,322 and say so; carried figures keep their 1,322 denominator and are labelled.
corpus_denominator: 1342 Facebook and Instagram ad comments, Meta ad account HealthForMoms, act 484897827497337
corpus_date_range: 2025-01-08 to 2026-09-03
prior_version: none. First run. No recurrence history to carry forward.
snippets_captured: 2
snippets_about_the_product_itself: 0
sources_read:
  - Parker MCP search_facebook_ad_comments_sql, 17 filtered pulls on 2026-09-04, most of which returned zero or near-zero and are the evidence for this doc's blank. Every count and row id was re-derived by me from the returned rows.
  - Parker MCP search_facebook_ad_comments_semantic, two themed passes on 2026-09-04 aimed squarely at unexpected positives. Both reported totalCommentsAnalyzed 1342. One returned seven results in the entire corpus and that number is the strongest single piece of evidence in this doc.
  - Parker MCP search_customer_reviews_sql, unfiltered, 2026-09-04. Returned totalReviews 0. This is where delight language normally lives.
  - Parker MCP semantic_search_post_purchase_survey, 2026-09-04. Returned totalResponsesForBrand 0 with the collection existing. The open question about what you did not expect lives here, and this brand does not ask it.
  - Parker MCP search_facebook_ads_sql, 2026-09-04, lifetime mode with the scripts block, top ten ads by lifetime spend. Read to establish which benefits the brand already markets, which is the only way to tell an organic surprise from a promoted benefit coming back.
  - source-pulls/brand-self-echo-detection.md, for the standing verdict on the brand's three self-authored product-experience phrases. Re-verified live here against the larger corpus.
  - personas/voice-of-customer/voc-outcome-phrase.md, whose two service records this pass re-reads under a different lens, and whose blank finding this pass independently confirms rather than repeats.
  - personas/voice-of-customer/voc-objection.md, voc-pain-phrase.md, voc-trigger-moment.md, voc-anti-language.md, voc-metaphor.md, voc-aspirational.md and voc-category-jargon.md, the sibling extractions.
  - running-notes/missing-context.md and running-notes/brand-rules.md, for the lead-generation account shape that explains this blank.
  - parker-system/creative-strategy-context/customer-review-mining-method.md and persona-research-and-creative-strategy-process.md, the two methods this pass is performed through.
expected_sources_missing:
  - customer reviews. Zero rows, verified live 2026-09-04. A delight is almost always reported after the thing worked, which makes this the most damaging blank for this category.
  - post-purchase surveys. Zero responses, verified live 2026-09-04. The question that surfaces a delight directly - what did you not expect - is a survey question, and this brand asks nobody.
  - Reddit and forums. Not pulled. People share pleasant surprises with peers freely and with no brand prompting.
  - competitor and category reviews. No rival brands tracked in the Parker app.
  - agent call notes and partner-agency records. The service moment where a delight would be created is a phone call handled by a partner agency, invisible to every tool Parker has.
  - brand-reputation, other-reviews, support tickets, organic social comments. None ingested.
  - personas-profile.md. Not yet written, so identity and behavioral-signal tags are null by rule.
data_limitations:
  - This doc is a near-blank and the blank is the finding. Two snippets in 1,342 records, 0.15%, and neither is about the product. Both are about the agent who could not help.
  - Zero records describe an unexpected positive about the thing the brand sells. That is stated as a measured result, not as an impression.
  - One source type only, so nothing here could rise above mixed even if it were plentiful. Both captured snippets are thin on top of that.
  - The surface is structurally hostile to this category, more so than to any other in the library. A delight requires having received the thing. A comment section under a paid ad is upstream of receiving anything.
  - author_name and author_id are null on all 1,342 rows. Every count is a count of comments, never of people.
  - permalink_url is null on all 1,342 rows, so url is null on every snippet.
  - The semantic comment tool and the SQL comment tool return different identifier spaces for the same row. Every review_id below is the SQL comment_id, resolved by exact-text lookup where a row was first surfaced semantically. The "Wow this sounds better than my plan" row logged below is a clean example - the semantic id is d1038ca4 and the SQL comment_id is 23c73d99.
  - The database stores curly apostrophes, so contraction searches were written apostrophe-free. "t expect" was used rather than "didn't expect" for that reason.
  - No join exists between any comment and the 39,569 leads this account has produced lifetime, so nothing here can be tied to a person who was actually handed to an agent.
  - refresh_by is 30 days rather than the 180-day voice-of-customer cadence, matching the sibling docs. This doc and voc-outcome-phrase.md are the two most likely in the library to change completely the moment any review or survey pipeline is switched on.
  - There is no get_current_time tool on this MCP surface, so the date comes from the session clock.
---

# Voice of Customer — surprise and delight — Health For Moms

## The short version, before anything else

**This category is nearly empty for this brand, and the emptiness is the finding.** Two records in 1,342, and neither one is about the product. Both are about an insurance agent being kind to a woman he could not help.

That is not a failed pass. It is a measured result, and the mining method is explicit that a proven blank with the reason attached beats a padded section. `voc-outcome-phrase.md` came back near-empty for the same underlying reason and was correct to. This doc re-tested the question from a different angle rather than assuming that result carried, and it lands in the same place.

The reading surface is one thing: **1,342 Facebook and Instagram ad comments** from Meta ad account `HealthForMoms`, act `484897827497337`, 2025-01-08 to 2026-09-03. I re-pinned that total with my own offset probe today. Customer reviews returned zero rows live. Post-purchase surveys returned zero responses live. Reddit is not pulled.

## The sweeps, and what came back

Every figure below is a case-insensitive substring search across all 1,342 records, run live today, with each returned row read in place.

| String searched | Records | What they actually are |
|---|---|---|
| "surprise" | 2 | both are advice about cash prices and drug costs, neither about this brand |
| "t expect" | 1 | a joke about the brand not covering expecting mothers |
| "thank you" | 3 | **all three thank another commenter, none thanks the brand** |
| "so glad" | 1 | a political remark about Trump |
| "love it" | 1 | wishing a company existed that covered alternative medicine |
| "easy" | 3 | none about this brand's process |
| "recommend" | 5 | two say "Not recommend," one says "I DO NOT RECOMMEND!", one recommends her own plan, one recommends calling any agent |
| "answered a few questions" | **0** | |
| "explained things" | **0** | |
| "pressured" | **0** | |
| "cross this off" | **0** | |

Those last four are not idle searches. They are the phrases the brand's own context document lists under "How They Describe the Product Experience," presented as customer language. `source-pulls/brand-self-echo-detection.md` established on 2026-09-03 that all of them return zero across 1,322 records, and that the document itself admits their origin, introducing them with "Based on the brand's positioning and on-site language, the ideal customer experience language reads." **I re-ran all four today against the larger 1,342-record corpus and all four still return zero.** `verified`. The standing echo verdict holds against twenty more rows than when it was written.

**The semantic sweep is the stronger evidence, because it catches the paraphrase a string match misses.** I ran a pass across the whole corpus for "I did not expect this, pleasantly surprised, better than I thought, bonus I did not know about, unexpectedly good experience," at a 0.30 similarity floor — a deliberately loose floor, chosen to over-return rather than under-return. In 1,342 records it came back with **seven results total**. Seven. And reading all seven, **not one is about Health For Moms**:

- "Wow this sounds better than my plan" — row `23c73d99-a6b6-cd23-2de6-4567dcb5a64f`, ad `Internal Videos - OCT - B2 - Copy 3`, 2025-10-27. A reaction to a claim in an ad, not to anything received.
- "I was extremely shocked when I found out that they offered this. I didn't even know companies offered this level of health insurance." — 2026-04-28, 3 likes. Her employer.
- "I have no copay, blessed beyond belief!" — 2026-04-26. A plan she already had.
- "you have excellent benefits at your job! This is not the norm." — 2026-04-07, 7 likes. Somebody else's job.
- "Welp thankfully I have benefits thru my job" — 2026-05-10. Her job.
- "When i realized the premium was NOT part of the deductible I was flabbergasted" — 2026-04-13. A surprise, and an unpleasant one.
- "Cool, what is your out of pocket? 🤔" — 2026-04-27. A question.

That is the shape of the thing. **Ask this corpus for delight and it hands you five people who are pleased with their employer and one woman who was flabbergasted in the wrong direction.**

## Why the blank is structural, not a sampling accident

A reader could reasonably conclude from the table above that this brand's service is disappointing people. That is not what the evidence says, and getting this right matters.

**One. A delight requires having received something, and nobody in this corpus has.** These 1,342 people are commenting under an ad. `running-notes/missing-context.md` is blunt about the account shape and it is the key to this doc: this is lead generation, not ecommerce. Lifetime the account has produced **39,569 leads across $743,218.09 of spend at an $18.78 cost per lead, and zero purchases**, because no purchase event exists. `verified` from the lifetime summary I pulled today. Surprise-and-delight is a post-receipt category and this is a pre-receipt surface. The two do not overlap.

**Two. There is no unboxing here, and that is not a joke.** Most of the examples this prompt names — the touch in the packaging, the secondary use stumbled into, the unforeseen convenience — assume a physical or ongoing product the customer lives with. This brand's deliverable is a phone call with a partner agency, and after it either a policy exists somewhere or it does not. There is no moment where a person opens something. The category's usual raw material does not exist for this business, and no amount of corpus would produce it.

**Three. The one place a delight could be created is invisible.** The service moment is that phone call, handled by a partner agency, with no recording, no transcript, no follow-up email and no review request reaching any tool Parker has. `voc-outcome-phrase.md` made this argument about outcomes and it applies with more force here, because a delight is created by service quality specifically, and service quality is exactly what happens on that call.

**So the honest statement is not "customers report no delights."** It is **"Parker has no way to observe whether customers are delighted, and neither does the brand."** Those are different sentences and only the second is true.

## What the blank costs, in plain terms

**The brand is writing its own delight.** Three phrases in its context document describe an easy, unpressured, well-explained experience, and the document says outright they were derived from the brand's own positioning and website. All three return zero in the customer record, re-verified today. Any writer who opens that section will ship the brand's marketing back at the customer as her own pleasant surprise.

**Worse, the only service evidence that does exist points the other way.** `source-pulls/brand-self-echo-detection.md` found fifteen comments across ten different ads warning that filling in the form brings a flood of calls, and the sharpest of them drew 33 likes, the third-highest in the corpus. `voc-objection.md` holds that cluster. A writer using "Nobody pressured me" as customer language would be writing directly against the only service signal the brand actually has.

**There is no delight to lead with, because there is no observed delight at all.** The prompt's whole purpose — find the unmarketed benefit customers discovered themselves, and put it in the headline — cannot be served here. Not because the audience is quiet, but because the surface cannot see the moment where a delight would happen.

**The practical consequence.** Do not write a pleasant-surprise line for this brand. Until a review pipeline, a post-purchase survey, or agent call notes exist, delight claims should be routed to the pain, objection, trigger and jargon banks, which are genuinely full, and the proof should come from the problem side rather than the pleasure side.

## Surprise/delight phrases

Two records. **Neither describes the product**, and the heading exists so a later pass sees the blank rather than assuming the category was skipped.

Both are re-read here from `voc-outcome-phrase.md`, which captured them as outcome phrases on a stated and visible reading. That was the right call there and this is the right call here, and the difference is worth saying plainly rather than leaving as a duplicate. As outcomes, they are the product half-working: the consultation happened, the plan did not. **As surprises they are something better and more specific — both women expected an insurance agent to be useless and found him kind instead, and both said so after being told no.** The element of exceeded expectation is what this category is for, and it is stronger in these two records than the outcome reading was.

Source type is `ad-comment` on both, because it is the only source that exists. `review_id` is the Parker SQL `comment_id`. `url` is null because `permalink_url` is null on all 1,342 records. `identity_tag` and `behavioral_signal_tag` are null because `personas-profile.md` does not exist yet and this pass never invents a slug. Both are `thin`, and nothing here could reach `strong` under the single-source ceiling even if it were plentiful.

- snippet: Best advice I have gotten from an insurance agent! She didn’t have anything that fit but pointed me in the right direction!
  category: surprise_delight
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads Moms Nahuel WV#1 - V9 and Moms Nahuel WV#1 - V9 - Copy
    review_id: 45bc3e26-5d26-1d96-30c2-686ca6e5fbf8
    date: 2026-04-17
    url: null
  recurrence: 2 for the kind-agent surprise, which is the whole category
  source_diversity: [ad-comment]
  first_seen: 2026-04-01
  last_seen: 2026-04-17
  confidence: thin
  brand_self_echo: false
  notes: The clearest surprise in 1,342 records and it qualifies precisely because the core job failed. She says outright that nothing fit, so the good thing here cannot be the outcome she came for - it is entirely a benefit beyond it. "Best advice I have gotten from an insurance agent" is a comparative against every agent she has dealt with before, which is the exceeded-expectation signal this category is built on. Carries 2 likes, meaningful in a corpus where roughly three quarters of rows carry none. Denominator 1,342, so the kind-agent surprise runs at 0.15%. Echo false: no ad in the account uses "pointed me in the right direction" or anything near it, checked today against the transcripts of the ten highest-spend ads. Also captured in voc-outcome-phrase.md under the outcome reading; the two entries are the same record read through two lenses and the assembly pass should reconcile rather than double-count. Claims-check: usable only as service proof, never as proof that a plan was found. Voice-check in-voice.

- snippet: I was connected to a very helpful agent. They weren’t able to find a lower price for our particular situation but he was very kind and helpful and respectful.
  category: surprise_delight
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: df460383-699e-27a3-e2ef-e4f3197790f4
    date: 2026-04-01
    url: null
  recurrence: 2 for the kind-agent surprise
  source_diversity: [ad-comment]
  first_seen: 2026-04-01
  last_seen: 2026-04-17
  confidence: thin
  brand_self_echo: false
  notes: The other of the two, same shape, and the miss is stated even more plainly - they could not find a lower price. "Kind and helpful and respectful" is the phrase, and the three-word pile-up is the tell that she is describing something she did not expect rather than rating a service. The pattern across both records is worth naming as an inference: both women were told no and both praised the brand anyway, which is unusual enough that it is the second open loop below. Two records is a candidate and not a pattern, and the mining method's ten-record bar is nowhere near met, so it must never be written as a stable finding. Carries 1 like. Echo false - none of these words appear in any ad transcript. Also held in voc-outcome-phrase.md.

## Positives in this corpus that are not this brand's delights

Recorded with full attribution so the assembly pass sees they were found and correctly routed, rather than assuming they were missed or, worse, later mistaking one for this brand's proof. **Anyone quoting one of these as a Health For Moms surprise is misattributing it.**

- **"Wow this sounds better than my plan"** — row `23c73d99-a6b6-cd23-2de6-4567dcb5a64f`, ad `Internal Videos - OCT - B2 - Copy 3`, 2025-10-27. The only positive reaction to this brand's offer in the entire corpus, and it is a reaction to a claim in an ad, not to anything anyone received. It fails this category's own test, which turns on expectation being exceeded by an experience. Logged prominently because a later reader will find it and be tempted, and because it is the cleanest example of the identifier trap in this doc: the semantic tool returns `d1038ca4` for this row and the SQL `comment_id` is `23c73d99`.
- **"I was extremely shocked when I found out that they offered this. I didn't even know companies offered this level of health insurance."** — 2026-04-28, 3 likes. A genuine, textbook delight — about her employer's plan.
- **"you have excellent benefits at your job! This is not the norm."** — 2026-04-07, **7 likes**. The most-liked pleasant-surprise record in 1,342 and it is one woman congratulating another on her employer.
- **"Zero dollar copay but I do have a maximum out of pocket that's $3k per person... Highly recommend. Paid absolutely nothing for full body xray and ct after my wife had a dirt bike accident."** — row `862af0f0-f252-a0fc-50aa-b1b49f3f2623`, ad `MOMS39 - 2 - V2`, 2026-04-22. The only "highly recommend" in the corpus and it recommends her own existing plan. Already logged in `voc-outcome-phrase.md` for the same reason and repeated here because it is the single record most likely to be misread as a testimonial.
- **"When i realized the premium was NOT part of the deductible I was flabbergasted"** — 2026-04-13. A real surprise and a bad one. It belongs to `voc-pain-phrase.md`.
- **The three thank-yous, and where they point.** "Thank you" appears in 3 of 1,342 records and **every one of them thanks a fellow commenter rather than the brand**: `896950ce` thanking someone for correcting the ad and telling her to repeat it in the main thread, `ab8cce20` thanking someone for the same correction, `e38731a7` thanking someone for commiserating about a switch from Blue Cross to Cigna. `verified`. That is not a delight in this brand's product and it is not captured as one. It is recorded because it is the sharpest single line in this doc: **in 1,342 comments under its own ads, nobody has ever thanked Health For Moms.**

## The thing this corpus does have, named precisely so it is not mistaken for a delight

There is one real and recurring unexpected positive in these threads, and it is not about the product at all. It is that **strangers help each other here, at length, for nothing.**

The clearest case is a four-comment exchange under the ad `IMG 6` in January and February 2025. A woman mentions she beat chronic Lyme disease with food and herbs. Another woman, a stranger, asks where someone who has suffered for decades should turn. The first replies:

> "let me find my old notebook of everything I did to fight the chronic lyme... Let me look tomorrow, Friday and I'll get back to you no later than Saturday with info. Maybe we can call eachother over messenger, it's easier for me to talk than type all the information."

And two minutes later, unprompted:

> "I will also look up who may be available in your state that is a lyme specialist. The medical community is divided on lyme, which I'm sure you've found out. We'll get this figured out for you, hang in there, I promise there is hope!"

Rows `64ecc884-6f79-f5e4-04a1-d1a03e2160c9` and `e556576c-dea2-740d-2a1d-91a12cd3778c`, both 2025-02-07. `verified`.

It is not a one-off. A woman explains the TEFRA and Katie Beckett programs to another mother, in detail, ending "It is lots of papers to fill out but its state insurance! Good luck ❤️" — row `2d84a240-ebe1-dbe0-5eef-1bb3b4195f91`, 2026-03-26, 2 likes. Another walks a stranger through asking for the cash price and using a GoodRx card — row `39c8eb3c-911a-d885-bca3-e45234e9e590`, 2026-04-25, 2 likes. `voc-category-jargon.md` holds the eight-line unpaid glossary one commenter wrote for another.

**Why it is not captured as a snippet.** This prompt is specific: a surprise-and-delight phrase is an unexpected positive about the product or the experience of buying it. None of this is about Health For Moms. The brand did not do it, does not deliver it, and could not currently claim it. Promoting it into this doc's snippet list would be exactly the padding the mining method warns against, and it would hand a writer a testimonial the brand did not earn.

**Why it is here anyway.** It is the only genuinely warm thing happening in 1,342 records, it recurs across at least four separate threads spanning fourteen months, and it is happening inside space the brand pays for. That is worth a strategist's attention even though it is worth nothing to a copywriter today. It is the third open loop below.

Note the sharp contrast with the four "Pm me" records, which look superficially similar and are not: `f8b65ddb`, `37fc7787`, `95cdeab9` and `17d11a60` are all insurance sellers prospecting, three of them within four minutes of each other on 2026-04-07. Help from a peer and a pitch from a stranger read the same at a glance and are opposite things.

## Open loops

Three loops. None repeats a loop already filed in `voc-corpus-profile.md`, `voc-pain-phrase.md`, `voc-objection.md`, `voc-trigger-moment.md`, `voc-outcome-phrase.md`, `voc-anti-language.md`, `voc-metaphor.md`, `voc-aspirational.md`, `voc-category-jargon.md` or `source-pulls/brand-self-echo-detection.md`. In particular, the loop about what happens after the phone call is already filed in `voc-outcome-phrase.md` and is not repeated. The missing reviews, surveys and Reddit pull are infrastructure items and sit in `data_limitations` above rather than here, per the rubric.

**1. Nobody has ever thanked this brand in its own comment sections.**

"Thank you" appears three times in 1,342 records and all three thank another commenter — twice for correcting the ad. Across fourteen months, four thousand three hundred leads in the last ninety days alone and nearly forty thousand lifetime, not one person has come back to the ad to say the company did something good for her.

Pull: **Gap.** There is an enormous amount of completed activity here and no trace of gratitude anywhere in the record, and nothing has been done with that absence.

Question: Where do the women who had a good experience with this brand actually say so?

Why it matters: if they are saying it somewhere — a text thread with the agent, a friend, a Facebook group the brand does not run — that surface is the missing proof asset and finding it is cheaper than building a review pipeline. If they are saying it nowhere, the brand has a service problem it cannot currently see. **Routed to the brand**, because answering it needs partner-agency contact that no tool can reach. Territory: **Product.**

**2. The only two pleasant surprises in the corpus came from being turned down.**

Both records here are women who were told no. One says the agent "pointed me in the right direction," the other that he was "kind and helpful and respectful." Neither got a plan. Both left praise anyway.

Pull: **Surprise.** People who are told no do not normally stop to compliment the company that told them, and that is not what the setup would predict.

Question: What is the agent conversation giving these women that the product could not?

Why it matters: if the consultation has standalone value, the brand owns a service story it has never told and a proof asset that does not depend on a plan being found — which matters enormously for a business where a large share of applicants are disqualified. Two records is a candidate rather than a pattern, which is exactly why this is a question and not a recommendation. Territory: **Messaging.**

*Note: `voc-outcome-phrase.md` filed a loop from the same two records asking the same underlying thing. This is that loop arriving independently through a second lens, which the assembly pass should treat as corroboration rather than as two loops.*

**3. Strangers are doing real, unpaid care work inside space this brand pays for.**

A woman offers to dig out her old notebook and phone a stranger about chronic Lyme disease. Another walks a mother through the TEFRA and Katie Beckett programs. Another explains the entire deductible ladder in eight correct lines. None of it is about the product, all of it happens under paid placements, and it spans from January 2025 to the most recent months of the corpus.

Pull: **Resonance.** This is the only warm thing in 1,342 records, it keeps happening, and nothing in the brand's context explains why an insurance ad is where it lands.

Question: What is it about these ads that makes women stop and help a stranger?

Why it matters: whatever triggers it is producing the highest-quality engagement in the whole account, and it is currently an accident. If the brand understood it, it could build creative that invites the helping instead of triggering the correcting — which is the same behavior pointed at a much better outcome. Territory: **Messaging.**

## Sources

- Parker MCP `search_facebook_ad_comments_sql`, 17 filtered pulls on 2026-09-04. Every count here, including the four zero-return searches on the brand's own claimed product-experience phrases re-verified against the larger 1,342-record corpus, and the offset probe that re-pinned the total.
- Parker MCP `search_facebook_ad_comments_semantic`, two themed passes on 2026-09-04 aimed at unexpected positives, each reporting `totalCommentsAnalyzed 1342`. The pass that returned seven results at a deliberately loose 0.30 floor is the strongest single piece of evidence in this doc.
- Parker MCP `search_customer_reviews_sql` and `semantic_search_post_purchase_survey`, both 2026-09-04, both zero, both checked live. These are the two sources where delight language normally lives, and the survey is where the question that surfaces it directly would be asked.
- Parker MCP `search_facebook_ads_sql`, lifetime mode with the scripts block, 2026-09-04. The transcripts behind the read of which benefits the brand already markets, which is the only way to separate an organic surprise from a promoted benefit coming back, plus the lifetime lead and spend figures behind the pre-receipt argument.
- `source-pulls/brand-self-echo-detection.md`. The standing verdict on the three self-authored product-experience phrases and the fifteen-comment flood-of-calls warning, both carried forward and not re-judged, with the zero counts re-verified live here.
- `personas/voice-of-customer/voc-outcome-phrase.md`. The two service records this pass re-reads under a different lens, and the near-blank finding this pass independently re-tested rather than repeated.
- `personas/voice-of-customer/voc-objection.md`, `voc-pain-phrase.md`, `voc-trigger-moment.md`, `voc-anti-language.md`, `voc-metaphor.md`, `voc-aspirational.md`, `voc-category-jargon.md`. The sibling extractions holding the service complaints, the bad surprises and the unpaid glossary routed out of this pass.
- `running-notes/missing-context.md` and `running-notes/brand-rules.md`. The lead-generation account shape and the partner-agency phone call that together explain why this doc is a blank.
- `parker-system/creative-strategy-context/customer-review-mining-method.md`. The method this pass was performed through: the rule that a positive review is not a golden nugget, the exclusion of generic positive sentiment, the ten-record bar that keeps two records a candidate, the denominator discipline, the claims-check and voice-check governors, the brand-echo failure mode, and above all the rule that a blank beats a guess.
- `parker-system/creative-strategy-context/persona-research-and-creative-strategy-process.md`. The evidence ranking that puts post-purchase survey data at the top, which is precisely the source this category needs and this brand lacks, and the served-versus-buyer discipline behind the finding that nobody in this corpus has received anything.

Neither of the two method docs this pass routes to carries a required sign-off line, so none is stamped here. Stamping one they do not have would be a false proof-of-read.
