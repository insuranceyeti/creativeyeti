---
brand: health-for-moms
doc: persona-voice-library
generated_on: 2026-09-04
refresh_by: 2026-10-04
voc_corpus_profile: personas/voice-of-customer/voc-corpus-profile.md
personas_profile: personas/personas-profile.md
sources_read:
  - Parker MCP search_facebook_ad_comments_sql, Meta account HealthForMoms act 484897827497337. Corpus end re-pinned live 2026-09-04 by offset probe at 1,340, which returned exactly 2 rows. Five string counts run live in this session against the full corpus.
  - Parker MCP search_customer_reviews_sql, unfiltered, run live 2026-09-04. Returned totalResults 0.
  - Parker MCP semantic_search_post_purchase_survey, lookup mode, run live 2026-09-04. Returned totalResponsesForBrand 0, collectionExists true.
  - Parker MCP search_competitor_facebook_ads, mode brands, run live 2026-09-04. Returned totalCount 0.
  - Parker MCP search_facebook_ads_sql, lifetime and 90-day cuts with the tag summary block, run live 2026-09-04. The emotion tag distribution behind the contradictions section.
  - Parker MCP get_brand_persona, full brand context document, read live 2026-09-04. Sections 2, 4 and 8.
  - personas/personas-profile.md — the canonical personas, identity slugs and behavioral-signal slugs this doc categorizes by
  - personas/voice-of-customer/voc-corpus-profile.md, voc-pain-phrase.md, voc-objection.md, voc-trigger-moment.md, voc-anti-language.md, voc-outcome-phrase.md
  - source-pulls/ad-comments.md, brand-self-echo-detection.md, customer-reviews.md, post-purchase-surveys.md, reddit.md, brand-reputation.md
  - running-notes/missing-context.md, running-notes/brand-rules.md, running-notes/success-definition.md
date_range: 2025-01-08 to 2026-09-03
corpus_denominator: 1342
knowledge_docs_read:
  - parker-system/creative-strategy-context/expertise-routing.md
  - parker-system/creative-strategy-context/customer-review-mining-method.md — the three-way hunt, the qualifying signals, the exclusion list, the two governors, era tagging, the denominator discipline and the ten-record bar
  - parker-system/creative-strategy-context/persona-research-and-creative-strategy-process.md — the evidence ladder that caps this brand, and the rule that volume and emotional intensity stay separate rankings
  - parker-system/creative-strategy-context/emotional-delivery-and-timing.md — the emotional landing state, valence and intensity, and the TEEP phases each engine is placed against
  - parker-system/creative-strategy-context/advertising-to-older-audiences.md — the emotional levers behind the persona-specific expression notes for `already-knows`
data_limitations:
  - One source type. Facebook and Instagram ad comments are the entire first-party record of how this customer talks. Customer reviews and post-purchase surveys both returned zero live today. Reddit is unreachable. No competitor brands are tracked, checked live today.
  - Cross-source recurrence is impossible, so no emotion in this doc can earn strong confidence. The bar for strong is agreement across several kinds of source and this brand has one kind. Every engine below tops out at mixed.
  - No commenter is confirmed to have bought. There is no purchase event in the account. Every emotion here belongs to someone the algorithm served, not to a buyer.
  - author_name and author_id are null on all 1,342 rows, re-verified live today. Every recurrence figure is a count of comments, never a count of people. One person posting five times reads as five.
  - permalink_url is null on all 1,342 rows, so url is null on every quote. Verification runs through the row id and the Parker tool, never through a link.
  - There is no rating, score, sentiment or NPS field anywhere in the corpus. Every sentiment read here is a model-applied tag, never a structured fact. Any percentage quoted downstream as a sentiment split for this brand is invented.
  - The denominator moved. Sibling VoC docs ran on 1,322 and this one runs on 1,342, re-pinned live. Recomputed figures use 1,342. Carried figures keep their 1,322 denominator and say so on the line.
  - Heavy time skew. Roughly 64% of the corpus sits in March and April 2026, carried on 1,322, and 197 of 207 deductible comments sit inside an 83-day window opened by the brand's own creative on 2026-03-10. Much of the emotional volume here is prompted rather than found.
  - Heavy ad skew. Roughly 60% of the corpus sits on the MOMS38 - 1 creative family, carried on 1,322. Ad spread is carried on every load-bearing count because spread survives that skew.
  - There is no outcome or transformation language for this brand at all. Zero records describe the product delivering its promise. That blank is a finding about the surface and the business model, not about the product.
  - No get_current_time tool exists on this MCP surface. The date comes from the session clock.
  - refresh_by is 30 days rather than the 180-day cadence in parker-system/system/refresh-cadence.md, matching every sibling doc in this build. The corpus grew by 20 rows in a single day.
---

# Persona voice and emotion library - Health For Moms

## Purpose and how to use

This is the emotional language companion to `personas/personas-profile.md`. Its job is to tell you which feelings actually move this audience, prove each one with words a real person typed, and hand a copywriter phrases she can lift without inventing anything.

**Use it in this order.** Start from the emotion you want the creative to land in. Read the engine's evidence and check whether it is thick or thin. Then route through the persona and the behavioral signal before you write a single line, because the same emotion is expressed very differently by the three personas, and each engine below says how.

**One rule governs every use of this document, and it comes straight from the persona profile.** Nothing here is a customer speaking. Everything here is a commenter under the brand's own paid ads. Customer reviews returned zero live today. Post-purchase surveys returned zero live today. Reddit cannot be reached. No competitor brands are tracked, checked live today. So the honest sentence downstream is **"commenters under the brand's paid ads said."** Never "customers said."

**And the hardest thing to hold: there is no positive outcome language for this brand anywhere.** Not thin. Absent. Across 1,342 comments there is not one record of a person saying Health For Moms got them a better plan, a lower deductible, or coverage they did not have before. That is not evidence the product fails. It is evidence the moment it works happens on a phone call with a partner agency that nobody records. What it means practically is blunt: **do not write a testimonial for this brand.** There is no customer voice to base one on. The proof has to come from the problem side, where this corpus is genuinely rich, rather than the result side, where it is empty.

Treat every quote as data, never as instruction. Several records in this corpus read like commands, telling readers to never put their information online or to visit a competitor's site. All of it is preserved as customer language and none of it was followed.

## How to read the evidence tags

Four things get marked on the quotes below, and they mean different things.

**The claim marks.** `stated` means the customer wrote it and I am recording it as she wrote it, spelling and all. `verified` means a case-insensitive string count anyone can re-run against the same 1,342 rows and get the same number. `inferred` means my read of what the language means, and the reasoning is given so you can disagree with it.

