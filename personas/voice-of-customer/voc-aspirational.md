---
brand: health-for-moms
doc: voc-aspirational
category: aspirational
generated_on: 2026-09-04
refresh_by: 2026-10-04
live_pulls_run_on: 2026-09-04. Every Parker MCP call behind this doc ran today, against a corpus re-pinned live at 1,342 by my own offset probe. The earliest sibling docs ran on 2026-09-03 against 1,322 and say so; carried figures keep their 1,322 denominator and are labelled.
corpus_denominator: 1342 Facebook and Instagram ad comments, Meta ad account HealthForMoms, act 484897827497337
corpus_date_range: 2025-01-08 to 2026-09-03
prior_version: none. First run. No recurrence history to carry forward.
snippets_captured: 10
snippets_naming_a_personal_future_self: 4
sources_read:
  - Parker MCP search_facebook_ad_comments_sql, 19 filtered pulls on 2026-09-04, including the zero-return searches that are the evidence for what this audience never says. Every count and row id here was re-derived by me from the returned rows.
  - Parker MCP search_facebook_ad_comments_semantic, two themed passes on 2026-09-04 aimed squarely at desired-future and desired-self language. Both reported totalCommentsAnalyzed 1342. What they returned instead of aspiration is itself the main finding of this doc.
  - Parker MCP search_customer_reviews_sql, unfiltered, 2026-09-04. Returned totalReviews 0. Checked live by me.
  - Parker MCP semantic_search_post_purchase_survey, 2026-09-04. Returned totalResponsesForBrand 0 with the collection existing.
  - Parker MCP search_facebook_ads_sql, 2026-09-04, lifetime mode with the scripts block, top ten ads by lifetime spend. Read at full media depth to establish which aspirational identity the brand projects, so echo could be judged against the creative rather than an ad name.
  - source-pulls/brand-self-echo-detection.md, for the standing verdicts. The "wife of the year energy" finding is carried forward and re-verified live against the larger corpus, not re-judged.
  - personas/voice-of-customer/voc-corpus-profile.md, for field coverage, corpus bias and carried theme counts.
  - personas/voice-of-customer/voc-pain-phrase.md, voc-outcome-phrase.md, voc-objection.md, voc-trigger-moment.md, voc-anti-language.md and voc-metaphor.md, the sibling extractions, used to route present pain, realized results and situational triggers away from this pass.
  - running-notes/missing-context.md and running-notes/brand-rules.md.
  - parker-system/creative-strategy-context/customer-review-mining-method.md and persona-research-and-creative-strategy-process.md, the two methods this pass is performed through.
expected_sources_missing:
  - customer reviews. Zero rows, verified live 2026-09-04.
  - post-purchase surveys. Zero responses, verified live 2026-09-04. This is where "what were you hoping for" gets asked directly, and it is the single source this category most needs.
  - Reddit and forums. Not pulled. People describe the life they are trying to build to peers, with no brand projecting an aspiration onto them.
  - competitor and category reviews. No rival brands tracked in the Parker app.
  - brand-reputation, other-reviews, support tickets, organic social comments. None ingested.
  - personas-profile.md. Not yet written, so identity and behavioral-signal tags are null by rule.
data_limitations:
  - One source type only, so nothing here can rise above mixed under this prompt's confidence rule. Cross-source recurrence is what earns strong and this brand has one kind of source.
  - This is a thin doc and the thinness has a specific shape rather than being a general shortage. Only 4 of the 10 snippets name a personal future self. The other 6 are system-level wishes about how the category ought to work. That split is argued in full below and it should not be flattened by a later pass.
  - The surface actively suppresses this category. A comment under a paid ad is a public reply to a stranger's pitch, and people do not describe the self they are reaching for in that setting. They ask whether they qualify.
  - author_name and author_id are null on all 1,342 rows. Every count is a count of comments, never of people.
  - permalink_url is null on all 1,342 rows, so url is null on every snippet.
  - The semantic comment tool and the SQL comment tool return different identifier spaces for the same row. Every review_id below is the SQL comment_id, resolved by exact-text lookup where the snippet was first surfaced semantically. Three of the ten were surfaced semantically and none of their semantic ids matched the SQL id.
  - The database stores curly apostrophes, so a search written with a straight apostrophe silently misses rows. The "shouldn't" family was searched as "houldn" for that reason, which catches both spellings and the contraction-free form.
  - No commenter here is confirmed to have bought anything, so strictly these are the wants of people the algorithm served, not the wants of buyers.
  - refresh_by is 30 days rather than the 180-day voice-of-customer cadence, matching the sibling docs. This is the category most likely to change the day a survey pipeline is switched on.
  - There is no get_current_time tool on this MCP surface, so the date comes from the session clock.
