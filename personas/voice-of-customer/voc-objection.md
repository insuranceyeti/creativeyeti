---
brand: health-for-moms
doc: voc-objection
category: objection
generated_on: 2026-09-04
refresh_by: 2026-10-04
live_pulls_run_on: 2026-09-03. The session spanned the date rollover; every Parker MCP call in this doc was made on 2026-09-03 and the corpus end date is that same day.
corpus_denominator: 1322 Facebook and Instagram ad comments, Meta ad account HealthForMoms, act 484897827497337
corpus_date_range: 2025-01-08 to 2026-09-03
prior_version: none. First run. No recurrence history to carry forward.
sources_read:
  - Parker MCP search_facebook_ad_comments_sql, twelve filtered passes on 2026-09-03. Every count in this doc was re-derived by me from the returned rows, not carried from an upstream doc.
  - Parker MCP search_facebook_ad_comments_semantic, five passes on 2026-09-03, each reporting totalCommentsAnalyzed 1322, which agrees with the SQL denominator.
  - Parker MCP search_customer_reviews_sql, unfiltered, 2026-09-03. Returned totalReviews 0.
  - Parker MCP semantic_search_post_purchase_survey, 2026-09-03. Returned totalResponsesForBrand 0, collection exists.
  - personas/voice-of-customer/voc-corpus-profile.md, the measured spine for denominators, field coverage and corpus bias.
  - source-pulls/ad-comments.md, the full-corpus persona read of the same 1,322 rows. Used as a claim to check against, not as a count to trust.
  - running-notes/missing-context.md, running-notes/brand-rules.md, running-notes/success-definition.md.
  - parker-system/creative-strategy-context/customer-review-mining-method.md and persona-research-and-creative-strategy-process.md, the two methods this pass is performed through.
sources_missing:
  - customer reviews. Zero rows, verified live 2026-09-03.
  - post-purchase surveys. Zero responses, verified live 2026-09-03. This is the top of the evidence rank and it is empty.
  - Reddit, forums and community. Not pulled for this brand.
  - competitor and category reviews. No rival brands tracked in the Parker app.
  - third-party and retail reviews, support tickets, organic social comments. None ingested.
  - personas-profile.md. Not yet written, so no identity or behavioral-signal slug exists. Every tag in this doc is null by rule, not by oversight.
data_limitations:
  - One source type only. Under this prompt's own confidence rule, cross-source recurrence is what earns strong, so no objection in this doc can rise above mixed no matter how often it repeats.
  - These are publicly performed objections. They are not the same thing as the private hesitation that stops a purchase, and the difference is argued in full below.
  - author_name and author_id are null on all 1,322 rows. Every count here is a count of comments, never a count of people.
  - permalink_url is null on all 1,322 rows, so no snippet can carry a link. Verification runs through the row id and the tool.
  - No join exists between any comment and the 4,336 leads the account produced in the last 90 days. Nothing here can be said to have cost a lead.
  - 846 of 1,322 comments, 64.0%, sit in March and April 2026, and 795 of 1,322, 60.1%, sit on the MOMS38 - 1 creative family. Ad spread is the more durable number than raw count and is carried on every cluster.
  - Two clusters below are floors rather than totals, and each says so on its own line: the deductible correction and the state exclusion.
---

# Voice of Customer — objection phrases — Health For Moms

## What this pass read, and what the reader should hold before reading a single quote

I read one source, because one source is all this brand has. Customer reviews returned zero rows when I called the tool on 2026-09-03, unfiltered. Post-purchase surveys returned zero responses on the same day, with the collection existing and empty. Those are not broken pipes and they are not thin piles. They are blanks, and I checked both live rather than trusting the note in `running-notes/missing-context.md`. `verified`.

So the whole objection set below comes from 1,322 Facebook and Instagram ad comments on the Meta ad account HealthForMoms, act 484897827497337, dated 2025-01-08 through 2026-09-03, the day the pulls ran. I pinned that denominator myself instead of accepting it: an offset probe at 1,321 returned exactly one row, the oldest comment in the corpus, and offset 1,322 returned nothing at all. Five semantic passes each reported `totalCommentsAnalyzed: 1322`. Two tools, same number. `verified`.

**These ad comments are not this brand's review corpus and must never be presented as one.** Anywhere downstream that a doc says "customers said," the honest sentence for Health For Moms is "commenters under the brand's paid ads said."

Now the part that decides how much weight every snippet below can carry.

**For an objection pass, this surface is an advantage. Say the advantage out loud, and say its limit in the same breath.** The persona method ranks customer evidence with post-purchase survey data at the top and public comments near the bottom, and this brand holds only the bottom rank. For most Voice of Customer work that is a crippling handicap. For objections it is not, because a public comment section is where doubt goes to be performed. People come under an insurance ad to argue, correct, warn strangers, and be seen agreeing. That selection bias, which ruins an outcome pass, is exactly what fills an objection pass. The corpus profile put it plainly and it is right: this is the richest section the corpus has.

**The limit is real and it is not a footnote.** A publicly performed objection and a private hesitation are two different things, and they diverge in three ways I can see in the data itself.

First, a public objection is written for an audience. Nine of the pregnancy comments below open by quoting the brand's own name back at it before making the point, which is a rhetorical move, not a shopping thought. Nobody thinks in air quotes.

Second, the public surface over-selects for the objector who will never buy under any wording. The self-insurers, the political reactors, and the rival agents are all here in volume, and none of them is a lost sale. The corpus holds 33 comments arguing you should drop insurance entirely and 39 where a competing agent pitches his own book of business. Answering those objections in copy would be answering people who are not customers.

Third, and most important, the quiet objection leaves no trace here. A woman who watched the ad, thought "I'll get buried in sales calls," and scrolled past wrote nothing. The 17 comments about the call flood below are the loud tail of something that is almost certainly much larger and completely uncountable from this surface. So treat every count in this doc as a floor on the doubt and never as its size.

**One structural consequence, stated up front so nobody has to hunt for it.** This prompt's confidence rule reserves *strong* for cross-source recurrence, *mixed* for single-source recurrence, and *thin* for a one-off or a suspected brand echo. Health For Moms has exactly one source type. So the ceiling on this entire document is **mixed**, and an objection appearing 42 times across 17 different ads still earns mixed rather than strong. That is not me hedging. It is the rule applied honestly to a brand whose top two evidence tiers are empty.

## How I re-derived the counts, and where I landed differently from upstream

The brief named five objection clusters found upstream and told me to verify them independently rather than repeat them on trust. I did that with twelve filtered SQL pulls and five semantic passes, reading and classifying every returned row myself against the mining method's exclusion list. Here is what I found, and where my numbers differ from `source-pulls/ad-comments.md`.

| Objection cluster | My count | My ad spread | Upstream said | Read on the gap |
|---|---|---|---|---|
| Pregnancy and maternity exclusion | 36 comments, 2.7% of 1,322 | 15 ad names | 42 across 15 | Spread matches exactly. My count is stricter: I dropped four rows that mention pregnancy while describing their own existing plan rather than doubting this one. |
| The hook's central term corrected | at least 51 comments, 3.9% | 8 ad names | 103 across 13 | **Floor, not total.** Mine counts only rows carrying the exact strings "out of pocket" or "OOP." 207 rows, 15.7%, contain "deductible," and I did not classify all 207 row by row. Upstream's larger number is the superset and is consistent with mine. |
| Pre-existing condition screening | 42 comments, 3.2% | 17 ad names | 55 across 17 | Spread matches exactly. My count is stricter on the same principle. |
| My state is not on the list | at least 15 comments, 1.1% | 5 ad names | 19 across 8 | **Floor, not total.** Semantic recall, not an exact-string count, because there is no reliable string for it. |
| Buried in calls after the form | 17 customer comments plus 1 rival agent, 1.3% | 10 ad names | 15 across 10 | Spread matches exactly. My count is slightly higher because I combined the string pass with a semantic pass and picked up four rows that never use the word "call." |