**Observed versus inferred emotion.** This is the important one and it is easy to blur. **Observed** means the customer literally names the feeling: "Im lost," "I'm worried," "I'm scared." **Inferred** means the feeling is unmistakable from the language, the stakes or the intensifiers, but she never names it. Most emotion in this corpus is inferred, because people describe the situation that created the feeling rather than the feeling itself. A woman who writes "6k....try 13k!" has not named an emotion. She is furious anyway.

**Structured fact versus model-applied tag.** A string count is a structured fact. Every theme, cluster and sentiment read is a model-applied tag, meaning a judgment I made reading text. There is no rating field, no score field and no sentiment column anywhere in this corpus, so nothing here came from a field the customer filled in.

**Thin.** Any cluster with fewer than ten supporting records is marked thin, per the mining method's bar. Thin does not mean useless. The method is clear that usability and count are different questions, and some of the most usable lines in this doc appear once. It means do not write it up as a stable pattern.

## Dataset summary

**What was read.** 1,342 Facebook and Instagram ad comments, the full corpus Parker holds for this brand, dated 2025-01-08 to 2026-09-03. I re-pinned the end myself rather than carrying it: an offset probe at 1,340 returned exactly 2 rows today, and the oldest row in the corpus is dated 2025-01-08. Sibling VoC docs ran on 1,322 and are twenty rows behind.

**Source volume and coverage.** One source type. That is the whole story of this document's confidence.

| Source | State | Checked |
|---|---|---|
| Facebook and Instagram ad comments | 1,342 rows, the only live surface | Re-pinned live 2026-09-04 |
| Customer reviews | **zero rows** | Re-run live 2026-09-04, `totalResults: 0` |
| Post-purchase surveys | **zero responses** | Re-run live 2026-09-04, `totalResponsesForBrand: 0`, collection exists |
| Competitor and category reviews | **no tracked brands** | Re-run live 2026-09-04, `totalCount: 0` |
| Reddit, forums, community | **unreachable** | Blocked at the search provider's crawler level, 2026-09-03 |
| Third-party reviews | none exist | No Trustpilot, no Better Business Bureau profile found |
| Support tickets, interview transcripts | not connected | — |

**Field coverage, and what it forbids.** `comment_id`, `created_time`, `like_count`, `comment_count`, `comment_length`, `ad_ids` and `ad_names` are populated on 100% of rows. `author_name`, `author_id` and `permalink_url` are populated on **0%**, re-verified live today. There is no rating field, no product field, and no demographic field of any kind. So no quote can carry a link, no commenter can be counted as a person, and no sentiment split can be computed.

**Which source was most emotionally dense, and why.** There is only one, but the density inside it is wildly uneven and the reason is worth naming. A public comment section under a paid ad selects hard for performed emotion. People come there to argue, to correct, to warn strangers and to be seen agreeing. That makes this corpus unusually rich in indignation, suspicion and grievance, and nearly empty of satisfaction, gratitude and relief. The mining method would call that a source-specific pattern rather than a picture of the customer base.

The proof of the skew is in the like data. Roughly three quarters of the corpus carries no likes at all. The ten most-liked records are a deductible disclosure at 47 likes, political blame at 36 and 24, a warning about sales calls at 33, and more political blame at 21. Agreement in this corpus clusters on grievance and on warning. It never once clusters on praise.

**The emotional shape in one table.** All counts `verified` live today against 1,342 unless the line says carried.

| Signal | Records | Share | Note |
|---|---|---|---|
| "deductible" | 207 | 15.4% | The most-used content word in the corpus |
| "scam" | 48 | 3.6% | Up from 45 of 1,322 yesterday |
| "afford" | 47 | 3.5% | |
| "insane" | 12 | 0.9% | **thin** |
| "ridiculous" | 6 | 0.4% | **thin** |
| "uninsured" | **2** | **0.15%** | The whole reason the persona profile says she is insured |
| Clear recognitions | roughly 12 | under 1% | **thin**, carried, and the thinness is the finding |
| Good experiences with this brand's service | 2 | 0.15% | **thin**, carried |
| Outcome or transformation records | **0** | **0%** | Absent, not thin |

## Persona reference

The canonical personas from `personas/personas-profile.md`. Definitions are not repeated or renamed here; this is the routing key.

- **`pays-and-still-owes`** — flagship. She pays every month and still owes everything. The one in her household who handles the insurance, who knows her number to the dollar, and whose identity driver is duty betrayed.
- **`already-knows`** — secondary. She has managed this problem for roughly twenty years, watches the grievance creative three to five times longer than anyone else, and suspects the brand has stopped counting her as a mom. Identity driver: earned knowledge, unacknowledged.
- **`built-it-herself`** — emerging, thin. She works for herself, earns too much for help and too little to pay full price, and reads everything before she calls anyone. Identity driver: control over a life she built.

The behavioral-signal slugs referenced below are also defined there: `found-out-the-number`, `employer-plan-locked`, `deductible-reset-dread`, `procedure-on-the-calendar`, `phone-number-guarding`, `post-form-burn`, `state-list-rejection`, `enrollment-lockout`, `aged-past-the-word-mom`, `income-gap-rejection`.

## Top emotional engines

**How these are ranked, and why there is no formula.** I weighed five things together and used judgment rather than a score, because no scoring system exists in this data system and inventing one would dress a judgment up as arithmetic. The five: how often the feeling recurs against the 1,342 denominator, how intense it reads, how close it sits to the moment of clicking, how many kinds of source support it, and how useful it would be to a strategist. The fourth of those is identical for every engine here, because there is one source. So the ranking really turns on the other four, and I have said on each one where it sits.

The order below is not the order of the account's spend. That mismatch is the subject of the contradictions section, and it is the most important thing in this document.

---

### Emotion 1 - Indignation at having paid and gotten nothing

**The felt sense.** She did the responsible thing, every month, for years. She paid. And when she needed the thing she paid for, it was not there. This is not worry about the future and it is not fear of a bill. It is the specific anger of someone who kept her side of a deal.

**Frequency.** The strongest signal in the corpus by a wide margin. "deductible" appears in **207 of 1,342 records, 15.4%**, `verified` live today, making it the most-used content word in the whole corpus. The counter-bid behavior underneath it, where she answers the ad's figure with her own, appears in **82 of 1,342, 6.1%**, `verified` live today, across 8 distinct ad names. An upstream pass read all 82: 76 post a specific dollar figure and **64 of those 76, or 84%, name a number higher than the $6,000 the ad states**. Supporting words: "afford" at 47 of 1,342 (3.5%), "scam" at 48 (3.6%), "insane" at 12 (0.9%, **thin**).

**Intensity, with the reasoning.** High, and it is the highest-agreement emotion in the corpus, which is the only proxy for resonance this data offers. The single most-liked record in all 1,342, at 47 likes and 9 replies, is a woman doing exactly this. Roughly three quarters of the corpus carries zero likes, so 47 is agreement on a scale nothing else here reaches. Read on the valence and intensity grid in `emotional-delivery-and-timing.md`, this is high-intensity negative. That matters practically: high arousal narrows her attention onto whatever is in front of her and suppresses the reflective processing that identification needs. It is a good state for provoking a reply and a poor one for making her see herself.