---

# Voice of Customer — aspirational phrases — Health For Moms

## What this pass read, and the trap it had to avoid

This pass hunts the customer's own words for who she wants to become and what she wants her life to look like. The prompt is blunt about the risk sitting in this category, and it is the right warning for this brand specifically: aspiration is where a brand most tempts itself to project the customer it wishes it had onto the customer it actually has. `source-pulls/brand-self-echo-detection.md` already caught this brand doing exactly that in its context document, where twelve phrases the brand wrote for itself are filed under a heading that says customers said them.

So the discipline here was to capture only what a person actually typed, and to be plain when the answer is small.

The reading surface is one thing: **1,342 Facebook and Instagram ad comments** from Meta ad account `HealthForMoms`, act `484897827497337`, 2025-01-08 to 2026-09-03. I re-pinned that total myself today with an offset probe. Customer reviews returned zero rows live today. Post-purchase surveys returned zero responses live today. Reddit is not pulled.

One source means a hard ceiling. Cross-source recurrence is what this prompt says earns `strong`, and this brand has one kind of source, so **nothing below is `strong`** no matter how often it repeats. That is a fact about the corpus, not about the phrases.

And the account shape matters here more than in any other pass. Lifetime the account has produced **39,569 leads on $743,218.09 of spend at $18.78 each, and zero purchases**, because no purchase event exists. `verified` from the lifetime pull today. Nobody in this corpus is confirmed to have bought. So every want below belongs to a woman standing outside the product, which is actually the right place to catch an aspiration — she is at the point of consideration — but it also means none of it has been tested against what buying actually delivered.

## What this corpus does instead of aspiring

Here is the honest headline: **ask this audience what she wants and she asks you whether she is allowed in.**

That is not a figure of speech. I ran a semantic sweep across all 1,342 records for desired-future and desired-self language — what I want for my family, the life I want, I want to stop worrying, I want to feel secure. The top thirty results came back, and roughly two thirds of them are eligibility questions. "What if you're not a mom?" "Why do you have to be a mom???" "What about moms with adult children or children in college?" "Is this for single moms??" "What if I'm a mom, but my son is in college 🤔" "Markets to moms. Provides zero plans for moms. 🚩 Makes perfect sense." — that last one carries **15 likes**. `verified` from the returned rows.

That is the shape of the thing. The aspiration question comes back as a qualification question, and the qualification complaints already live in `voc-objection.md` where they belong.

**The string sweeps say the same.** Each of these is a case-insensitive substring search across all 1,342 records:

| String searched | Records | What they actually are |
|---|---|---|
| "I just want" | 2 | one real want, one greeting to a friend |
| "I wish" | 3 | one is a want, one is envy of a smaller deductible, one is a joke about lawsuits |
| "so I can" | 3 | none aspirational — two are questions about the form |
| "hope" | 3 | none about this category — two are strangers helping a woman with Lyme disease |
| "be able to" | 7 | one real want, the rest are policy arguments and brokers pitching |
| "wife of the year" | **0** | the brand's own aspirational identity, and nobody has ever said it |

**"Wife of the year" returning zero is the one to sit with.** It is the text hook on `Moms43 - 4 - V3` and its family, which took most of the last 90 days of spend and produced thousands of leads. The echo doc measured zero uses against 1,322 records on 2026-09-03. **I re-ran it today against 1,342 and it is still exactly zero.** `verified`. A brand can say a thing millions of times and have it come back never.

**Why the category is thin here, `inferred` from the surface itself.** A comment under a paid ad is a short public reply to a stranger's sales pitch. That setting rewards arguing, correcting, warning and asking whether you qualify. It does not reward describing the self you are reaching for, which is a private thing people say to peers or to a survey box. The mining method's source-coverage rule covers this exactly: a pass missing material sources is partial, and this one is missing the two sources — reviews and surveys — where aspiration normally lives.