Two things about that table matter more than the individual rows.

**The spreads reproduce almost perfectly and the raw counts do not.** Three of five clusters landed on the identical number of distinct ads, independently derived. That is the strongest internal check available in a single-source corpus, and it tells you the mining method is right that spread beats raw count. A count moves with how strictly you classify. A spread does not.

**I also found three objections that appear on neither the brand's stated list nor the upstream cluster list.** A silent rejection at the qualifier, an income floor, and a friction objection about being forced to hand over a phone number to see any price at all. Those are in the set below.

## The brand's own objection list, checked against the record

The brand context document names five objections it believes it handles: is this legit, I do not want to get on a call and be sold to, I do not have time, my state probably is not included, and I should just wait for open enrollment. I checked all five against the corpus by string and by meaning.

Three of the five are really there. Legitimacy is there, with 45 records containing "scam," 3.4%, though most aim at the insurance category rather than at this brand. The sales-call objection is there and is one of the highest-liked things in the corpus. The state objection is there, though smaller than the others.

**Two of the five are close to invisible.** "Open enrollment" appears in exactly 1 of 1,322 records, 0.1%, and "enrollment" in any form appears in 2, 0.2%. I pulled both rows and read them. Neither is a customer saying she will wait. One is a commenter telling another commenter that a signup window exists. The other is a peer explaining that marketplace plans are guaranteed issue. `verified`. The time objection is similarly absent as a stated doubt.

Meanwhile the two widest objections in the brand's own comment sections, the pregnancy exclusion at 36 comments across 15 ads and the pre-existing screen at 42 across 17, are on no stated list at all. That is a real gap between what the brand thinks stops the buyer and what the record shows her typing, and it is the single most useful thing this pass produces.

One caution the persona method demands and I am applying: the served audience is not the buyer. Everything above describes people Meta served an ad to. Whether any of these doubts stops an actual purchase cannot be known from here, because no buyer source exists for this brand.

---

## Objection phrases

### Cluster one — the name promises what the product excludes

**The evidence walk.** I pulled every row containing "pregnan," which returned 38, then every row containing "maternity," which returned 4, then caught one more phrased as "expecting" through the eligibility pull. I read all of them in full rather than skimming headlines, because the mining method warns the usable line usually sits mid-comment. I dropped four rows that mention pregnancy while describing the commenter's own existing plan, since a complaint about the problem is a pain phrase and not a doubt about this product. That left **36 comments across 15 distinct ad names, running 2025-07-01 to 2026-06-09**, which is fourteen months and five separate creative families. It survives every creative refresh in the corpus. `verified` on the count and the spread, both re-derived today.

The reason this is load-bearing and not a complaint log: the brand's name is the setup for the objection. Nine of the 36 open by quoting "Health for Moms" back at the ad before making the argument. Two rival agents use the same exclusion as a sales wedge in the brand's own thread. And the qualifier apparently asks about intent as well as state, which creates an edge case the funnel generates and nobody answers.

My read, marked `inferred`: the underlying concern is not really about maternity coverage. It is a trust judgment. A woman who reads the name as a promise and then gets screened out concludes the brand was never honest with her, and she says so in front of everyone else scrolling the ad. That is why the phrasing runs to "false advertising" and "disgusting tactic" rather than to "do you have a maternity plan."

```yaml
- snippet: How can you have healthcare for moms if you don’t cover maternity? Makes zero sense. False advertising.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 3b2ac139-83f3-123e-bd63-6321ff80f4d4
    date: 2025-08-12
    url: null
  recurrence: 36
  source_diversity: [ad-comment]
  first_seen: 2025-07-01
  last_seen: 2026-06-09
  confidence: mixed
  brand_self_echo: false
  notes: >
    Denominator 1,322 comments, so 36 is 2.7%, spread across 15 distinct ad names and five creative
    families over fourteen months. Underlying concern, my inference: this reads as a verdict on the
    brand's honesty rather than a coverage question, which is why the words reach for false
    advertising. Confidence capped at mixed because one source type cannot earn strong under this
    prompt's rule. Ceiling is mixed for every entry in this doc for the same reason.
```

```yaml
- snippet: Health for Moms, but only if your babies are out of the womb. I was denied for being pregnant. Scam.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: a04168ce-2e0e-2ceb-7992-d6427575062f
    date: 2026-02-03
    url: null
  recurrence: 36
  source_diversity: [ad-comment]
  first_seen: 2025-07-01
  last_seen: 2026-06-09
  confidence: mixed
  brand_self_echo: false
  notes: >
    A distinct phrasing of the same doubt, kept separate because the wording is what a writer lifts.
    This one carries a first-hand denial rather than an inference from the form, which makes it the
    strongest single piece of evidence in the cluster. Claims-check: unusable as a claim, since the
    brand cannot repeat it. Usable only as the objection a script answers head on.
```

```yaml
- snippet: One question literally asks if you are pregnant or planning to be pregnant? The answer choices are no and I’m not planning to be or yes I’m pregnant. I’m not pregnant but I’m planning to be. So I picked yes pregnant and it says there are no plans. You would think if it is advertising as a mom insurance company then pregnancy status should not matter.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: a8f8a46c-9484-ad65-fcc5-28e9f8ebb25c
    date: 2026-02-08
    url: null
  recurrence: 36
  source_diversity: [ad-comment]
  first_seen: 2025-07-01
  last_seen: 2026-06-09
  confidence: mixed
  brand_self_echo: false
  notes: >
    The most precise record in the cluster. She narrates the exact qualifier screen and the exact
    dead end it produced. This is a whole-review concept candidate in the mining method's sense: the
    full arc, from clicking through to being turned away by a question about a future she has not
    lived yet, maps to a producible ad if the product ever changes. A resolution exists nowhere in
    the thread; the brand does not answer.
```

```yaml
- snippet: Plans not available for those that don’t plan or can’t get pregnant anymore bc of an unexpected hysterectomy last year  - yet have kids already… (health for moms) makes sense 👍🏼
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 7a742fa2-fc66-940e-3000-b682cf371251
    date: 2026-04-08
    url: null
  recurrence: 36
  source_diversity: [ad-comment]
  first_seen: 2025-07-01
  last_seen: 2026-06-09
  confidence: mixed
  brand_self_echo: false
  notes: >
    Kept because it inverts the cluster and shows the screen is wider than pregnancy. She is
    excluded for the opposite reason to everyone else here. My inference: the qualifier is reading
    reproductive status in both directions, so the objection is not really the maternity exclusion,
    it is that an unrelated health fact decides whether she is a mom to this brand.
```

```yaml
- snippet: What happens if you accidentally get pregnant while having this coverage? do you lose this coverage? ￼
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: f7ddf89a-3efb-2a0e-a997-acec679181a0
    date: 2026-04-22
    url: null
  recurrence: 36
  source_diversity: [ad-comment]
  first_seen: 2025-07-01
  last_seen: 2026-06-09
  confidence: mixed
  brand_self_echo: false
  notes: >
    The forward-looking version of the doubt, and the only phrasing in the cluster that is a genuine
    risk question rather than an accusation. Underlying concern, my inference: she is asking whether
    buying this is safe, not whether it covers her today. That is a different objection to answer and
    a friendlier one. No reply from the brand exists on the thread.
```

```yaml
- snippet: Health care for moms but you don’t qualify if your pregnant? Make that make sense.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 1afe1a89-020a-5fba-9d5d-592484d005e1
    date: 2026-05-05
    url: null
  recurrence: 36
  source_diversity: [ad-comment]
  first_seen: 2025-07-01
  last_seen: 2026-06-09
  confidence: thin
  brand_self_echo: true
  notes: >
    Echo flag set and confidence dropped to thin on purpose. The ad MOMS39 - 2 - V2 overlays a tweet
    reading "My deductible is $6000... Make that make sense...." and this commenter turns the brand's
    own sentence pattern back on it. Per the mining method's echo rule this is brand language
    returning, not customer language, and it must not enter the phrase bank as a customer phrase.
    The objection underneath it is real and is already carried by the entries above.
```