**Where it appears in the journey.** Squarely in **Trigger**, the TEEP phase where a need has just become conscious and she is still making sense of it. She is not comparing plans. She is grieving a bill. Nearly every funded script in the account is written for **Evaluation**, and the mismatch shows in the behavior itself: she answers the ad's number instead of the ad's offer.

**Persona alignment.** `pays-and-still-owes` primarily and `already-knows` strongly. Not `built-it-herself`, whose grievance is structural rather than personal.

**Contextual triggers.** `found-out-the-number` above all. Also `deductible-reset-dread` in December and January, and `employer-plan-locked` when the anger has nowhere to go.

**Verbatim evidence.**

- "This sounds too good to be true. I pay over $1,000 a month for a premium. We have to pay an $8000 deductible per family member or up to $17,000 for the entire family. It's insane. I have 2 members of the family with chronic diseases. This absolutely insane. I want the 1990's back." — row `b7aa4d37-2243-d0fe-03e6-50c8b7d495ca`, `MOMS38 - 1 - V1`, 2026-03-22, 47 likes, 9 replies. `stated` / **inferred emotion**. The most-liked record in the corpus.
- "Why we have insurance and still have a damn bill when we go to the doctor." — row `fd6d3fb4-3868-cc4d-1ebe-ca2e8ef40dc8`, `MOMS38 - 1 - V8`, 2026-04-15. `stated` / **inferred**. The tightest statement of the engine in nine words.
- "Lucky! Mine is $11,000" — row `aa3d6d52-d3a5-63ad-78bb-570b4939eb59`, `MOMS38 - 1 - V3`, 2026-03-17, 19 likes. `stated` / **inferred**.
- "Mine is a 20k deductible before insurance helps with anything. 6k is a dream" — row `c28373d7-0028-0042-fc87-1cc7e3858509`, `MOMS38 - 1 - V2`, 2026-03-21, 7 likes, 6 replies. `stated` / **inferred**.
- "6k....try 13k!" — `MOMS38 - 1 - V1`, 2026-04-02. `stated` / **inferred**.
- "I still pay full price for everything all year until I pay $6k which has been never. They have never helped me pay for anything, but I give them thousands a year for what?" — row `be59e705-66a5-1215-96a0-bdd826f0f68c`, `MOMS38 - 1 - V5`, 2026-04-08. `stated` / **inferred**. **thin** at one record and the sharpest statement of the paying-for-nothing idea in the corpus.
- "Except the premium for that policy costs more than my house note. Who can afford that? If you get a lower premium then your deductible is much higher and no one can afford the higher deductible so either way people are screwed. Broken system" — row `dc090fc7-be0b-3156-eaaa-efcdc96f62c6`, `MOMS33 - N3 - V2`, 2026-02-14. `stated` / **inferred**. Dated 24 days before the creative that produced most of this language, which makes it era evidence that the feeling is hers rather than the ad's.
- "I pay $400 a month, my deductible is 13,000 I make 12700 in a year on disability. Cuz this makes sense." — row `6510e12d-3ac0-df2d-1b6b-af541fcbb690`, `MOMS38 - 1 - V1`, 2026-04-08. `stated` / **inferred**. **thin**. Her deductible is larger than her annual income. Flag for the claims-check governor before any use, since the figures are self-reported and unverifiable.

**Short lifted phrases, for static headlines.**

- "6k is a dream"
- "I want the 1990's back."
- "Broken system"
- "which has been never"
- "costs more than my house note"
- "Wow only 6? Must be nice" — **thin**, 3 records, and it carries 13 likes

**Longer lifted phrases, for video hooks or voiceover starts.**

- "Why we have insurance and still have a damn bill when we go to the doctor."
- "I still pay full price for everything all year until I pay $6k which has been never."
- "If you get a lower premium then your deductible is much higher and no one can afford the higher deductible so either way people are screwed."

**Persona-specific expression notes.**

`pays-and-still-owes` says it clipped and numeric. She leads with a figure and ends with a shrug: "Total. Scam." "Cuz this makes sense." Lift her lines short.

`already-knows` says it long and explanatory. She describes the mechanism that traps her and she has been describing it for years. She will follow a longer setup, which per `advertising-to-older-audiences.md` is the opposite of the usual assumption about this age group. Give her room before the payoff.

`built-it-herself` barely expresses this engine at all. Her version is structural, not personal: "There is no middle class on the marketplace unfortunately."

**One warning that belongs with this engine.** The behavior it produces is a counter-bid. Naming a specific figure reliably invites her to top it, which quietly disqualifies the offer as unrealistic in front of everyone else reading. That is not a reason to abandon the engine. It is a reason to consider whether the creative leads with a number, a range, or no figure at all.

---

### Emotion 2 - Suspicion that she is about to be taken

**The felt sense.** She wants this to be real and she is almost certain it is not. The specific fear is not that the plan will be bad. It is that the moment she types her phone number, her life gets worse.

**Frequency.** Fifteen comments across 10 different ads carry the call-flood objection, carried on the 1,322 denominator. That count is small and the ad spread is wide, which per the mining method is the more durable of the two numbers. Supporting: "scam" at **48 of 1,342, 3.6%**, `verified` live today, though roughly 28 of those aim at the health insurance industry rather than at this brand and only about 11 aim squarely here. "legit" appears in 4 records.

**Intensity, with the reasoning.** Very high relative to its count, and the like data proves it. The sharpest single record drew **33 likes, the third-highest in the entire corpus**. The highest-liked *question* in all 1,342 is a request for a review. A count of fifteen understates this badly, because the quiet version leaves no trace: a woman who thought "I'll get buried in calls" and scrolled past wrote nothing. Treat fifteen as a floor on the doubt, never as its size.

**Where it appears in the journey.** **Evaluation**, and it is the only engine here that sits right at the click. That makes it the most commercially valuable emotion in the document despite ranking second on volume. The emotional-delivery method is direct about this phase: she is not looking for more information, and applying pressure or over-explaining your worth here makes her decide you are not the one. Name the hesitation instead.

**Persona alignment.** All three, and it sharpens as it goes down the list. `built-it-herself` feels it hardest because her phone is her business line.

**Contextual triggers.** `phone-number-guarding` and `post-form-burn`.

**Verbatim evidence.**