## The two kinds of wanting this corpus does hold

What is here splits cleanly in two, and the split is the most useful thing in this doc.

### 1. The system-level wish. Louder, more repeated, and impossible for this brand to serve.

Six records ask for the whole category to be replaced. "Universal healthcare" appears in **5 of 1,342 records** and "socialized healthcare" in 1, across 5 distinct ads, 2025-07-23 to 2026-04-26. `verified`. The loudest of them carries **7 likes**:

> "This is why we need universal healthcare."

And one of them is aimed straight at this brand's positioning, which makes it the sharpest record in the doc:

> "We need to get rid of insurance companies and invest in single payer, universal healthcare. We don't need more "more compassionate" insurance companies."

Read that second sentence again. Health For Moms is, in its own creative, a more compassionate insurance option — an insurer built for moms that actually has your back. She names that exact pitch and refuses it as a category, not as a product.

**The strategic read, `inferred`:** the clearest thing this audience says about the future she wants is that she does not want to be shopping for insurance at all. That is a real aspiration, it is the most-liked one here, and there is no version of this brand's offer that satisfies it. A writer who reaches into this bank for "what she wants" and pulls this will write an ad that argues with its own product.

### 2. The personal future self. Four records, and they are quiet.

Only four snippets in 1,342 name a future self or a future life in the customer's own words. Four. Here they are in one place, because a reader should see how small the pile is:

- "My family isn't done growing." — a woman explaining why the exclusion for planning a pregnancy shuts her out.
- "it would be great to be able to travel and not have to worry about only being in your hometown to be able to go to the doctor" — 3 likes.
- "I just want insurance for me and one child without having to pay for a whole family plan."
- "I'm currently in school now so that one day I can have a good paying job with good insurance again" — and this one is from a father, not a mother.

**What they have in common, `inferred`:** not one of them wants a feeling. They want a shape of life — a growing family, the freedom to leave town, a household of two counted as two, a job good enough to carry its own insurance. The brand's own aspirational register runs the other way, toward states of mind: peace of mind, rest easier, no more worrying. `source-pulls/brand-self-echo-detection.md` verified those outcome phrases at zero in the customer record, and this pass now shows why the miss is structural rather than accidental. **The brand sells a feeling. The four women and one man who said what they want asked for a circumstance.**

### The near-miss family: "should," not "I want."

Sitting between those two kinds is a small group that states how the world ought to work without naming a self. "Health insurance shouldnt cost you a fortune. PERIOD." "I think if we pay for health insurance, we shouldn't have a deductible." Five records match the "houldn" search and three of them are this shape.

I captured two of them and I want the reason visible, because this is the judgment call in the doc. The prompt says the absence of a pain is not on its own an aspiration. A pure complaint about a deductible would fail that test and belongs to `voc-pain-phrase.md`. But these two do something a complaint does not: they describe a state of affairs the speaker wants to exist, in the positive, unprompted. That is a desired future framed as a hope, which is what this category is for. They are marked `mixed` and their notes say plainly that they are category-level rather than identity-level.

## Aspirational phrases

Ten snippets. Source type is `ad-comment` on every one, because it is the only source that exists. The `platform` line carries the ad the comment sits under. `review_id` is the Parker SQL `comment_id`, resolved by exact-text lookup wherever a row was first surfaced semantically. `url` is null on all ten because `permalink_url` is null on all 1,342 records. `identity_tag` and `behavioral_signal_tag` are null on all ten because `personas-profile.md` does not exist yet and this pass never invents a slug.

Every `snippet` line is `stated` and exact. Every count is `verified` as a string check anyone can re-run. Every read is `inferred` and says so. Nothing is `strong`, per the single-source ceiling.

- snippet: Why can’t you get this if you want another kid? I don’t know when I’m gonna have another kid, but I do know I want another kid. My family isn’t done growing.
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: de24f387-6146-3d93-36f7-ce3df523a9fb
    date: 2026-04-22
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-22
  last_seen: 2026-04-22
  confidence: thin
  brand_self_echo: false
  notes: The best aspirational phrase in 1,342 records and it is worth the whole pass on its own. "My family isn't done growing" names a future life in five words, and it does it while she is being told she does not qualify, which is what gives it force - the aspiration and the rejection are in the same breath. One record, so thin, and it must never be presented as a pattern. Denominator 1,342. The exclusion complaint around it belongs to voc-objection.md, which already holds the pregnancy-eligibility cluster; only the want is captured here. Claims-check clear as customer self-description. Voice-check in-voice - it is warm, plain and unpolished, which is the register the brand's guidelines describe. Strongest headline candidate in this doc. A trailing object-replacement character in the stored row was dropped from the snippet; nothing else was changed.