### Cluster two — the audience corrects the word the whole hook rests on

**The evidence walk.** I pulled all 74 rows containing "out of pocket" and all 10 containing "OOP," then classified each one myself as a correction of the ad's central claim or as something else. **At least 51 are corrections, across 8 distinct ad names**, running 2026-03-16 to 2026-05-22. That figure is a floor and I want to be blunt about why: 207 rows, 15.7% of the corpus, contain the word "deductible," and I did not classify all 207 one by one. Corrections phrased with only "max," "coinsurance" or "MOOP" fall outside my filter. Upstream's 103 across 13 ads is the superset of my number and the two are consistent. `verified` on my 51, `stated` on the 103.

What makes this different from every other cluster: the objection is not to the offer, it is to the brand's competence. The winning ad opens with a woman saying "My deductible is $6,000. I have to spend $6,000 in medical expenses before everything is taken care of and there's no copays," and the audience says that describes an out-of-pocket maximum, not a deductible. Self-identified licensed brokers, a licensed insurance broker, an insurance agent, a medical biller and a certified application counselor all show up in the corrections. This is the corpus's clearest **messaging opportunity** in the mining method's sense: the customer is handing the brand more precise language than the brand is currently using.

My read, marked `inferred`: the served audience is far more fluent in this category than the creative assumes. The category jargon count is the proof. Deductible in 207 records, out of pocket in 74, premium in 46, plus coinsurance, guaranteed issue, medical underwriting, marketplace, subsidy, HSA and Direct Primary Care all appearing unprompted. A hook built on a term this audience owns is a hook the audience will grade.

```yaml
- snippet: That’s not a deductible that’s a medical maximum out of pocket. You should educate people, not misinform!!
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: c0a3c689-ecb4-a5a8-ae30-3176267bcc34
    date: 2026-03-29
    url: null
  recurrence: 51
  source_diversity: [ad-comment]
  first_seen: 2026-03-16
  last_seen: 2026-05-22
  confidence: mixed
  brand_self_echo: false
  notes: >
    Recurrence is a floor. 51 corrections carrying the exact strings "out of pocket" or "OOP" across
    8 ad names, out of 1,322. The true cluster is larger, since 207 records contain "deductible" and
    were not all classified. Underlying concern, my inference: this is not a coverage doubt at all,
    it is a competence verdict. If the brand is wrong about the first sentence, she has no reason to
    trust the rest of it. Drew 2 likes and 3 replies.
```

```yaml
- snippet: As a licensed insurance broker this is VERY misleading in the beginning. The first half is talking about a medical maximum out of pocket. A deductible is something you pay before your insurance kicks in with co insurance.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: efb760eb-07c9-633d-d536-f92c0ac05bc4
    date: 2026-04-07
    url: null
  recurrence: 51
  source_diversity: [ad-comment]
  first_seen: 2026-03-16
  last_seen: 2026-05-22
  confidence: mixed
  brand_self_echo: false
  notes: >
    Quoted to its first three sentences; the full record continues into a four-paragraph explanation
    of coinsurance. Sits on MOMS38 - 1 - V1, the account's highest-spend creative. The word
    "misleading" from a self-identified broker is the sharpest version of this doubt in the corpus.
    Voice-check: off-voice as written for the brand to adopt, but the observation is exactly right.
```

```yaml
- snippet: Deductible is different than maximum out of pocket 😃 -an insurance agent
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: b41c3c21-4571-2770-b3ae-65e929619418
    date: 2026-05-01
    url: null
  recurrence: 51
  source_diversity: [ad-comment]
  first_seen: 2026-03-16
  last_seen: 2026-05-22
  confidence: mixed
  brand_self_echo: false
  notes: >
    The shortest and most quotable form of the correction, and the one that carries its own
    credential in the sign-off. A golden nugget by the mining method's test, though only as the line
    an ad answers rather than a line the brand can say.
```

```yaml
- snippet: A deductible ≠ out of pocket max. You should consider yourself lucky if your OOP Max is $6,000. A $6,000 deductible would the the amount you pay in full BEFORE copays kick in.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 3486a679-7242-6515-294d-89bbbf4ead71
    date: 2026-03-23
    url: null
  recurrence: 51
  source_diversity: [ad-comment]
  first_seen: 2026-03-16
  last_seen: 2026-05-22
  confidence: mixed
  brand_self_echo: false
  notes: >
    Distinct because it does two jobs at once. It corrects the term and it rejects the premise that
    $6,000 is a shocking number, which undercuts the ad's whole emotional setup. My inference: the
    hook is trying to agitate with a figure that a sophisticated slice of this audience reads as
    lucky, so the agitation lands backward on them.
```

```yaml
- snippet: Bc careful woth that Max Out of Pocket. U can have a $0 Deductible but an $8,000 Max Out of Pocket. Pay attention to the fine lines bc that's how they get u. Working with health insurance. This is kinda a sneak trick that's hidden out in the open. It's why I do not get insurance
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 8694ba97-9d45-43ac-565c-a768450c6c43
    date: 2026-05-05
    url: null
  recurrence: 51
  source_diversity: [ad-comment]
  first_seen: 2026-03-16
  last_seen: 2026-05-22
  confidence: mixed
  brand_self_echo: false
  notes: >
    The most damaging single record in the cluster and the reason it deserves its own entry. It aims
    the correction directly at the brand's own headline offer, the zero-dollar deductible, and calls
    it the trick. This is the objection that turns a terminology fight into a doubt about the product
    being sold.
```

```yaml
- snippet: THANK YOU  I was so annoyed that she was talking about how shit is covered in full once ded is met because unless it’s the same amount as OOPM, that’s incorrect.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: ab8cce20-9d2e-f8e5-f305-b3fe52cd7eb1
    date: 2026-04-03
    url: null
  recurrence: 51
  source_diversity: [ad-comment]
  first_seen: 2026-03-16
  last_seen: 2026-05-22
  confidence: mixed
  brand_self_echo: false
  notes: >
    Kept because it is agreement with an earlier correction rather than a fresh one, which shows the
    correction thread compounding. Voice-check: off-voice as written. The observation survives, the
    wording cannot be lifted.
```

### Cluster three — you cannot have this if you actually need it

**The evidence walk.** I pulled every row containing "existing," which returned 38, then "diabet," which returned 11, then "cancer," which returned 9, then "qualify," which returned 42, and classified each. **42 comments carry the medical underwriting objection, across 17 distinct ad names**, running 2025-07-02 to 2026-09-02. `verified`. The last one landed on 2026-09-02, the day before the pulls ran, which means the objection is live right now and not a historical artifact.

Era tagging matters here and cuts the other way from most clusters. Where the AI backlash is a 2025 objection concentrated on one retired ad, this one is spread evenly across fourteen months and seventeen ads, including the newest creative in the account. It is the widest objection in the corpus by ad spread.

My read, marked `inferred`: this is where the corpus's highest emotional intensity collides with the product's eligibility rules. The persona method says to keep volume and emotional intensity as separate rankings, and this cluster is the proof. By volume it is 3.2% of comments. By intensity it holds the longest, angriest and most specific records in 1,322, from families naming cancer, MS, a NICU stay, type one diabetes and prescriptions in the thousands per fill. The people who need the product most are the people the underwriting screens out, and they say so in public under the brand's paid creative.