- "Filled it out and have been getting calls everyday from all sorts of companies which are mostly India based.  Also, the harassment from whomever keeps calling me about Medicare (India again).  This is the ONLY form I've filled out since getting my new phone number 3 months ago so it came from this site!" — `MOMS38 - 1 - V3`, 2026-03-16, **33 likes**. `stated` / **inferred**. Note the detail she volunteers: she had already changed her number once to escape calls.
- "Anyone actually have this and have insight?" — row `7d74447b-bc85-97f5-c3ec-39d711ff885b`, `MOMS38 - 1 - V1`, 2026-03-20, **15 likes, 6 replies**. `stated` / **inferred**. The highest-liked question in the corpus, and the brand never answered it.
- "How many calls will I get if I try to see how this works?" — row `3707bfa1-c0bd-2629-63b4-6987e500f611`, `Moms36 - 3 - A - 2 - V4c`, 2026-05-17, 17 likes. `stated` / **observed** on the worry, inferred on the distrust.
- "I filled this out because it literally says we won't be contacted by random agents. That's a lie. I immediately received 5 text messages from 5 different agents claiming to be from 5 different companies." — `B1 samar- Copy`, 2025-11-28. `stated` / **inferred**.
- "Really wish you could see plans without adding all your personal information to get even more telemarketing calls than we already do." — `OMC - C11 - 2b`, 2026-03-13. `stated` / **inferred**.
- "I don't wanna put my information and get called by hundreds of people though.." — `MOMS38 - 1 - V8`, 2026-03-11, 2 likes. `stated` / **observed** on the not-wanting.
- "Just give some pricing without making people sign up 🙄" — `MOMS38 - 1 - V1`, 2026-03-15, 3 likes. `stated` / **inferred**.
- "A Google search doesn't pull anything about this. Is it legit?" — `B1 samar- Copy`, 2025-07-24, 1 like. `stated` / **inferred**.

**Short lifted phrases, for static headlines.**

- "Anyone actually have this and have insight?"
- "How many calls will I get if I try to see how this works?"
- "Just give some pricing without making people sign up"

**Longer lifted phrases, for video hooks or voiceover starts.**

- "I filled this out because it literally says we won't be contacted by random agents. That's a lie."
- "Really wish you could see plans without adding all your personal information to get even more telemarketing calls than we already do."

**Persona-specific expression notes.** `pays-and-still-owes` asks it as a warning to other women. `already-knows` asks it as a flat verification question and expects a straight answer, which fits the older-audience pattern where clarity beats cleverness and hype reads as a reason to distrust. `built-it-herself` does not ask at all; she goes looking for something to read and leaves when she finds nothing.

**The shape changed over time, and it matters.** In 2025 this is a report from someone who did it. By 2026 it is pre-emptive fear from someone who has not. That is the objection spreading from experience into reputation, and it is the single clearest case in this corpus of a problem getting worse while nobody addressed it.

---

### Emotion 3 - Recognition, the relief of being described accurately

**The felt sense.** Someone finally said the thing out loud, exactly as it happens, and she does not have to explain it. It arrives as laughter rather than gratitude.

**Frequency.** Roughly **12 clear recognitions across 1,342 records, under 1%**, carried from the full-corpus read. **thin** by any bar, and the thinness is itself the headline finding. For a corpus this size, twelve is very low, and it says the creative is generating argument rather than identification.

**Intensity, with the reasoning.** Individually warm rather than loud, which is exactly why it matters. Read on the valence and intensity grid, this is **low-intensity positive**, and `emotional-delivery-and-timing.md` names that quadrant as the one most brands underinvest in precisely because it is uncomfortable to make. It is also the quadrant that creates identification, which high-intensity creative cannot. So this engine ranks third on count and first on strategic usefulness.

**Where it appears in the journey.** **Trigger**, but a completely different doorway from Emotion 1. Emotion 1 mirrors a number back at her, which she can dispute. This mirrors an experience back at her, which she cannot.

**Where it clusters, and this is the whole finding.** Almost every one of the twelve sits on one creative family, `MOMS38 - 2`, the skit where a single woman plays both a frustrated mom and an insurance rep denying a claim because it happened "in a different hallway." That family holds the account's highest hold rate at 24.48%, double the craft floor of 12% and more than six times the current top spender's 3.28%, which I re-pinned live today. It cost roughly $3,774 across three ads.

**Persona alignment.** `already-knows` above all. This is her engine and the account has barely funded it.

**Contextual triggers.** The claim fight. Hours on the phone losing an argument.

**Verbatim evidence.**

- "\"It's out of network\"  \"But it's in the same building!\"  \"In a different hallway\"  🤣🤣🤣🤣🤣 whoever came up with this ad deserves a raise!! Love this!" — `MOMS38 - 2 - V1`, 2026-04-03, 4 likes. `stated` / **inferred**.
- "TRUTH! A SAD TRUTH." — `MOMS38 - 2 - V1`, 2026-04-06. `stated` / **inferred**.
- "Had a similar conversation recently with my soon to be former insurance company." — `MOMS38 - 2 - V4`, 2026-03-23. `stated` / **inferred**.
- "At the Mayo Clinic for my husband right now.  Absolutely dealing with this." — `MOMS38 - 2 - V1`, 2026-04-06. `stated` / **inferred**.
- "Absolutely accurate" — `MOMS38 - 2 - V3`, 2026-03-31. `stated` / **inferred**.
- "I swear this is true !! lol" — `MOMS38 - 2 - V4`, 2026-03-18. `stated` / **inferred**.
- "I literally was just on the phone for hours today figuring out something eith insurance...and still no answer." — row `622cb438-d58d-9f87-f722-59a7c197eccf`, `MOMS38 - 2 - V1`, 2026-04-04. `stated` / **inferred**. The only pain phrase in the corpus that sits on the recognition creative, and it names time rather than money. The typo is original.

**Short lifted phrases, for static headlines.**

- "TRUTH! A SAD TRUTH."
- "In a different hallway"
- "Absolutely accurate"

**Longer lifted phrases, for video hooks or voiceover starts.**

- "I literally was just on the phone for hours today figuring out something eith insurance...and still no answer."
- "Had a similar conversation recently with my soon to be former insurance company."

**Persona-specific expression notes.** `already-knows` expresses this as laughter with an edge, and she is the only persona who reliably does. `pays-and-still-owes` reaches for it rarely, because her state is anger rather than fatigue. `built-it-herself` does not appear here at all.

**The claims-check note.** Every one of these praises the *ad*, not the product. They are proof that a message landed, never proof that anything was delivered. Do not let one migrate into a testimonial slot.

---

### Emotion 4 - The injury of being excluded by a brand that used her name

**The felt sense.** She was invited by name and then told she does not qualify. The rejection lands on who she is rather than on her wallet, and she reads it as bad faith rather than as a product limit.

**Frequency.** The widest recurring objection in the corpus. The pregnancy exclusion runs **42 comments across 15 different ads over fourteen months**, carried on 1,322, and a stricter independent recount in `voc-objection.md` puts it at 36 across the same 15 ads. The pre-existing condition screen runs **55 across 17 ads**, carried, with a stricter recount of 42 across the same 17. Diabetes alone is named 11 times. The aged-out version runs 16 across 7 ads. Note that the two recounts landed on the *identical* ad spread while the raw counts differed, which is the strongest internal check a single-source corpus can offer and a good reason to trust spread over count.