- snippet: You know it would be great to be able to travel and not have to worry about only being in your hometown to be able to go to the doctor if there’s an emergency or you’re visiting for a long period of time at least be able to go to the urgent cares
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads Moms Nahuel WV#1 - V9 and Moms Nahuel WV#1 - V9 - Copy
    review_id: 7d41203a-6335-bf85-93fa-c7fadc338e92
    date: 2026-04-15
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-04-15
  last_seen: 2026-04-15
  confidence: thin
  brand_self_echo: false
  notes: The only record in the corpus that describes a wanted day rather than a wanted number, and it carries 3 likes in a corpus where roughly three quarters of rows have none. The want is freedom of movement - being able to leave your town without leaving your coverage behind. Notable because the brand's own top-spending script promises exactly this, "nationwide coverage that truly protects your family" and "the freedom to choose your own doctors, specialist without restrictions," verified from the B1 samar- Copy transcript. Echo false all the same: she is stating the want in her own words with no phrase overlap, and the network-restriction complaint is a well-worn category grievance that voc-objection.md tracks independently. One record, thin. Claims-check gated - nationwide access is a specific product claim and this phrase should not be used to imply it without substantiation.

- snippet: I just want insurance for me and one child without having to pay for a whole family plan.
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad Moms36 - 3 - A - 2 - V4a
    review_id: 270c3096-0d86-0259-bf00-6d48b423e338
    date: 2026-06-01
    url: null
  recurrence: 1 exact, 2 for the "I just want" string of which only this one is a want
  source_diversity: [ad-comment]
  first_seen: 2026-06-01
  last_seen: 2026-06-01
  confidence: thin
  brand_self_echo: false
  notes: A small, precise want and the most actionable one here, because it names a product shape rather than a feeling: a household of two, priced as two. It sits on a different creative family from most of this doc, which is worth noting in a corpus this ad-skewed. The underlying idea recurs elsewhere in different words - "What if I'm a mom, but my son is in college," "What about moms with adult children" - but those are eligibility questions and are held by voc-objection.md, so recurrence is recorded as 1 for the want as stated. One record, thin. Claims-check clear. Voice-check in-voice.

- snippet: I’m currently in school now so that one day I can have a good paying job with good insurance again
  category: aspirational
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
  notes: The only record in the corpus that names a future self reached by a plan the speaker is already executing - back in school, aiming at a job that carries insurance. "Again" is the load-bearing word: this is a want to return to something lost, not to reach something new, which is a different emotional shape from anything else in the doc. The speaker is a father, and 96.1% of this account's lifetime spend delivers to women, so he is off-persona. That is recorded rather than smoothed over: the corpus's clearest statement of an aspiration reached through effort comes from the demographic the brand does not address. The same comment supplies the only self-directed simile in voc-metaphor.md. Snippet trimmed to the aspiration. Voice-check transformable.

- snippet: This is why we need universal healthcare.
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V2
    review_id: bb851402-3cbc-6d0e-7497-bb9f6c2cc3de
    date: 2026-04-26
    url: null
  recurrence: 6 for the system-replacement wish - 5 for "universal healthcare" and 1 for "socialized healthcare"
  source_diversity: [ad-comment]
  first_seen: 2025-07-23
  last_seen: 2026-04-26
  confidence: mixed
  brand_self_echo: false
  notes: The most-liked aspirational statement in the corpus at 7 likes, and the most repeated. Denominator 1,342, so the system wish runs at 0.45% across 5 distinct ads and spans fourteen months, which makes it the only aspiration here that survives the corpus time skew. Captured as aspirational rather than routed to objection because it is a positive statement of a wanted future rather than a complaint about the present. It is also the aspiration this brand can least serve, and that is the point of capturing it - a writer needs to see it so they do not accidentally write toward it. Claims-check unusable for copy. Its value is strategic, not liftable.