```yaml
- snippet: Don’t bother looking into it if you’re diabetic . I’ll be uninsured until I die.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 01b5ff6d-1ea1-b12f-fe1f-136348d8c40b
    date: 2025-08-14
    url: null
  recurrence: 42
  source_diversity: [ad-comment]
  first_seen: 2025-07-02
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  notes: >
    42 of 1,322, 3.2%, across 17 distinct ad names, the widest spread of any objection in the corpus.
    The second sentence is the highest-intensity line in the whole cluster and it is a pain phrase
    riding inside an objection; the pain half belongs to voc-pain-phrase, the first half is the
    objection. Note the shape: she is warning other women off, not asking the brand a question.
```

```yaml
- snippet: It only works if you don’t have any preexisting conditions. You gotta be perfectly healthy to qualify it looks like
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 6537b3b8-785c-62e2-6891-2b1ac3ebd571
    date: 2026-08-13
    url: null
  recurrence: 42
  source_diversity: [ad-comment]
  first_seen: 2025-07-02
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  notes: >
    The plainest statement of the barrier in the corpus and the most lift-ready as the doubt a script
    answers. Drew 2 likes and a reply. Recent, on live creative, which matters because era tagging
    shows this cluster has not faded the way the AI objection did.
```

```yaml
- snippet: Preexisting health condition of cancer disqualified me
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 3bcd0ddf-30f5-1e4c-a318-1868b9e7055f
    date: 2026-09-02
    url: null
  recurrence: 42
  source_diversity: [ad-comment]
  first_seen: 2025-07-02
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  notes: >
    The newest record in this cluster, posted 2026-09-02, the day before the pulls ran. Six flat words, no anger, no
    audience. It is the closest thing in the corpus to a private hesitation written in public, which
    is why it is kept despite carrying no quotable heat.
```

```yaml
- snippet: I like how it's "insurance that has your back" but apparently there's no plans for someone who's pregnant with type one diabetes. Yeah, totally has my back on the condition that I'm healthy before getting the insurance
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: c07a7826-7f12-090e-db52-0b8ff04c4abb
    date: 2026-04-12
    url: null
  recurrence: 42
  source_diversity: [ad-comment]
  first_seen: 2025-07-02
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  notes: >
    Counted once, in the pregnancy cluster, and quoted here because it is the record where both
    screens fire on one person. Drew 4 likes and 3 replies. The quoted phrase "insurance that has
    your back" is the brand's own line coming back sarcastically, so a light echo caution applies to
    that fragment even though the objection itself is the commenter's own.
```

```yaml
- snippet: So u mean to tell me I have to be in good health to qualify? Because they turned me down when I said I have an existing condition.  Please explain
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 3b9c3df6-07eb-c1f4-adc8-c88e974f5563
    date: 2025-07-05
    url: null
  recurrence: 42
  source_diversity: [ad-comment]
  first_seen: 2025-07-02
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  notes: >
    The earliest record in the cluster and the only one framed as a direct request for an answer
    rather than a warning to peers. "Please explain" went unanswered on the thread. My inference:
    the objection hardens into warning language over the following months precisely because nobody
    answers it at this stage.
```

```yaml
- snippet: And they’re holding pre-existing conditions against you, which is illegal. Their system automatically bounced me out. Since I’m a certified application counselor for the healthcare marketplace I know these things I’ve done medical billing for 30 years plus. I wouldn’t waste my time on this page.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 8c7778e3-0f5c-637f-5546-54babff4e694
    date: 2025-07-23
    url: null
  recurrence: 42
  source_diversity: [ad-comment]
  first_seen: 2025-07-02
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  notes: >
    Carried as customer language, not endorsed. The legal claim is the commenter's, marked stated and
    not verified, and it is a question for the brand and its counsel rather than for this doc. Kept
    because it is the version of the objection that carries a credential and tells other readers to
    leave, which makes it the most costly single phrasing in the cluster.
```

### Cluster four — turned away with no reason given

**The evidence walk.** This one is not on the brand's stated list and not on the upstream cluster list. It surfaced when I read all 42 rows containing "qualify" rather than pulling only the clusters I was sent to check. **11 comments across 7 distinct ad names**, running 2025-07-28 to 2026-06-03, describe reaching the end of the qualifier and being told no, several of them explicitly saying they were never told why. `verified` on the count.

11 of 1,322 is 0.8%, which is under the mining method's ten-record threshold for a stable pattern only at the level of a single ad. Across seven different ads over eleven months it clears that bar as a real if small recurring barrier, and I am marking it mixed rather than thin for that reason.

My read, marked `inferred`: this is a different objection from the two screens above, and collapsing them would be a mistake. The pregnancy and pre-existing objections are about the rule. This one is about the silence. She does not know which rule caught her, so she cannot tell whether to try again, try a different product, or conclude the whole thing was a bait. Several of these records read as the moment a warm lead turns into a public detractor.

```yaml
- snippet: Well, this mom did not qualify and it didn’t tell me why.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 74fca251-35b8-f2ea-3eac-104d73d47476
    date: 2025-08-03
    url: null
  recurrence: 11
  source_diversity: [ad-comment]
  first_seen: 2025-07-28
  last_seen: 2026-06-03
  confidence: mixed
  brand_self_echo: false
  notes: >
    11 of 1,322, 0.8%, across 7 distinct ad names over eleven months. Not on the brand's stated
    objection list and not surfaced as its own cluster upstream. Underlying concern, my inference:
    the doubt is not about eligibility, it is about being left without an answer, which is what turns
    a screened-out visitor into someone who posts about it. A resolution exists nowhere on the thread.
```

```yaml
- snippet: So me and my kids still dont qualify thats stupid thought yall were supposed to help moms but I guess not thanks for another time waster
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: be1f0c49-c3f3-65da-6203-60f13c71ef54
    date: 2025-08-03
    url: null
  recurrence: 11
  source_diversity: [ad-comment]
  first_seen: 2025-07-28
  last_seen: 2026-06-03
  confidence: mixed
  brand_self_echo: false
  notes: >
    The phrase "another time waster" is the closest thing in the corpus to the brand's stated "I
    don't have time" objection, and note where it appears: after the form, not before it. My
    inference: the time objection for this brand is not a reason to skip the funnel, it is a verdict
    on the funnel after she has already spent the time.
```

```yaml
- snippet: Who do you actually help because I’m a single mom but every time I try to get a quote it tells me you have no plan for me? So what are the qualifications m? Making over $30,000 or needing to have preexisting things? Not sure while I fall short at.. 🤷🏻‍♀️
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 890aae1e-37cf-d43e-2057-a4730d81221f
    date: 2026-05-10
    url: null
  recurrence: 11
  source_diversity: [ad-comment]
  first_seen: 2025-07-28
  last_seen: 2026-06-03
  confidence: mixed
  brand_self_echo: false
  notes: >
    The fullest statement of the doubt in the corpus, and it names repeat attempts rather than one.
    "Who do you actually help" is the underlying question beneath every entry in this cluster,
    stated outright by the commenter rather than inferred by me. A golden nugget as the objection a
    script answers.
```

```yaml
- snippet: So I don’t qualify with the 4 questions they asked! WTF! This is a joke!
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: e06f2bcc-c1df-fb43-5146-404586cf9bf1
    date: 2025-08-07
    url: null
  recurrence: 11
  source_diversity: [ad-comment]
  first_seen: 2025-07-28
  last_seen: 2026-06-03
  confidence: mixed
  brand_self_echo: false
  notes: >
    Distinct because it counts the questions. Four questions and a rejection is the specific detail
    that makes the record replayable, and specificity of that kind is a qualifying signal under the
    mining method. Voice-check: off-voice as written.
```

### Cluster five — give them your number and you will never stop paying for it

**The evidence walk.** I ran the string "call," which returned 49 rows, then a semantic pass on selling information and spam contact, because four of the strongest records never use the word call at all. Classifying both sets gives **17 customer comments across 10 distinct ad names**, running 2025-08-13 to 2026-05-17, plus one more where a rival agent amplifies the same objection to win the click for himself. `verified`.