**Intensity, with the reasoning.** The highest in the document, and it is the only engine that actively damages the brand while it burns. Nine of the pregnancy comments open by quoting the brand's own name back at it before making the point. That is a rhetorical move performed for an audience, not a private hesitation, and it means the injury is being broadcast under paid media.

**Where it appears in the journey.** After **Evaluation** and at the gate. She has already decided to try. This is where the journey ends for her.

**Persona alignment.** This is the engine that does *not* map cleanly to a persona, and that is deliberate. The two loudest groups carrying it, the expecting mother and the chronic-condition family, are **not personas** in `personas/personas-profile.md`, because the product's medical underwriting screens them out and a persona requires a buyer. The one version that does attach to a persona is the aged-out form, which belongs to `already-knows` and her `aged-past-the-word-mom` signal.

**Verbatim evidence.**

- "How can you have healthcare for moms if you don't cover maternity? Makes zero sense. False advertising." — row `3b2ac139-83f3-123e-bd63-6321ff80f4d4`, `B1 samar- Copy`, 2025-08-12. `stated` / **inferred**.
- "Health for Moms, but only if your babies are out of the womb. I was denied for being pregnant. Scam." — row `a04168ce-2e0e-2ceb-7992-d6427575062f`, `MOMS30 - 1 - V20`, 2026-02-03. `stated` / **inferred**.
- "Markets to moms.\nProvides zero plans for moms. 🚩\nMakes perfect sense." — row `184aaf10-b07b-3145-feae-4376d3f497de`, `B1 samar- Copy`, 2025-07-29, 15 likes. `stated` / **inferred**.
- "So because I make under $30,000 and am under 63.. no othe questions that fit as to why I can't get coverage.. I'm a single mom not making enough to afford insurance so who's this plan for if not moms like me? Doesn't seem legit" — `MOMS38 - 1 - V2`, 2026-04-09. `stated` / **inferred**. The sharpest line in the corpus, and note her conclusion is not "this isn't for me" but "this isn't legitimate."
- "Don't bother looking into it if you're diabetic . I'll be uninsured until I die." — row `01b5ff6d-1ea1-b12f-fe1f-136348d8c40b`, `B1 samar- Copy`, 2025-08-14. `stated` / **inferred**. One of only 2 records in 1,342 containing "uninsured."
- "Preexisting health condition of cancer disqualified me" — row `3bcd0ddf-30f5-1e4c-a318-1868b9e7055f`, `moms-63 3e`, 2026-09-02. `stated` / **inferred**. Two days before this doc, which shows the objection is live.
- "OK, this is great for mom's of young children. What about the rest of us? ... What about those of us whose children are grown and moved out of the house now? My deductible used to be reasonable, now it's almost $7000 a year." — `MOMS38 - 1 - V2`, 2026-04-26, 2 likes. `stated` / **inferred**. The `already-knows` version, and note how polite it is.

**Lifted phrases.** **None from the first two groups.** This is the one engine in the document where the right instruction is not to lift. These lines are objections to answer, never claims to make, and building creative around this feeling would send more women into a funnel that rejects them in public using the brand's own name as the punchline.

The aged-out version is different and it is genuinely usable, because the brand *can* serve her:

- "What about the rest of us?"
- "My deductible used to be reasonable, now it's almost $7000 a year."
- "What if your kids are over 18, do I still qualify as a Mom?"

**Persona-specific expression note.** The tone difference is the tell. The excluded mother writes in fury and uses the brand's name as a weapon. `already-knows` asks politely and nobody answers her. The polite one is the one the product can actually sell to.

---

### Emotion 5 - Resignation, the decision to stop trying

**The felt sense.** She has run out of moves. This is not anger, which still expects something. It is the quiet after.

**Frequency.** **thin** and deliberately kept. The clearest records number under ten. The adjacent behavior is larger: 33 comments across 10 ads, carried on 1,322, argue the right answer is to drop insurance and pay cash.

**Intensity.** High per record and very low in volume. The persona method insists volume and emotional intensity stay separate rankings, and this engine is the clearest case in the document of why.

**Where it appears in the journey.** Out of the journey entirely. This is the exit.

**Persona alignment.** None cleanly. The woman leaving the category is watched in the persona profile as a cluster forming, not written up as a persona, because she is not a buyer for this product.

**Verbatim evidence.**

- "I'll be uninsured until I die." — inside row `01b5ff6d-1ea1-b12f-fe1f-136348d8c40b`, `B1 samar- Copy`, 2025-08-14. `stated` / **inferred**.
- "This is me. Im on moujaro for diabetes and now I can't afford it because they want me to pay $1000 a month till my deductible is met. Im lost, can't afford it now." — row `6c7fc8bc-6da9-09e3-2684-a4225d319004`, `MOMS38 - 1 - V1`, 2026-03-30. `stated` / **observed**. "Im lost" is the only place in 1,342 records where anyone names the feeling rather than the figure. The drug misspelling is original.
- "I would rather have no insurance you would get better self-pay rates then you do with \"having coverage\"" — `MOMS38 - 1 - V2`, 2026-03-26, 14 likes. `stated` / **inferred**.
- "It doesn't make sense. It's never made sense." — row `f1f160d4-9962-e98e-eece-5b9bde1234e2`, `Moms43 - 5 - V1`, 2026-09-03. `stated` / **inferred**. The newest record in the corpus.
- "shoot im just trying to figure out on how to pay the monthly charges to get health insurance let alone the charges they dont cover with copays its annoying when im barely making it" — row `aaefb729-af45-6ee5-6dd0-c9017487a6bc`, `MOMS39 - 2 - V2`, 2026-03-22. `stated` / **inferred**.

**Short lifted phrases.**

- "It doesn't make sense. It's never made sense."
- "Im lost"
- "im barely making it"

**Voice-check flags, per the mining method's governor.** "Im lost" and "im barely making it" are **transformable**, not liftable as written. The lowercase and unpunctuated register will not survive into brand copy, and the brand's own guidelines describe its voice as warm and conversational. The observation is the asset; the wording needs rework. "It doesn't make sense. It's never made sense." is **in-voice** and can be lifted as written.

**A hard warning on this engine.** The brand's own best-performing hook, "Health Insurance is a scam 🙄," argues this woman's case for her and then asks her to buy insurance. Thirty-three comments across ten ads take the argument to its natural conclusion and decline the product. Using this engine harder recruits more of her.

---

## Low-confidence signals

Emotions and themes that appeared and did not earn a place. Sample evidence preserved, with what would clarify each.