- snippet: We need to get rid of insurance companies and invest in single payer, universal healthcare. We don't need more "more compassionate" insurance companies.
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad OMC - C11 - 2b
    review_id: 5b252400-94b4-fe51-ee63-495a40cd0dba
    date: 2026-03-12
    url: null
  recurrence: 1 exact, 6 for the system-replacement wish
  source_diversity: [ad-comment]
  first_seen: 2026-03-12
  last_seen: 2026-03-12
  confidence: mixed
  brand_self_echo: false
  notes: The sharpest record in this doc, and it is captured whole because the second sentence is the finding. She names this brand's exact positioning - a kinder insurance company for a group nobody serves well - and rejects the category rather than the product. Her scare quotes around "more compassionate" are hers, kept exactly. This is the clearest evidence in the whole library that a segment of the served audience is not shoppable at any price or with any message, which is a targeting question rather than a copy question. Marked mixed because it belongs to a six-record family rather than standing alone. Not liftable. Routes to the persona and messaging work, not to a writer.

- snippet: we should all just have socialized healthcare.
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad B1 samar- Copy
    review_id: 0bb56fef-8bb4-8bf6-1cce-06a292d0bb80
    date: 2025-07-23
    url: null
  recurrence: 1 exact, 6 for the system-replacement wish
  source_diversity: [ad-comment]
  first_seen: 2025-07-23
  last_seen: 2026-04-26
  confidence: mixed
  brand_self_echo: false
  notes: The earliest system wish in the corpus and the anchor for the first_seen date on the whole family, which is what shows the wish is not an artifact of the spring 2026 comment surge. Snippet trimmed to the aspiration; the rest of her comment holds the best-written sentence in the corpus and is captured in voc-metaphor.md for its alliteration and its stuck-in-a-rut image. Same claims-check as the two above: strategic, not liftable.

- snippet: Health insurance shouldnt cost you a fortune. PERIOD.
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ads MOMS39 - 2 - V2 and MOMS39 - 2 - V2 - Copy
    review_id: f566d1d8-95e5-71bd-d0f9-8f0c540f87fc
    date: 2026-04-28
    url: null
  recurrence: 5 for the "houldn" family, 3 of them stating a wanted state of affairs
  source_diversity: [ad-comment]
  first_seen: 2026-03-22
  last_seen: 2026-05-04
  confidence: mixed
  brand_self_echo: false
  notes: The judgment call in this doc, made in the open. It is a normative statement about the category rather than a personal future self, and the prompt is clear that the absence of a pain is not on its own an aspiration. It is captured because it states a wanted state of affairs in the positive and unprompted, which is the test this category actually runs. Read it as category-level, never as identity-level, and do not let a later pass promote it into a persona want. The all-caps PERIOD and the missing apostrophe are hers. This is the closest thing in the corpus to a phrase the brand could adopt directly, which is also exactly why the echo flag needs watching on the next run: if the brand starts saying it, later customer uses stop being evidence.

- snippet: I think if we pay for health insurance, we shouldn’t have a deductible
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V3
    review_id: 724f34e4-47df-48c7-51ba-dba35561db5f
    date: 2026-03-22
    url: null
  recurrence: 5 for the "houldn" family, 3 stating a wanted state of affairs
  source_diversity: [ad-comment]
  first_seen: 2026-03-22
  last_seen: 2026-05-04
  confidence: mixed
  brand_self_echo: false
  notes: The earliest of the three normative wants and the one that lands nearest the product, since a zero-dollar deductible is precisely what the brand sells. That proximity is a risk rather than a win. The deductible framing is already settled in source-pulls/brand-self-echo-detection.md as 95.2% concentrated inside an 83-day window the brand's own creative opened, so a want expressed in the brand's own vocabulary, in a window the brand created, is weak evidence of an organic aspiration. Echo is marked false because "if we pay for health insurance we shouldnt have a deductible" is her own construction and appears in no ad transcript, but the surrounding concentration is why this is mixed and not stronger. Category-level, not identity-level.