This cluster punches far above its 1.3% share for one reason: agreement. The corpus has no rating field, so likes are the only proxy for resonance available, and this objection holds the third-most-liked record in all 1,322 at 33 likes and another at 17. Roughly three quarters of the corpus carries no likes at all. So a cluster this small holding two of the ten most-liked records is meaningful.

Era tagging shows the objection changing shape, which is the single most useful thing in this cluster. In 2025 it is a report from someone who filled the form. By 2026 it is fear from someone who has not. That drift matters because it means the barrier has moved upstream, from a service complaint into a pre-click hesitation, which is exactly the kind of doubt this pass exists to catch.

```yaml
- snippet: Filled it out and have been getting calls everyday from all sorts of companies which are mostly India based.  Also, the harassment from whomever keeps calling me about Medicare (India again).  This is the ONLY form I've filled out since getting my new phone number 3 months ago so it came from this site!
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 3e6adba4-f376-7605-39dc-2dba27b2a2a5
    date: 2026-03-16
    url: null
  recurrence: 17
  source_diversity: [ad-comment]
  first_seen: 2025-08-13
  last_seen: 2026-05-17
  confidence: mixed
  brand_self_echo: false
  notes: >
    33 likes, the third-most-liked record in 1,322, and roughly three quarters of the corpus carries
    no likes at all, so the agreement here is the signal rather than the count. Strictly this is a
    post-form service complaint rather than a pre-purchase doubt, and it is kept in the objection set
    because it is the source the 2026 fear entries are quoting. The new phone number detail is what
    makes it credible to other readers.
```

```yaml
- snippet: How many calls will I get if I try to see how this works?
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 3707bfa1-c0bd-2629-63b4-6987e500f611
    date: 2026-05-17
    url: null
  recurrence: 17
  source_diversity: [ad-comment]
  first_seen: 2025-08-13
  last_seen: 2026-05-17
  confidence: mixed
  brand_self_echo: false
  notes: >
    17 likes and a reply. The purest pre-click form of the objection in the corpus and the single
    best line in this doc for a writer, because it is short, spoken, and asks the exact question a
    script can answer with a number. A golden nugget, clear on the claims-check only if the brand can
    actually state the number.
```

```yaml
- snippet: I filled this out because it literally says we won't be contacted by random agents. That's a lie. I immediately received 5 text messages from 5 different agents claiming to be from 5 different companies.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: bd37a0d3-af13-5151-8a43-90c98a6b4f41
    date: 2025-11-28
    url: null
  recurrence: 17
  source_diversity: [ad-comment]
  first_seen: 2025-08-13
  last_seen: 2026-05-17
  confidence: mixed
  brand_self_echo: false
  notes: >
    Echo flag left false but worth a note: she is quoting the brand's own promise back at it, which
    is the reverse of a brand echo. The brand's reassurance became the evidence against it. My
    inference: promising no contact from random agents is currently generating the objection rather
    than answering it, which is a claims-check problem sitting in the funnel copy, not in the ads.
```

```yaml
- snippet: I don’t wanna put my information and get called by hundreds of people though..
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: a90f4907-4814-82da-e141-d85c223b181f
    date: 2026-03-11
    url: null
  recurrence: 17
  source_diversity: [ad-comment]
  first_seen: 2025-08-13
  last_seen: 2026-05-17
  confidence: mixed
  brand_self_echo: false
  notes: >
    2 likes. The plain-spoken 2026 fear version, from someone who has not filled anything out. This
    is the objection sitting closest to the click and the exact wording a hook can answer. In-voice
    and liftable as written.
```

```yaml
- snippet: Absolutely do not give them your info. You will receive calls and texts nonstop from an insane amount of reps.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 7af3b3e3-998b-1c9f-f978-43bc96334e0a
    date: 2025-09-17
    url: null
  recurrence: 17
  source_diversity: [ad-comment]
  first_seen: 2025-08-13
  last_seen: 2026-05-17
  confidence: mixed
  brand_self_echo: false
  notes: >
    6 likes and a reply. The warning form, aimed at other viewers rather than at the brand, which is
    the most costly shape this objection takes because it does the discouraging work under live paid
    creative. Two more near-identical warnings sit on the same ad within hours.
```

```yaml
- snippet: If only you didnt send out info to 100 companies so moms werent getting bombarded with calls. Just give quotes online
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 8c5ec2e3-3230-ef04-4d1c-60d721726634
    date: 2026-02-08
    url: null
  recurrence: 17
  source_diversity: [ad-comment]
  first_seen: 2025-08-13
  last_seen: 2026-05-17
  confidence: mixed
  brand_self_echo: false
  notes: >
    Kept separate because it carries the objection and the fix in one line. It also bridges into the
    friction cluster below, where the doubt is about the form itself rather than what happens after
    it. The two are related and should not be merged; one fears the calls, the other resents the
    gate.
```

### Cluster six — I am not allowed to see a price without handing over my life

**The evidence walk.** A semantic pass on being asked for personal information before any price returned six records, and I confirmed each in the row data. **6 comments across 6 distinct ad names**, running 2025-07-07 to 2026-03-15. `verified` on the count. Six of 1,322 is 0.5% and sits below the mining method's ten-record threshold, so this is marked **thin** and should be read as a candidate rather than a barrier.

It earns its place for two reasons. It is not on the brand's stated list or the upstream list, and it names a specific step in the flow rather than a feeling, which the mining method treats as a qualifying signal. My read, marked `inferred`: this is a different job from the call fear. She is not afraid of what happens after the form. She objects to the trade itself, giving up contact details to learn a price, and she says the trade tells her the price is bad.

```yaml
- snippet: Just give some pricing without making people sign up 🙄
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 82440b0a-b0d7-5f79-b96d-6202c36cabcd
    date: 2026-03-15
    url: null
  recurrence: 6
  source_diversity: [ad-comment]
  first_seen: 2025-07-07
  last_seen: 2026-03-15
  confidence: thin
  brand_self_echo: false
  notes: >
    3 likes. 6 of 1,322, 0.5%, across 6 distinct ad names, which is below the ten-record threshold
    for a stable pattern, so thin by rule. Not on the brand's stated objection list. Short, spoken
    and liftable, which is why it is captured despite the thinness.
```

```yaml
- snippet: Why can't you give a quote without my email!
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 3936813d-9ec5-58cb-b814-a02a2299424f
    date: 2025-08-12
    url: null
  recurrence: 6
  source_diversity: [ad-comment]
  first_seen: 2025-07-07
  last_seen: 2026-03-15
  confidence: thin
  brand_self_echo: false
  notes: >
    The earliest form of the same doubt, ten months before the entry above, which is what makes the
    pair worth carrying despite the low count. Persistent rather than recent.
```

```yaml
- snippet: Id be way more interested if I didn't have to talk on the phone immediately tbh. It's super difficult for me to process information without reading and I get so flustered on the phone
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 26f24c05-00d0-6bda-e4e7-10ae9ddd0617
    date: 2025-02-15
    url: null
  recurrence: 3
  source_diversity: [ad-comment]
  first_seen: 2025-02-15
  last_seen: 2026-03-10
  confidence: thin
  brand_self_echo: false
  notes: >
    A related but genuinely separate doubt, so it carries its own recurrence count of 3 rather than
    the cluster's 6. Three records across three ads name the phone call itself as the barrier, not
    the number of calls. This is the closest match in the corpus to the brand's stated "I don't want
    to get on a call and be sold to," and it is the only one of the three that explains why, which
    makes it the most useful. Opens with what would fix it, which is rare in this corpus.
```

### Cluster seven — my state is not on the list, so why am I seeing this