**Hope, aspiration, and pride.** This is the most important entry in this section, because it is the brand's biggest bet. The account's own AI tags put **Hope on 53.4% of lifetime spend and Pride on 9%**, both re-pinned live today. In the customer language there is almost nothing. The literal string "wife of the year" appears in **0 of 1,342 records**. "overpaying" appears in 1, and it is about drug prices rather than her own insurance choice. What would clarify it: a post-purchase survey or a thank-you page question capturing what a woman says in the minutes after she fills in the form, where hope would plausibly live and a comment section structurally cannot see it.

**Relief and gratitude.** Effectively zero. A semantic sweep for relief and gratitude language across the whole corpus at a 0.35 floor returned **two results total**, and neither is about this brand: one woman is praising her employer's new plan and one is praising a plan she already had. What would clarify it: any surface downstream of the phone call.

**Trust.** The account tags Trust on 0.6% of lifetime spend, re-pinned live. The corpus supports even less. The two positive service records are about manners, not confidence: "he was very kind and helpful and respectful." What would clarify it: agent call notes or a follow-up question after the handoff.

**Fear of a catastrophic bill.** The brand's own document lists "I'm scared one ER visit will wipe us out" as customer language. That exact phrase returns zero. Nobody in this corpus talks about being wiped out; they quote the number instead. The idea does run as a static headline at a $9.62 cost per lead, so the brand demonstrably says it. Whether a customer said it first cannot be settled here. What would clarify it: a brand-free source, or the brand naming where the quote came from.

**Amusement.** Real but tiny. It exists almost entirely on the skit family and is captured under Emotion 3 rather than split out, because on twelve records splitting it would manufacture a second pattern out of one.

**Political anger.** 54 comments across 14 ads, carried on 1,322, and among the highest like counts in the corpus. Deliberately **not** promoted to an engine. It is about American health policy rather than about this brand, this product or this buyer, and the brand's own compliance rules forbid political framing outright. It is logged here so nobody mistakes its size for relevance. What it does tell you is the emotional environment the creative lands in, which is high-intensity negative, and that is carried into Emotion 1.

---

## Creative language opportunities

Words, frames and distinctions the customer is handing over that the brand is not using. Each tied to evidence.

**The audience is supplying more precise vocabulary than the brand uses, and the brand is arguing with it instead.** "out of pocket" and "max out of pocket" appear in 74 of 1,322 records, carried, and 103 comments across 13 ads argue that the ad describes an out-of-pocket maximum rather than a deductible. Self-identified brokers, agents and medical billers are among them. "As a licensed insurance broker this is VERY misleading in the beginning. The first half is talking about a medical maximum out of pocket." This is the textbook messaging opportunity the mining method describes: the customer handing the brand better language than it currently uses. The brand has never used it.

**The weekly unit.** "Insurance through employer we pay $250/week and still have copay of $50." She experiences the bill weekly, not monthly. No ad in the account uses that unit, and it makes the number feel closer.

**"Battle" as the metaphor.** "its a battle for them to cover anything." The mining method flags metaphor as one of the two highest-value signals most passes miss, and this corpus is genuinely poor in it. "Battle" is the best one there is. The others: "scam" as the dominant metaphor at 48 records, "magical plan" as the sarcasm she reaches for when an offer sounds too good, and one record rendered entirely as "🐂 💩."

**The permission she does not know she has.** "if it's an employer insurance, you don't have to sign up with that employer insurance you can decline the coverage and go out and find your own insurance carrier." A customer wrote that to another customer on 2026-05-05. It is the single highest-value unused sentence in this document, it maps to the `employer-plan-locked` signal, and the two statics that touch the idea returned the cheapest leads in the account's history. The brand has never said it.

**The comparison she makes herself.** "costs more than my house note." She measures a premium against a mortgage without being prompted. That is a customer-made frame and it is more concrete than any savings percentage.

**The trap nobody names.** "If you get a lower premium then your deductible is much higher and no one can afford the higher deductible so either way people are screwed." That is the exact bind the brand's offer claims to solve, stated better by a commenter than by any ad in the account.

**Specific odd numbers, which read as real.** "This year it took 35 days to hit our 8k OOP. Next year it could take as few as 1." The mining method names specific, non-round numbers as the top qualifying signal for realness, and this corpus is full of them.

**"A mom is a mom."** Sixteen comments across 7 ads ask whether grown children still count. Zero ads answer. This is the cheapest opportunity in the document: one line of copy against a question the audience is already asking in public.

---

## Contradictions and warnings

This section is not softened, per the prompt.

**The account spends more than half its money on an emotion the customer language does not contain.** Parker's own tags put **Hope on 53.4% of lifetime spend** and Pride on 9%, both re-pinned live today. The corpus contains almost no hope and essentially no pride. Meanwhile Anger sits at 30.6% of tagged spend and Frustration at 15.4%, and those two are nearly the whole corpus. The account's emotional allocation and its audience's emotional reality are close to inverted.

**The brand's four stated outcome phrases return zero, and they were re-checked against the larger corpus.** "I finally understand my insurance," "My family is covered, no matter what," "I made a smart choice," and "No more worrying every time my kid gets sick" each return **0 of 1,342**. The brand context document calls these lines "the outcome language the brand cultivates (and that customers ideally echo)" in one section and lists them under a customer heading in another. Both cannot be true. Any writer who opens that section and lifts from it will ship the brand's own marketing back at the customer as her voice.

**The phrase carrying roughly two thirds of the spend has never been said back once.** "wife of the year" returns **0 of 1,342**. That is not echo and it is not organic. It is a phrase the brand has paid to say millions of times with zero trace in what anyone says in response.

**The persona profile and this document agree on a ranking that the ad account inverts.** The engine with the strongest evidence, indignation, is funded heavily but framed as a number rather than an experience. The engine with the highest strategic value, recognition, holds the account's best hold rate at 24.48% and roughly 0.5% of spend. The engine sitting closest to the click, suspicion, has **zero** creative addressing it anywhere in the account.

**The brand's stated objection list misses the two widest objections in its own comment sections.** It names five: is this legit, I do not want to be sold to, I do not have time, my state probably is not included, and I should wait for open enrollment. "open enrollment" appears in **1 of 1,342 records**. Meanwhile the pregnancy exclusion at 42 comments across 15 ads and the pre-existing screen at 55 across 17, both carried, are on no stated list at all.

**A warning about this corpus that cuts against everything above.** Most of the pain language here was provoked rather than found. Of the 207 comments containing "deductible," **197, or 95.2%, sit inside an 83-day window that opens the day the MOMS38 creative launched on 2026-03-10**. That is a compliment to the creative and a warning about the evidence in the same breath. The feeling is real, the volume is prompted, and the corpus has gone quiet since: since 2026-07-01 it holds only 86 comments, many of them the single word "Help" under one ad. **The brand's only listening post is going silent while the spend continues.**