- snippet: I wish I had the money to make a for dad’s or men only insurance company! My ex-husband worked hard until his body broke! Why doesn’t he get help?
  category: aspirational
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook or Instagram, Meta ad account act 484897827497337, ad MOMS38 - 1 - V1
    review_id: 54d534aa-6273-934b-7ce2-35dcb21892f0
    date: 2026-03-30
    url: null
  recurrence: 1
  source_diversity: [ad-comment]
  first_seen: 2026-03-30
  last_seen: 2026-03-30
  confidence: thin
  brand_self_echo: false
  notes: An aspiration pointed at someone else, which is why it is unusual enough to capture. She is not naming a self she wants to become; she is naming a thing she wishes existed for her ex-husband, and the emotional detail - worked hard until his body broke, split because he became too mean, still not happy about his options - makes it one of the most human records in 1,342. Its strategic value is a lens the account has never used: this brand's audience contains women who are advocating for men. Snippet trimmed to the want and its reason. One record, thin. Voice-check off-voice. Not liftable, but the observation is real.

## Wanting that exists in this corpus and belongs to somebody else

Recorded with full attribution so the assembly pass sees it was found and correctly routed, rather than assuming it was missed or, worse, later mistaking one of these for this brand's aspiration.

- **"Affordable insurance that actually works still exists in plenty avenues even for those with high income. You just have to work with brokers that care and are knowledgeable enough to show you the right products."** — row `a8a56981-cb20-bdb1-b456-ebd07cabc132`, 2026-05-20, **6 likes and 5 replies**. This is a rival broker prospecting inside the brand's comment section, and "insurance that actually works" is nearly word for word the brand's own closing line, "get coverage that actually works," from the `MOMS39` and `Moms43` scripts. It is competitor copy, not customer aspiration, and anyone quoting it as customer language is misattributing it badly.
- **"I promise the premiums and copays are worth the peace of mind that a bad diagnosis won't steal everything you and your loved ones have built."** — row `4da1389b-0d84-386d-1dac-89a3a877597a`, ad `MOMS38 - 1 - V3`, 2026-03-25. The most eloquent statement of what insurance is *for* in the corpus, and it is an argument against the account's premise, written by a woman defending the system the ad is attacking. The echo doc already settled that "peace of mind" is category-standard language rather than lifted, and the mining method rules it out as generic positive sentiment anyway.
- **"But Mexico has free universal health care before USA. Let that sink in."** — row `673a0cc6-9024-5a6c-70cd-900cbee9b1ca`, ad `MOMS38 - 1 - V2`, 2026-04-15, and **"This is why there are people that go to other countries every 6 months for dental and physicals... My friend goes to Colombia every 6 months."** — row `d01c0343-002c-28e0-32e0-5b7caa9b690a`, ad `MOMS38 - 1 - V3`, 2026-04-25. Both describe a better arrangement located somewhere other than here. They are the system wish with a passport, and they route to the same strategic conclusion rather than to a copy bank.
- **The affordability numbers, for scale.** "Afford" in any form appears in 47 of 1,342 records, "affordable" in 23, and the negative construction "t afford" in 17. `verified`. That is the single largest want-adjacent cluster in the corpus by a distance, and almost none of it is aspirational under this prompt's definition — it is people saying they cannot pay, which is present pain and lives in `voc-pain-phrase.md`. It is recorded here so a later reader does not look at the ten small snippets above and conclude the corpus is quiet. It is not quiet. It is loud about what she cannot have and near-silent about what she is reaching for.

## Open loops

Three loops. None repeats a loop already filed in `voc-corpus-profile.md`, `voc-pain-phrase.md`, `voc-objection.md`, `voc-trigger-moment.md`, `voc-outcome-phrase.md`, `voc-anti-language.md`, `voc-metaphor.md` or `source-pulls/brand-self-echo-detection.md`. The missing surveys, missing reviews and missing Reddit pull are infrastructure items and sit in `data_limitations` above rather than here, per the rubric.

**1. The loudest thing this audience wants is for the whole category to stop existing.**

Six records ask for universal or socialized healthcare, across five ads and fourteen months, and the most-liked of them carries 7 likes. One of them names this brand's exact pitch — a more compassionate insurance company — and refuses it as a category. Against that, only four records in 1,342 name a personal future the brand could actually sell toward.

Pull: **Surprise.** A comment section under an insurance ad would be expected to hold people wanting better insurance, and instead its clearest collective want is for insurance to be replaced.

Question: How much of the audience this account reaches is unwinnable at any price or with any message?