**The evidence walk.** There is no reliable string for this objection, so it was derived semantically at two thresholds and every returned row was read. **At least 15 comments across 5 distinct ad names**, running 2026-03-13 to 2026-09-02. This is a floor, not a total, because semantic recall is not an exact count, and I am saying so rather than presenting it as complete. `verified` that the 15 exist, `data-limited` on the true size.

This is the one objection on the brand's stated list that also shows clearly in the record, and the brand treats the state list as a deliberate open loop meant to compel the click. The comments show it firing backward part of the time. My read, marked `inferred`: the doubt is not really about geography. It is a targeting complaint dressed as an eligibility question, and the sting is that she was invited by an ad she was never eligible for.

```yaml
- snippet: I didn't see my state... So why am I getting this ad?
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 5c403d2c-f9c9-5054-ad96-6b0baba50ff0
    date: 2026-04-07
    url: null
  recurrence: 15
  source_diversity: [ad-comment]
  first_seen: 2026-03-13
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  notes: >
    Recurrence is a floor derived semantically across two thresholds, not an exact string count, and
    the true number is higher. 15 of 1,322 is 1.1% across 5 distinct ad names. The clearest form of
    the doubt: the objection is to being served the ad, not to the state list itself.
```

```yaml
- snippet: Why is this being shown in IL if it’s not on the list???😭🤦🏼‍♀️
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 713721dc-21b1-d455-1fdd-ca76dc7ed44e
    date: 2026-09-02
    url: null
  recurrence: 15
  source_diversity: [ad-comment]
  first_seen: 2026-03-13
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  notes: >
    Posted 2026-09-02, the day before the pulls ran, on the newest creative in the corpus, which is
    what makes it worth its own entry. The objection is current, not historical. Era tag: live.
```

```yaml
- snippet: Ha… “in these states” proceeds to list all 50 states… scam
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 5826f609-559c-5978-9b92-6fb1de0b16e4
    date: 2026-03-26
    url: null
  recurrence: 15
  source_diversity: [ad-comment]
  first_seen: 2026-03-13
  last_seen: 2026-09-02
  confidence: mixed
  brand_self_echo: false
  notes: >
    Distinct because it converts the state device into a legitimacy objection rather than an
    eligibility one. My inference: the creative device meant to compel a click reads to part of the
    audience as a tell that the exclusivity is fake, which is a straight line from this cluster into
    the legitimacy cluster below.
```

### Cluster eight — is this even real

**The evidence walk.** 45 of 1,322 records, 3.4%, contain the word "scam," verified by string count. Most aim at the insurance category rather than at Health For Moms, and the mining method's exclusion list is right that a complaint about the category is not a doubt about the product, so the brand-directed subset is what I captured. A semantic pass returned six direct legitimacy questions on top of that.

The most-liked record in all 1,322, at 47 likes, opens with "This sounds too good to be true," which makes disbelief the single most agreed-with reaction in the corpus. `verified` on the like count and the string counts.

My read, marked `inferred`: the underlying concern is not fraud in the criminal sense. It is that the offer is not what it appears to be, and the audience's evidence for that is the gap between what the ad claims and what the qualifier does. Every other cluster in this document feeds this one.

```yaml
- snippet: This sounds too good to be true. I pay over $1,000 a month for a premium. We have to pay an $8000 deductible per family member or up to $17,000 for the entire family. It’s insane. I have 2 members of the family with chronic diseases. This absolutely insane. I want the 1990’s back.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: b7aa4d37-2243-d0fe-03e6-50c8b7d495ca
    date: 2026-03-22
    url: null
  recurrence: 45
  source_diversity: [ad-comment]
  first_seen: 2025-01-13
  last_seen: 2026-09-01
  confidence: mixed
  brand_self_echo: false
  notes: >
    47 likes and 9 replies, the most-liked record in the entire corpus. Recurrence 45 is the string
    count for "scam" across 1,322, 3.4%, and most of those aim at the insurance category rather than
    at this brand, so the brand-directed share is smaller. Only the first sentence is the objection;
    the rest is a pain phrase and belongs to voc-pain-phrase. "I want the 1990's back" is a headline
    candidate and routes there too.
```

```yaml
- snippet: Anyone actually have this and have insight?
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: a08ebb3f-7ebf-5b83-95fa-5d36f553dd8c
    date: 2026-03-20
    url: null
  recurrence: 6
  source_diversity: [ad-comment]
  first_seen: 2025-07-24
  last_seen: 2026-05-15
  confidence: mixed
  brand_self_echo: false
  notes: >
    15 likes and 6 replies, and its own recurrence count of 6 for the direct legitimacy question,
    separate from the 45 scam records. This is the politest and highest-agreement form of the doubt:
    she is not accusing, she is asking the crowd for proof. My inference: with zero reviews, zero
    surveys and only two positive service reports in 1,322 comments, there is nothing anywhere for
    her to find, which is a supply problem rather than a copy problem.
```

```yaml
- snippet: A Google search doesn't pull anything about this. Is it legit?
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 9e6fca11-0848-5d26-aecb-e6324ff55c6c
    date: 2025-07-24
    url: null
  recurrence: 6
  source_diversity: [ad-comment]
  first_seen: 2025-07-24
  last_seen: 2026-05-15
  confidence: mixed
  brand_self_echo: false
  notes: >
    1 like and a reply. The most actionable legitimacy record in the corpus because it names the
    exact check she ran and the exact result. This is the brand's own stated "is this legit"
    objection, confirmed in the record and given a specific cause.
```

```yaml
- snippet: Ok. What if you or your children have a preexisting condition? Is it guaranteed renewable? Whats the catch, because I guarantee there is one.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 5db97499-85e1-b2d1-619f-8e89522382d5
    date: 2026-05-26
    url: null
  recurrence: 6
  source_diversity: [ad-comment]
  first_seen: 2025-07-24
  last_seen: 2026-05-15
  confidence: mixed
  brand_self_echo: false
  notes: >
    3 likes and 3 replies. Quoted to its first four sentences; the full record continues into her own
    cost history and a preference for the marketplace. She stacks three objections into one comment,
    which is why she is kept here rather than only in the pre-existing cluster. "Whats the catch,
    because I guarantee there is one" uses the category term "guaranteed renewable" correctly, which
    is more evidence of how fluent this audience is.
```

```yaml
- snippet: click bait sends you to the same sales team for private quotes 🙄
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 3fef2c67-4e70-5841-b003-edc64640f6ba
    date: 2025-07-07
    url: null
  recurrence: 6
  source_diversity: [ad-comment]
  first_seen: 2025-07-24
  last_seen: 2026-05-15
  confidence: thin
  brand_self_echo: false
  notes: >
    A single record and therefore a candidate rather than a pattern, per the mining method's
    single-instance rule. Kept because it names the specific mechanism the doubt rests on, that the
    ad and the funnel lead to the same generic sales team, which no other record states this plainly.
```

### Cluster nine — is "mom" who I am or a rule I have to pass

**The evidence walk.** Reading the full "qualify" pull surfaced a set of sincere eligibility questions about the word the brand is named after. Combined with the records already known upstream, this runs to roughly **7 comments across 5 distinct ad names**, from 2025-01-08, the oldest comment in the entire corpus, through 2026-07-22. `verified` on the individual records, `data-limited` on the exact total, since there is no clean string for it.

My read, marked `inferred`, and it is the sharpest thing in this doc for the persona work downstream: the word "mom" is doing two jobs and the audience cannot tell which one is live. It is meant as an identity and it is being heard as an eligibility rule. That is why these come as questions rather than complaints. They are polite, which is rare here, and none of them is answered on the thread.