**A warning about the emotion the brand's best hook recruits.** "Health Insurance is a scam 🙄" is genuinely customer-owned language. The word appears in this brand's comment sections from 2025-01-13, fourteen months before the brand ran the hook, so the brand took the customer's word rather than the reverse, and that is the healthy direction. But agreeing that insurance is a scam recruits the woman whose conclusion is to leave the category, and 33 comments across 10 ads take exactly that path. The hook wins the argument and loses the sale.

---

## Quote appendix

The strongest verbatim evidence, with everything the corpus can carry attached. Every row: source type is `ad-comment`, platform is Facebook or Instagram on Meta ad account act 484897827497337, and **rating or score is null because no such field exists on any row**. `url` is null on every entry because `permalink_url` is null on all 1,342 rows. Product or SKU is null on every entry because no product field exists.

| Quote | Row id | Ad | Date | Likes | Persona tag | Emotion tag | Observed / inferred |
|---|---|---|---|---|---|---|---|
| "This sounds too good to be true. I pay over $1,000 a month for a premium. We have to pay an $8000 deductible per family member or up to $17,000 for the entire family. It's insane. I have 2 members of the family with chronic diseases. This absolutely insane. I want the 1990's back." | `b7aa4d37-2243-d0fe-03e6-50c8b7d495ca` | `MOMS38 - 1 - V1` | 2026-03-22 | 47 | `pays-and-still-owes` | Indignation | inferred |
| "Why we have insurance and still have a damn bill when we go to the doctor." | `fd6d3fb4-3868-cc4d-1ebe-ca2e8ef40dc8` | `MOMS38 - 1 - V8` | 2026-04-15 | 0 | `pays-and-still-owes` | Indignation | inferred |
| "Lucky! Mine is $11,000" | `aa3d6d52-d3a5-63ad-78bb-570b4939eb59` | `MOMS38 - 1 - V3` | 2026-03-17 | 19 | `pays-and-still-owes` | Indignation | inferred |
| "Mine is a 20k deductible before insurance helps with anything. 6k is a dream" | `c28373d7-0028-0042-fc87-1cc7e3858509` | `MOMS38 - 1 - V2` | 2026-03-21 | 7 | `pays-and-still-owes` | Indignation | inferred |
| "I still pay full price for everything all year until I pay $6k which has been never. They have never helped me pay for anything, but I give them thousands a year for what?" | `be59e705-66a5-1215-96a0-bdd826f0f68c` | `MOMS38 - 1 - V5` | 2026-04-08 | 0 | `pays-and-still-owes` | Indignation | inferred |
| "Except the premium for that policy costs more than my house note. Who can afford that? ... either way people are screwed. Broken system" | `dc090fc7-be0b-3156-eaaa-efcdc96f62c6` | `MOMS33 - N3 - V2` | 2026-02-14 | 0 | `pays-and-still-owes` | Indignation | inferred |
| "I pay $400 a month, my deductible is 13,000 I make 12700 in a year on disability. Cuz this makes sense." | `6510e12d-3ac0-df2d-1b6b-af541fcbb690` | `MOMS38 - 1 - V1` | 2026-04-08 | 0 | `pays-and-still-owes` | Indignation | inferred |
| "This year it took 35 days to hit our 8k OOP. Next year it could take as few as 1 depending on how prescriptions hit." | `b3e776b8-a237-3d00-f3ad-8cbf4cf4f298` | `MOMS39 - 2 - V2` | 2026-03-31 | 0 | none, chronic-condition overlay | Indignation | inferred |
| "girl, we pay $2,200 a month and its a battle for them to cover anything. I have MS so I NEED to be covered for my treatments" | `cf52967d-33bb-3f5d-ed9d-138895e40607` | `MOMS38 - 1 - V1` | 2026-03-23 | 4 | none, chronic-condition overlay | Indignation | inferred |
| "Filled it out and have been getting calls everyday from all sorts of companies which are mostly India based. ... This is the ONLY form I've filled out since getting my new phone number 3 months ago so it came from this site!" | carried, see `source-pulls/ad-comments.md` | `MOMS38 - 1 - V3` | 2026-03-16 | 33 | `pays-and-still-owes` | Suspicion | inferred |
| "Anyone actually have this and have insight?" | `7d74447b-bc85-97f5-c3ec-39d711ff885b` | `MOMS38 - 1 - V1` | 2026-03-20 | 15 | `pays-and-still-owes` | Suspicion | inferred |
| "How many calls will I get if I try to see how this works?" | `3707bfa1-c0bd-2629-63b4-6987e500f611` | `Moms36 - 3 - A - 2 - V4c` | 2026-05-17 | 17 | `already-knows` | Suspicion | observed |
| "\"It's out of network\" \"But it's in the same building!\" \"In a different hallway\" 🤣🤣🤣🤣🤣 whoever came up with this ad deserves a raise!! Love this!" | carried, see `source-pulls/ad-comments.md` | `MOMS38 - 2 - V1` | 2026-04-03 | 4 | `already-knows` | Recognition | inferred |
| "I literally was just on the phone for hours today figuring out something eith insurance...and still no answer." | `622cb438-d58d-9f87-f722-59a7c197eccf` | `MOMS38 - 2 - V1` | 2026-04-04 | 0 | `already-knows` | Recognition | inferred |
| "Markets to moms.\nProvides zero plans for moms. 🚩\nMakes perfect sense." | `184aaf10-b07b-3145-feae-4376d3f497de` | `B1 samar- Copy` | 2025-07-29 | 15 | none, excluded overlay | Exclusion injury | inferred |
| "Health for Moms, but only if your babies are out of the womb. I was denied for being pregnant. Scam." | `a04168ce-2e0e-2ceb-7992-d6427575062f` | `MOMS30 - 1 - V20` | 2026-02-03 | 0 | none, excluded overlay | Exclusion injury | inferred |
| "Preexisting health condition of cancer disqualified me" | `3bcd0ddf-30f5-1e4c-a318-1868b9e7055f` | `moms-63 3e` | 2026-09-02 | 0 | none, excluded overlay | Exclusion injury | inferred |
| "OK, this is great for mom's of young children. What about the rest of us? ... My deductible used to be reasonable, now it's almost $7000 a year." | carried, see `source-pulls/ad-comments.md` | `MOMS38 - 1 - V2` | 2026-04-26 | 2 | `already-knows` | Exclusion injury | inferred |
| "Don't bother looking into it if you're diabetic . I'll be uninsured until I die." | `01b5ff6d-1ea1-b12f-fe1f-136348d8c40b` | `B1 samar- Copy` | 2025-08-14 | 0 | none, excluded overlay | Resignation | inferred |
| "This is me. Im on moujaro for diabetes and now I can't afford it because they want me to pay $1000 a month till my deductible is met. Im lost, can't afford it now." | `6c7fc8bc-6da9-09e3-2684-a4225d319004` | `MOMS38 - 1 - V1` | 2026-03-30 | 0 | none, chronic-condition overlay | Resignation | **observed** |
| "It doesn't make sense. It's never made sense." | `f1f160d4-9962-e98e-eece-5b9bde1234e2` | `Moms43 - 5 - V1` | 2026-09-03 | 0 | `pays-and-still-owes` | Resignation | inferred |
| "There is no middle class on the marketplace unfortunately. You either pay next to nothing or almost all of it with no subsidy." | `8a885e35-71be-e442-a0da-f462b6eb3e9f` | `B1 samar- Copy` | 2025-08-09 | 0 | `built-it-herself` | Indignation, structural | inferred |
| "I'm self employed and can't find anything that doesn't have at least $5k deductible" | `2c7f384f-cae6-a020-456c-e5534a427218` | `MOMS39 - 2 - V2` | 2026-04-02 | 7 | `built-it-herself` | Indignation, structural | inferred |
| "Best advice I have gotten from an insurance agent! She didn't have anything that fit but pointed me in the right direction!" | `45bc3e26-5d26-1d96-30c2-686ca6e5fbf8` | `Moms Nahuel WV#1 - V9` | 2026-04-17 | 2 | unassigned | Gratitude, service only | inferred |
| "I was connected to a very helpful agent. They weren't able to find a lower price for our particular situation but he was very kind and helpful and respectful." | `df460383-699e-27a3-e2ef-e4f3197790f4` | `MOMS38 - 1 - V1` | 2026-04-01 | 1 | unassigned | Gratitude, service only | inferred |
| "if it's an employer insurance, you don't have to sign up with that employer insurance you can decline the coverage and go out and find your own insurance carrier" | carried, see `source-pulls/ad-comments.md` | `MOMS38 - 1 - V2` | 2026-05-05 | 0 | `pays-and-still-owes` | Permission, peer-taught | inferred |