Why it matters: if a real share of delivery is going to people who reject the category rather than the product, that is a targeting problem the creative cannot fix, and every dollar spent persuading them is spent arguing. Territory: **Personas.**

**2. The four women who said what they want asked for a circumstance, and the brand sells a feeling.**

The personal wants in this corpus are a growing family, the freedom to travel without losing coverage, a plan priced for a household of two, and a job good enough to carry its own insurance. The brand's aspirational register is peace of mind, rest easier, no more worrying — and all four of those phrases return zero in the customer record, re-verified live.

Pull: **Tension.** Two accounts of what this customer is buying toward sit side by side and cannot both be the working one.

Question: What does a mom picture herself doing differently on the day after her coverage problem is solved?

Why it matters: it decides whether the creative should promise a calmer mind or a specific unlocked circumstance, and the account has never tested the second. Territory: **Messaging.**

**3. The brand's biggest aspirational identity has been said millions of times and come back zero times.**

"Wife of the year energy" carries the text hook on the family that took most of the last 90 days of spend. The literal string appears in 0 of 1,342 comments, and I re-verified that today against twenty more rows than when the echo doc first measured it. Meanwhile the one identity the audience does raise unprompted is who counts as a mom at all — dozens of records asking whether a mom of a college student, a mom who might get pregnant, a dad, or a woman with no kids is allowed in.

Pull: **Gap.** There is an enormous amount of identity language in this account's creative and an entirely different identity argument happening underneath it, and nothing has connected the two.

Question: Who does this audience think this product is for?

Why it matters: the brand is selling a flattering identity, "wife of the year," while the audience is arguing about a membership rule, who counts as a mom. If the real identity question is belonging rather than achievement, the whole aspirational lane is aimed at the wrong emotion. Territory: **Personas.**

## Sources

- Parker MCP `search_facebook_ad_comments_sql`, 19 filtered pulls on 2026-09-04. Every count, row id and ad name here, including the zero return on "wife of the year" re-verified against the larger 1,342-record corpus, and the offset probe that re-pinned the total.
- Parker MCP `search_facebook_ad_comments_semantic`, two themed passes on 2026-09-04 aimed at desired-future and desired-self language, each reporting `totalCommentsAnalyzed 1342`. What these returned — eligibility questions rather than aspirations — is the central evidence for this doc's shape.
- Parker MCP `search_customer_reviews_sql` and `semantic_search_post_purchase_survey`, both 2026-09-04, both zero, both checked live. The survey is the source this category most needs and this brand has none.
- Parker MCP `search_facebook_ads_sql`, lifetime mode with the scripts block, 2026-09-04. The transcripts behind the read of which aspirational identity the brand projects, including "the freedom to choose your own doctors" and "coverage that actually works," plus the lifetime lead and spend figures.
- `source-pulls/brand-self-echo-detection.md`. The standing verdicts, carried forward and not re-judged: the twelve brand-authored phrases in the context document's customer-language section, and the "wife of the year energy" absence, which this pass re-verified live rather than repeating.
- `personas/voice-of-customer/voc-corpus-profile.md`. Field coverage, corpus bias and the carried theme counts on a 1,322 denominator.
- `personas/voice-of-customer/voc-pain-phrase.md`, `voc-outcome-phrase.md`, `voc-objection.md`, `voc-trigger-moment.md`, `voc-anti-language.md`, `voc-metaphor.md`. The sibling extractions holding the present pain, realized results, eligibility complaints and images routed out of this pass.
- `running-notes/missing-context.md` and `running-notes/brand-rules.md`. The dark-surface substitution rule and the lead-generation account shape.
- `parker-system/creative-strategy-context/customer-review-mining-method.md`. The method this pass was performed through: the exclusion list that rules out generic positive sentiment, the brand-echo failure mode this category is most exposed to, the denominator discipline, the claims-check and voice-check governors, the source-coverage rule that marks a pass partial when material sources are absent, and the rule that a blank beats a guess.
- `parker-system/creative-strategy-context/persona-research-and-creative-strategy-process.md`. The identity-first doctrine behind the read that these wants are circumstances rather than feelings, and the served-versus-buyer discipline behind the note that every voice here belongs to someone the algorithm served.

Neither of the two method docs this pass routes to carries a required sign-off line, so none is stamped here. Stamping one they do not have would be a false proof-of-read.