```yaml
- snippet: What if your kids are over 18, do I still qualify as a Mom?
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 0bf2b362-2726-f4a9-ebc0-3b5017d1037c
    date: 2026-04-29
    url: null
  recurrence: 7
  source_diversity: [ad-comment]
  first_seen: 2025-01-08
  last_seen: 2026-07-22
  confidence: mixed
  brand_self_echo: false
  notes: >
    Roughly 7 of 1,322 across 5 distinct ad names, count marked data-limited because no reliable
    string isolates this objection. Underlying concern, my inference: this is not a coverage doubt at
    all, it is a permission question. She is asking whether she is allowed to want this, which is a
    completely different thing for copy to answer than a price or a trust objection.
```

```yaml
- snippet: Why do you have to be a mother to qualify?
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 893d8ee3-88a0-3fc6-45f4-381245a04be9
    date: 2026-03-26
    url: null
  recurrence: 7
  source_diversity: [ad-comment]
  first_seen: 2025-01-08
  last_seen: 2026-07-22
  confidence: mixed
  brand_self_echo: false
  notes: >
    The version that questions the rule itself rather than her fit inside it. Worth carrying into
    persona work: 284 of 1,322 records, 21.5%, contain "insurance" while at most 73, 5.5%, contain
    "mom," and that 5.5% is inflated because the string also matches "moment." The audience is
    talking about the category far more than about the identity the brand named itself after.
```

```yaml
- snippet: Do you have to be a SHM or do working moms qualify also?
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: efbfc74f-dde7-9346-8830-e6840c5ff3a1
    date: 2026-07-22
    url: null
  recurrence: 7
  source_diversity: [ad-comment]
  first_seen: 2025-01-08
  last_seen: 2026-07-22
  confidence: mixed
  brand_self_echo: false
  notes: >
    Uses the insider shorthand SHM for stay-at-home mom without expanding it, which is category
    jargon and routes to voc-category-jargon as well. The most recent record in this cluster, so the
    confusion is current rather than solved.
```

```yaml
- snippet: Only for moms? Lol
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 81b9eb5f-aa87-be8c-8e56-a941e5be5f71
    date: 2025-01-08
    url: null
  recurrence: 7
  source_diversity: [ad-comment]
  first_seen: 2025-01-08
  last_seen: 2026-07-22
  confidence: thin
  brand_self_echo: false
  notes: >
    The single oldest record in the entire 1,322-comment corpus, and it is this objection. Thin on
    its own as four words with no reasoning attached. Kept for the era point: the very first thing
    anyone said under this brand's advertising was a question about who the word "mom" lets in.
```

### Cluster ten — I make too little to qualify for the plan for people who cannot afford insurance

**The evidence walk.** Four records say the product has an income floor, running 2025-08-03 to 2026-09-01, on four different ads. `verified` on the records, and 4 of 1,322 is 0.3%, well under the ten-record threshold, so this is **thin** and is a candidate, not a barrier. I am capturing it because it appears on neither the brand's stated objection list nor the upstream cluster list, and because the newest instance landed two days before this doc.

My read, marked `inferred`: if this is real it is the sharpest contradiction in the whole account. The creative recruits women who cannot afford what they have, and a qualifier apparently turns some of them away for not earning enough. The brand can settle this in a minute and nobody else can.

```yaml
- snippet: But if you make under 30k a year you don’t qualify smh
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 45b22fb4-ca7c-f1bb-b935-21e946bcae2c
    date: 2026-09-01
    url: null
  recurrence: 4
  source_diversity: [ad-comment]
  first_seen: 2025-08-03
  last_seen: 2026-09-01
  confidence: thin
  brand_self_echo: false
  notes: >
    4 of 1,322, 0.3%, across 4 distinct ad names. Thin by the ten-record rule and flagged as a
    candidate. On no stated objection list anywhere. Posted 2026-09-01, two days before the pulls ran, so it is live.
    Claims-check: the income floor itself is unverified by Parker and only the brand can confirm it.
```

```yaml
- snippet: I make less than 30,000 bc I'm a student in school and don't qualify for this.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: b9341ab7-c197-b4d6-b7da-4cbf57a08d81
    date: 2026-05-28
    url: null
  recurrence: 4
  source_diversity: [ad-comment]
  first_seen: 2025-08-03
  last_seen: 2026-09-01
  confidence: thin
  brand_self_echo: false
  notes: >
    Independent corroboration of the same floor at the same number, three months earlier and on a
    different ad. Two records naming the identical threshold is what lifts this from noise to a
    candidate worth the brand's answer.
```

```yaml
- snippet: I don't have any pre-existing conditions, so I don't think that was it. Probably more likely that they don't cover in my area. Or my income doesn't fall into the sweet spot. I don't make very much, just more than medicaid allows (which is far below poverty level).
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 057b1714-d666-2d73-a6c5-3a480d672d3f
    date: 2025-08-03
    url: null
  recurrence: 4
  source_diversity: [ad-comment]
  first_seen: 2025-08-03
  last_seen: 2026-09-01
  confidence: thin
  brand_self_echo: false
  notes: >
    The earliest record and the one that shows the doubt and the silent rejection working together:
    she is guessing at why she was turned down because nothing told her. "Sweet spot" is her own
    phrase for the income band and is a candidate for voc-category-jargon.
```

### Cluster eleven — I cannot switch even if I want to

**The evidence walk.** Five records across three ads say the employer picks the plan and she has no choice. `verified`. 5 of 1,322 is 0.4%, so **thin** by count. It is captured because it is not a doubt about the product at all, it is a doubt about whether the offer can apply to her, and the whole creative premise assumes she can switch.

My read, marked `inferred`, and it is a persona finding as much as an objection: she is reachable by the ad and unreachable by the offer. One commenter had to explain in the replies that declining employer coverage is allowed, which the brand never says anywhere. The persona method calls this an identity overlay rather than a persona, since being on an employer plan is a state that cuts across every buyer here, and it should be treated that way downstream rather than promoted into a persona of its own.

```yaml
- snippet: Tamara Paige nope.  My job picks the plan that they offer.
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 0f3700de-8f66-22bf-5b20-88e3477ab128
    date: 2026-03-30
    url: null
  recurrence: 5
  source_diversity: [ad-comment]
  first_seen: 2026-03-17
  last_seen: 2026-08-09
  confidence: thin
  brand_self_echo: false
  notes: >
    1 like. 5 of 1,322, 0.4%, across 3 distinct ad names, so thin. Underlying concern, my inference:
    this is not a doubt about the plan, it is a belief that she has no standing to shop at all. A
    resolution exists in the corpus but not from the brand: another commenter explains on 2026-05-05
    that employer coverage can be declined. That makes this an objection with a known answer nobody
    is giving.
```

```yaml
- snippet: Mine is $6k per person too but since it’s thru my job I don’t really have a choice
  category: objection
  identity_tag: null
  behavioral_signal_tag: null
  source:
    type: ad-comment
    platform: Facebook and Instagram, Meta ad account HealthForMoms act 484897827497337
    review_id: 33936dcd-893a-25ec-3240-bd21906f0e5a
    date: 2026-03-17
    url: null
  recurrence: 5
  source_diversity: [ad-comment]
  first_seen: 2026-03-17
  last_seen: 2026-08-09
  confidence: thin
  brand_self_echo: false
  notes: >
    The phrase "I don't really have a choice" is the clean statement of the barrier and is in-voice
    and liftable. She is agreeing with the ad's pain and declining its premise in the same sentence,
    which is the shape of this whole objection.
```

### What was found and deliberately routed elsewhere

Four things in this corpus look like objections and are not, and the mining method's exclusion list is why. Naming them here keeps the next pass from double-counting.

**The self-insurers.** 33 comments across 10 ads argue you should drop insurance and pay cash. That is a counter-offer to the whole category, not a doubt about buying this product, and the brand's own "insurance is a scam" hook is what recruits it. Routes to voc-anti-language and to the persona work.

**The political blame.** 54 comments across 14 ads route the cost to a political cause in both directions, and they carry some of the highest like counts in the corpus. That is reaction to American health policy, not a pre-purchase doubt. Routed out entirely.