### Lookup section — quotes that cannot be treated as clean evidence

These carry no source, no date and no surface. They are listed so a later reader can see exactly what was excluded and why. **They must never be used as voice of customer.** All fourteen come from Section 4 of the brand context document, titled "Customer Language," and every one returns zero hits across all 1,342 comments, re-checked in this run.

"I wish I'd known about this sooner" · "My friend told me about this and I'm so glad she did" · "I can't believe how much I was overpaying" · "I finally understand my insurance" · "My family is covered, no matter what" · "I made a smart choice" · "No more worrying every time my kid gets sick" · "It was so easy — I just answered a few questions" · "They actually explained things in a way I could understand" · "Nobody pressured me — they just showed me my options" · "I don't even know what my plan covers" · "I'm scared one ER visit will wipe us out" · "They don't give a rat's butt about people like me" · "We are super middle class — how are we stuck with everything?"

What is missing on every one: source surface, date, and any evidence that a customer said it.

## Open loops

**1. The account's biggest emotional bet leaves no trace in language at all.**

Parker's own tags put Hope on 53.4% of lifetime spend and Pride on 9%. The phrase carrying roughly two thirds of recent spend, "wife of the year," appears in 0 of 1,342 comments, and "overpaying" appears in 1, about drug prices. Meanwhile the language that does recur, the deductible arithmetic and the word scam, are ones the brand picked up from customers rather than the reverse.

*Pull: Gap.* There is an enormous amount of paid repetition here and zero trace of it in what anyone says back, and nothing has been done with that fact.

*Question:* What words do the moms who actually convert use for the moment they find a better plan?

*Why it matters:* the brand is writing the winning moment in its own voice with no way to check it. If converting moms describe that moment differently, the hook carrying most of the spend is built on invented language that happens to work, and the real version could work harder.

*Territory: Messaging.* **Routed to the brand**, because answering it needs a thank-you page question or agent call notes that no tool can reach.

**2. The only emotion that earns agreement is the one the account barely funds.**

Roughly 12 recognitions exist in 1,342 comments and nearly all sit on the denial skit, which holds 24.48% of viewers against the top spender's 3.28% and cost about $3,774 across three ads. Every other creative earns argument.

*Pull: Resonance.* The comments under that skit read completely differently from the comments under everything else in the account, and I want to know what it is doing that the rest is not.

*Question:* What is the pain this audience recognizes without being shown a price?

*Why it matters:* the account's whole emotional vocabulary is financial, and the only creative earning agreement instead of argument dramatizes an experience rather than a bill. If the recognizable pain is the fight and the phone call, the brand has a second messaging lane it has barely used.

*Territory: Messaging.*

**3. The emotion closest to the click has no creative anywhere.**

Suspicion about what happens to her phone number carries the third-highest-liked record in the corpus at 33 likes and the highest-liked question at 15. It sits at Evaluation, right at the moment of the click. No ad in the account addresses it.

*Pull: Surprise.* Given a lead-generation business whose entire ask is a phone number, finding zero creative that answers the phone-number objection is not what the setup would predict.

*Question:* How much of this audience's hesitation is about what happens after the form?

*Why it matters:* if the barrier is the handoff rather than the offer, then hook testing cannot move it and the fix lives in what the creative promises about the call. That reroutes the next round away from the hook and toward the close.

*Territory: Messaging.*

**4. The corpus that carries every emotion in this document is going quiet.**

Of the 207 comments containing "deductible," 197 sit inside an 83-day window opened by one creative launch on 2026-03-10. Since 2026-07-01 the corpus holds only 86 comments, and many are the single word "Help" under one ad.

*Pull: Surprise.* For a brand still spending heavily, finding that its audience stopped talking to it four months ago is not what the setup would predict, and the size of the drop is the signal.

*Question:* What is different about the creative running now that the audience no longer tells it anything?

*Why it matters:* comment sections are this brand's only source of customer language and its only listening post. If the current creative does not invite disclosure, the brand is losing its research pipeline while the spend continues, and every future refresh of this document gets thinner.

*Territory: Messaging.*

**5. The same feeling means two different things depending on who is carrying it.**

Indignation from `pays-and-still-owes` arrives as a shock, clipped and numeric: "6k....try 13k!" The same indignation from `already-knows` arrives as a long explanation of a system she has watched for years. One is a reaction and one is a verdict.

*Pull: Curiosity.* Two groups use the same emotional register in ways that read as genuinely different states, and nothing in the brand's context explains why the older woman's version is calmer and lasts longer.

*Question:* Why does the older woman in this audience express the same grievance with less heat and more detail?

*Why it matters:* it decides the pacing and length of any creative built on this engine, and the persona profile says she watches three to five times longer than anyone else. If her calm is patience rather than disinterest, the right build for her is the long story the account has never made.

*Territory: Personas.*

---

This is everything I know about advertising to older audiences.