**The AI backlash.** 32 comments call the creative fake, but 25 of them sit on one ad, `B1 samar- Copy`, between 2025-07-20 and 2026-04-05. Era tagging is decisive: this is a 2025 objection tied to one retired creative, with only a handful of 2026 sightings such as "Creepy AI blonde lady ruins the ad tbh" on 2026-04-05. Most of it is a rejection of how the ad is made, which is anti-language. One strand of it is a genuine trust doubt, best shown by the 2025-07-25 record arguing that a fake testimonial "unintentionally sends a message to people that no real actual person would say this about your service." That strand belongs in the legitimacy cluster and is noted rather than double-counted here.

**The deductible disclosures.** 160 comments across 17 ads disclose the commenter's own deductible or premium. That is the largest single theme in the corpus and it is a pain phrase, not an objection. The test the mining method sets is whether she is hesitating about the product or describing the problem the product addresses, and these describe the problem. They belong to voc-pain-phrase.

## Data limitations

**One source type sets a hard ceiling.** Reviews and surveys are both empty, verified live on 2026-09-03. The persona method ranks post-purchase survey data at the top of the evidence stack and public comments near the bottom, and this brand holds only the bottom. Under this prompt's own rule, nothing here can be marked strong.

**Public performance is not private hesitation.** Argued at the top of this doc and repeated here because it governs how every count should be read. Each number is a floor on the doubt, never its size. The woman who scrolled past in silence left nothing.

**Counts are comments, not people.** `author_name` and `author_id` are null on all 1,322 rows. At least nine near-identical rival-agent posts sit under one ad on one day, and they are separate records but not separate people. Any inflation from that kind of repetition is invisible.

**No links.** `permalink_url` is null on every row, so no snippet can be opened in its original thread. Verification runs through the row id in the source block and the Parker tool.

**Two counts are floors and say so.** The deductible correction at 51 and the state exclusion at 15 are both floors. The first is limited by an exact-string filter against a 207-record "deductible" pool I did not fully classify. The second is limited by semantic recall.

**Heavy skew, twice over.** 846 of 1,322 comments, 64.0%, sit in March and April 2026. 795 of 1,322, 60.1%, sit on the `MOMS38 - 1` creative family. Ad spread is carried on every cluster because it survives both skews and a raw count does not.

**No persona slugs exist.** `personas-profile.md` has not been written, so `identity_tag` and `behavioral_signal_tag` are null on all 34 blocks by rule. This pass never invents a slug. When the persona doc lands, this doc should be re-tagged rather than regenerated, because the recurrence history is the value.

**No competitor or category baseline.** No rival brands are tracked in the Parker app, so no objection rate here can be called high or low for health insurance lead generation.

**No lead join.** Nothing here can be tied to the 4,336 leads the account produced in the last 90 days, so no objection in this doc can be said to cost anything. Combined with the brand's own two-gate definition of a winner in `running-notes/success-definition.md`, where gate two is lead quality that Parker cannot see, that means no snippet here can be graded on business impact at all.

**First run, no history.** There is no prior objection set to carry forward, so every `first_seen` date is the earliest instance in the current corpus rather than a genuine first sighting, and nothing can yet be marked as fading. The next run should take this file as context and update rather than rebuild, since first-seen dates and recurrence counts are exactly what give each snippet its weight.

## Open loops

**1. The objections cluster on one creative family and almost skip another.**

Reading the ad names attached to every cluster, the `MOMS38 - 1` family absorbs the bulk of the correction, call-fear, state and legitimacy objections. The `MOMS38 - 2` skit family, where one woman plays both the frustrated mom and the rep denying a claim, appears once in the pregnancy cluster and essentially nowhere else, while holding nearly all of the corpus's few moments of recognition.

Pull: **Gap.** I went looking for objections on every ad and found a creative family that generates almost none, and nothing appears to have been done with that.

Question: What is different about the ads in this account that draw no objection at all?

Why it matters: right now the brand knows which ads spend and which ads get leads, but not which ads pick a fight. If the objection-free creative can be described, that description is a production brief, and it is cheaper to learn than any test.

Territory: **Messaging.**

**2. Two of the five objections the brand says it handles barely exist in its own comment sections.**

"Open enrollment" appears in 1 of 1,322 records and "enrollment" in any form in 2. I pulled and read both, and neither is a customer saying she will wait. The time objection is similarly thin. Meanwhile the two widest objections in the record, the pregnancy exclusion at 36 across 15 ads and the pre-existing screen at 42 across 17, appear on no stated list.

Pull: **Tension.** The brand's account of what stops its buyer and the record of what its audience actually types cannot both be right as stated.

Question: Where did the brand's stated objection list come from?

Why it matters: the stated list is what the creative is built to answer. If it came from a sales team, a landing-page test, or an assumption, that provenance decides whether the comment record should override it or sit beside it as a different slice of the same buyer.

Territory: **Messaging.** Only the brand can answer this one, so it routes to the brand.

**3. Some women are told no and never told why.**

11 comments across 7 ads describe reaching the end of the qualifier and being rejected, several saying outright they were given no reason. One woman guesses at three possible causes in a single comment. Another counts the four questions she was asked before the door closed.

Pull: **Curiosity.** A rejection screen that says nothing is an odd thing to build, and I cannot explain from here what it is for.

Question: What does the qualifier actually say to a woman it turns down?

Why it matters: that screen is the last thing a paid visitor sees, and right now some share of them leave it and post about the brand under live creative. What it says is fully within the brand's control and costs nothing to change.

Territory: **Product.** Only the brand can answer this, since it needs the funnel's own screens.

**4. A handful of women say they earn too little to qualify.**

Four records across four ads, from 2025-08-03 to 2026-09-01, say there is an income floor, two of them naming the same $30,000 threshold independently. The creative recruits women who cannot afford the plan they already have.

Pull: **Surprise.** For a product advertised to women drowning in medical costs, an income floor is not what the setup would predict, and the size of that gap is the signal.

Question: Who is the income floor turning away, and how many of them are there?

Why it matters: if it is real and sizeable, the ads are paying to reach a group the product cannot serve, which is a targeting fix rather than a copy fix. If it is a misunderstanding of a subsidy rule, it is one line of creative.

Territory: **Personas.** Only the brand can answer the first half, since it needs the qualifier's own rules.

**5. Nobody objects to this brand's price, because this brand never names one.**

202 of 1,322 records, 15.3%, contain a dollar figure, and in the ones I read the money is always the plan she already has. Across every cluster above I found no record objecting to what Health For Moms costs. Instead I found six records objecting to being unable to see a price at all without handing over contact details.

Pull: **Gap.** The most common objection in almost every category is missing here entirely, and something has taken its place.

Question: What does this audience expect this to cost before she gives up her phone number?

Why it matters: the funnel currently trades her contact details for a number she has no way to guess at. If her expectation is far from reality in either direction, that gap is either the reason she does not click or the reason the lead goes cold on the call.

Territory: **Product.**

**6. The audience teaches itself the category in the brand's own comment threads.**

Many of the deductible corrections are not aimed at the brand at all. They are commenters explaining coinsurance, out-of-pocket maximums and guaranteed issue to each other, at length. One woman had to be told by a stranger that she is allowed to decline her employer's plan. The brand does not appear in any of these threads.

Pull: **Resonance.** The most generous, detailed and useful writing anywhere in 1,322 comments is being done for free by the audience, and I want to know why it works when the ad's own explanation does not.

Question: What does this audience want explained that nobody is explaining to her?

Why it matters: 166 of 1,322 records, 12.6%, contain a question mark. If the thing she actually wants is an explanation rather than an offer, that reshapes the creative from a pitch into a teaching format, and the corpus already contains the syllabus.

Territory: **Messaging.**
