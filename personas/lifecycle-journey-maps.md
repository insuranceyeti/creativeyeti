---
brand: health-for-moms
doc: lifecycle-journey-maps
generated_on: 2026-09-04
refresh_by: 2026-10-04
personas_profile: personas/personas-profile.md
persona_voice_library: personas/persona-voice-library.md
sources_read:
  - personas/personas-profile.md — the three canonical personas, identity slugs and behavioral-signal slugs this doc maps over time
  - personas/persona-voice-library.md — the five emotional engines and the stage each sits in
  - personas/voice-of-customer/voc-corpus-profile.md, voc-pain-phrase.md, voc-objection.md, voc-trigger-moment.md, voc-outcome-phrase.md, voc-anti-language.md
  - source-pulls/ad-account.md, ad-comments.md, customer-reviews.md, post-purchase-surveys.md, reddit.md, brand-reputation.md, brand-self-echo-detection.md
  - sub-context-docs/customer-journey-and-persona-discovery.md — the prior journey read this doc builds on rather than repeats
  - audits/2026-Q3/quarterly-whitespace-analysis.md
  - running-notes/missing-context.md, brand-rules.md, success-definition.md
  - Parker MCP search_facebook_ads_sql, lifetime and 90-day cuts, run live 2026-09-04 for the delivery, hold-rate and destination figures used below
  - Parker MCP search_facebook_ad_comments_sql, corpus end re-pinned live 2026-09-04 at 1,342
  - Parker MCP search_customer_reviews_sql and semantic_search_post_purchase_survey, both run live 2026-09-04, both zero
measured_lifecycle_fields:
  - cost per lead, lead volume, cost per link click, click-through rate — Meta-reported, 90-day and lifetime
  - hook rate and hold rate per ad — Meta-reported
  - link clicks against landing page views, by destination — Meta-reported, and the source of the one measured leak in this doc
  - delivery demographics by age, gender, platform and device — Meta-reported
  - comment volume, dates, like counts and ad spread — from the 1,342-row corpus
directional_lifecycle_fields:
  - every stage duration and time in stage. Nothing measures how long any step takes.
  - time from first ad exposure to form fill
  - repeat purchase, renewal, cohort behavior, churn, lifetime value, contribution margin — none exist, and most do not apply as the business is currently shaped
  - referral and word of mouth — no measurement of any kind
  - channel pathing beyond Meta — Northbeam is not connected, so all attribution is single-platform
  - everything downstream of the form fill — the call, the enrolment decision, and the outcome are entirely outside Parker's reach
data_limitations:
  - "The standard five-stage lifecycle lens does not fit this business and forcing it would produce a fiction. There is no purchase event in the account at all: zero purchases against 4,421 leads in the trailing 90 days, re-pinned live today. There is no repeat purchase, no subscription, no replenishment, and no order record. The lens used below is a variation, and the reason for each change is given."
  - The brand can see roughly the first half of its own customer journey and nothing after. The conversion Parker measures is a phone number handed to a partner insurance agency. The purchase decision happens on a call at another company, and no artifact of it reaches any surface Parker can read.
  - There is no confirmed customer anywhere in this brain. Customer reviews returned zero live today. Post-purchase surveys returned zero live today. So every stage past the form fill is inferred from absence and from what leaks back into the comment section.
  - There is no outcome or transformation language for this brand. Zero records in 1,342 describe the product delivering its promise. That blank shapes the back half of every map below.
  - author_name is null on all 1,342 comment rows, re-verified live today. Nobody can be followed across stages. Every journey below is assembled from separate comments by separate unknown people, never from one person tracked over time.
  - Lead quality is invisible. The brand's own winner definition is two gates, cost per lead then lead quality, and gate two lives with the partner agencies. Every efficiency figure here clears gate one only.
  - Reddit is unreachable and no competitor brands are tracked, checked live today. So there is no view of how this journey looks outside the brand's own paid media.
  - The comment corpus is skewed: roughly 64% sits in March and April 2026 and roughly 60% on one creative family, both carried on the 1,322 denominator. Stage evidence drawn from it is weighted toward one campaign moment.
  - No get_current_time tool exists on this MCP surface. The date comes from the session clock.
  - refresh_by is 30 days rather than the 180-day persona cadence, matching every sibling doc in this build.
---

# Lifecycle journey maps - Health For Moms

## Purpose and how to use

Three documents work together and each answers a different question.

`personas/personas-profile.md` tells you **who** to talk to. `personas/persona-voice-library.md` tells you **what language** to use. This document tells you **when** to say it, and which specific movement the message is trying to create.

Use it by finding the persona, then the stage she is in, then the transition you are trying to move her through. The message that works at one stage actively hurts at another, and this brand has a live example of that: the account's funded creative is written for the moment of deciding, and most of its audience is standing in the moment of finding out. That mismatch is the subject of the cross-persona patterns section.

**Read this before anything else in the doc.** Everything here past the form fill is inferred from absence. This brand cannot see its own customers. It sees a phone number and then nothing.

## Lifecycle framework

**The standard five-stage lens does not fit this business, so I have not used it.** The prompt allows a variation where the business model requires one, and this one requires it plainly.

Here is why, and the numbers are re-pinned live today. The account produced **4,421 leads and zero purchases** in the trailing 90 days against $100,065.31 of spend. There is no purchase event, no order record, no repeat purchase, no subscription and no replenishment. Health For Moms is not an insurer. It is a matching service: a woman answers a few questions, her details go to a partner insurance agency, and an agent calls her. Whatever she buys, she buys from someone else.

So "first-trial buyer," "repeat buyer" and "subscriber" describe events that do not happen anywhere Health For Moms can observe, and "evangelist" describes a population this corpus shows does not currently exist. Writing those five stages up would produce a tidy document about a business that is not this one.

**The variation, in six stages.** Each is named for what actually happens, and the standard stage it replaces is given so a reader coming from the generic method can orient.

| Stage | What happens | Replaces | Can Parker see it? |
|---|---|---|---|
| **1. Cold scroll** | She is served an ad mid-feed, in whatever emotional state she was already in | Cold prospect | **Yes**, through delivery and hook rate |
| **2. The scan** | The state list appears and she stops to hunt for hers. Two seconds of active searching | Cold prospect, late | **Yes**, through hold rate and click-through |
| **3. The verification hunt** | She goes looking for proof this is real before she gives anything up | *No equivalent in the standard lens* | **Partly**, and only because it happens in the comments |
| **4. The handover** | She trades her phone number. This is the conversion the brand pays for | First trial, loosely | **Yes**, and it is the last thing Parker sees |
| **5. The call** | An agent phones her. The real buying decision happens here, at another company | First trial, actually | **No** |
| **6. After** | She is enrolled, or she is screened out. Then she tells people, or she does not | Repeat, loyal, evangelist | **No**, except what leaks back into the comment section |

**Three things about that table are the whole strategic picture.**

**The brand's sight ends halfway.** Stages 1 through 4 are measured. Stages 5 and 6 are dark. The brand's own definition of a winner is two gates, cost per lead and then lead quality, and gate two lives entirely in stages 5 and 6. So every performance number this brain holds grades the first half of a journey whose second half decides whether any of it was worth it.

**Stage 3 has no equivalent in the standard lens, and for this brand it may be the most important stage there is.** A woman about to hand her phone number to a health insurance ad on Facebook goes looking for a reason to trust it. For most brands she finds a review page. This brand has none. Two live web searches found no Trustpilot page, no Better Business Bureau profile, no press and no third-party review. So the hunt relocates into the ad's own comment section, where strangers answer it and the brand does not.

**Stage 6 runs backward.** In a healthy lifecycle, the far end produces advocates. Here it produces warnings. Across 1,342 comments there are exactly **3 records that read as any kind of defence of this brand, and two of those come from a licensed agent who sells the plans for a living**. Against that, 15 comments across 10 ads warn strangers away, and the sharpest carries 33 likes. The advocacy stage is populated by detractors.

**Movement is not linear and I have not drawn it that way.** A woman can reach stage 3, find a warning, and drop out without ever scanning again. A woman screened out at stage 5 returns to stage 3 as a voice in someone else's verification hunt, which is exactly how this brand's reputation is being written. And a meaningful share never reaches a decision at all, because they meet a gate rather than an offer.

## Data limitations

Restating the ones that shape how much any map below can carry, so nobody has to hunt for them.

**Measured.** Cost per lead, lead volume, click-through, cost per link click, hook rate, hold rate, link clicks against landing page views, and delivery by age, gender, platform and device. All Meta-reported on the org default window, all re-pinned live today.

**Inferred, and directional only.** Every duration. Time from first exposure to form fill. Anything at all about stages 5 and 6.

**Does not exist, and mostly does not apply.** Repeat purchase, subscription, replenishment, cohort behavior, churn, lifetime value, contribution margin, referral tracking, and channel pathing beyond Meta. Some of these are missing data. Most are missing because the business as currently shaped does not generate them.

**One measured thing that looks like a lifecycle finding and is not.** The `go.healthformoms.co/save/` destination converted 690 link clicks into 63 landing page views, a 9.1% landing rate at a $273.23 cost per lead, while the identical creative pointing at `www.healthformoms.co/save/` converted 213 clicks into 171 views, 80.3%, at $19.25. Same hook, same file, same audience. That is a page or tracking fault sitting between stage 2 and stage 4, not a customer behavior, and it inflates the cost per lead of every ad pointed at it. It is named here so no later reader mistakes a broken redirect for a drop-off pattern.

## Cross-persona summary

**Stage 1, cold scroll.** All three personas are reached, and the account reaches them with different creative without meaning to. `pays-and-still-owes` is who the warm aspirational openers find, which take the large majority of the budget. `already-knows` is who the grievance and skit openers find: those put 30% to 38% of their spend on women 45 and over against 7% to 12% for the warm ones, and the format cut reproduces it, with Skit sending 31.5% of its lifetime spend to the 45-and-over band against POV's 10.6%, re-pinned live today. `built-it-herself` is barely reached at all, at roughly 0.25% of lifetime spend.

**Stage 2, the scan.** This is the account's one genuinely strong mechanism and it works on everyone. The full-screen approved state list turns a passive watch into an active search in about two seconds, and it doubles as a scarcity device in a category where the brand has forbidden itself the word discount. It is also a single point of failure, because roughly 92.7% of spend closes on it and nothing else has been tried.

**Stage 3, the verification hunt.** This is where the personas diverge hardest and where the brand invests nothing. `pays-and-still-owes` asks the comment section. `already-knows` wants a credential and finds a frustrated peer instead. `built-it-herself` goes looking for something to read and leaves when there is nothing.

**Stage 4, the handover.** The objection here is identical across all three and it is the only objection sitting directly on the click: what happens to my phone number. No creative in the account addresses it.

**Stage 5, the call.** Dark for everyone. The one thing visible is that a large share never gets a real call at all, because a gate stops them first.

**Stage 6, after.** Dark, and what leaks back is negative. Two positive service records exist in 1,342 comments and both come from women who were told no and thanked the agent anyway.

**Where the brand should invest first, on the evidence.** Stage 3 for `pays-and-still-owes`, because that is the largest audience meeting the loudest unanswered objection at the point closest to the money. Then stage 1 for `already-knows`, because she is the most attentive audience in the account and has never had an ad built for her on purpose.

---

## Persona 1 - The One Who Pays and Still Owes

`pays-and-still-owes` · flagship · confidence **mixed**

She is the largest identity in the comment corpus and the one the account's money is aimed at, though aimed on a wrong premise. Her journey is genuinely short at the front and completely invisible at the back. She is not researching a category she does not understand; she has been paying into it for years. What moves her is not learning that better coverage exists. It is being given permission to doubt the plan she already has, and then being made to feel safe enough to hand over a phone number she has learned to protect.

### The journey arc

She is scrolling at night on her phone, which is where 99.5% of this account's spend lands. An ad names a deductible figure. She does not evaluate the offer; she answers the number, because the number is the thing she has been carrying. That is the whole of stage 1 for her, and it happens in seconds.

If the state list catches her, she scans it. If her state is there she has a reason to keep going, and if it is not the gate becomes a rejection instead of a hook. Then she stops, because the ask is her phone number and she has been burned before or has watched someone else get burned in the same comment thread she is reading. That pause is stage 3 and it is where this persona is lost in the largest numbers. If she pushes through, she gives the number, and from that moment the brand cannot see her.

### Stage by stage

**Stage 1 — Cold scroll.**
*Mindset:* not shopping. Carrying a grievance she has not put down.
*Entry triggers:* `found-out-the-number`, and `deductible-reset-dread` in December and January.
*What moves her forward:* being agreed with before being sold to.
*Drop-off risk:* the creative opens on a life she does not have. The most direct evidence is a comment on the aspirational montage from 2026-09-03: "I'm sure the mom that can afford matching outfits prob just pays in cash 🤦‍♀️."
*Best touchpoint:* paid social, and there is effectively nothing else. Discovery for this brand is one door.
*Key emotion:* indignation at having paid and gotten nothing.

**Stage 2 — The scan.**
*Mindset:* briefly active. Hunting for her state.
*What moves her forward:* seeing her state, plus the friction promise that follows it in nearly every script, "It'll take you 30 seconds."
*Drop-off risk:* `state-list-rejection`. "I didn't see my state... So why am I getting this ad?" And the list can read as a lie when it looks too long: "Ha… 'in these states' proceeds to list all 50 states… scam," 2026-03-26.
*Key emotion:* curiosity, briefly.

**Stage 3 — The verification hunt.**
*Mindset:* wants this to be real and expects it is not.
*What moves her forward:* nothing the brand currently provides.
*Drop-off risk:* the highest in the journey. She looks the brand up and finds nothing. "A Google search doesn't pull anything about this. Is it legit?" 2025-07-24. She asks the comment section and gets answers from strangers. The highest-liked question in all 1,342 comments is exactly this, at 15 likes and 6 replies: "Anyone actually have this and have insight?" The brand never replied. Of the five replies, four were negative or neutral.
*Best touchpoint:* the comment section, which the brand is not working.
*Key emotion:* suspicion that she is about to be taken.

**Stage 4 — The handover.**
*Mindset:* one objection left, and it is not the plan.
*What moves her forward:* naming the hesitation rather than adding pressure. The one ad in the account that does this, `moms-63 3e`, opens "I almost scrolled past this because I thought, 'I already have health insurance, this doesn't apply to me,'" and runs a $15.46 cost per lead against a roughly $22.63 account average.
*Drop-off risk:* `phone-number-guarding`. "Really wish you could see plans without adding all your personal information to get even more telemarketing calls than we already do."
*Key emotion:* suspicion, at its peak.

**Stage 5 — The call.** Dark. What little leaks back divides into two opposite failures, and both are real. Some report a flood: "I immediately received 5 text messages from 5 different agents claiming to be from 5 different companies." Others report silence: "I have signed up for the services and I've not recieved a call back yet," 2025-06-25. Those cannot both describe the same funnel behaving one way, and nobody has reconciled them.

**Stage 6 — After.** Dark. The one complete journey anyone has ever reported ended badly and it arrived on 2026-09-03: "I called them they spammed me and wasted hours of my time to tell me it was going to cost $400/month LOL SO IT DOESNT SAVE YOU $400." One record, so **thin**, and it is the entire evidence base for what the product delivers.

### T-E-E-P decomposition, cold scroll to handover

Read through `emotional-delivery-and-timing.md`.

**Trigger.** This is where she actually is, and it is the account's central mismatch. She has just been reminded what her plan costs. The creative that fits mirrors her internal state back with precision before introducing anything. The evidence that she is here rather than further along is behavioral: she answers the ad's number with her own instead of answering the offer, 82 times across 8 ad names.

**Exploration.** Very short for her, because she is not building a mental map of a category she already lives in. What she is actually exploring is whether this specific company is real, which is stage 3 above.

**Evaluation.** One objection, and it is the phone number. The emotional-delivery method is direct here: she is not looking for more information, and over-explaining your worth at this moment makes her decide you are not the one. Name the hesitation.

**Purchase.** Subtract. The state list already does the qualifying work; nothing else should be added.

### The critical transition

**Stage 3 to stage 4: from "what happens to my number" to "this is safe."**

This is the most valuable movement in the whole document. It matters because it is the only thing the ad actually asks her to do, and the loudest voice in her comment section is warning her against doing it. The brand's own site copy is being quoted back at it as a broken promise: "It listed no selling my number to scammers but it's been just a few hours and I've had multiple numbers contact me," 2026-01-28.

Marked **inferred** on the size and **measured** on nothing, because no join exists between a comment and a lead. The logic is hard to argue with even so.

### Drop-off pattern and win-back

**Where she drops:** stage 3, in the largest numbers, and silently. The 15 comments that voice it are the loud tail of something much larger, because a woman who thought it and scrolled past wrote nothing.

**The win-back move that fits her:** there is no email list and no retargeting creative for a woman who filled the form and did not answer the phone, which the ad-account read confirms as an absence. So the honest win-back is not a message at all; it is answering the question at stage 3 before she reaches stage 4. Given she is `phone-number-guarding`, a win-back that arrives as another phone call is the worst possible instrument.

---

## Persona 2 - The Woman Who Already Knows

`already-knows` · secondary · confidence **mixed**

Her journey is the longest in the account and the least served. She has been managing this problem for around twenty years, and she arrives at the ad already holding a complete view of the category. What she is missing is not information. It is any sign that the brand is talking to her, and any credential she can trust. She watches three to five times longer than anyone the account courts and has never had a single ad built for her on purpose.

### The journey arc

She is on Facebook rather than Instagram: the skit family that reaches her delivered 87.7% of its trailing-quarter spend to Facebook, re-pinned live today, against roughly 60% for the account overall. An ad opens on a frustrated woman or a claims-denial sketch, and she stays. She stays for a long time, which is the single most measurable fact about her: hold rates on the creative that finds her run 7.6% to 24.48%, against 2.4% to 4.3% on the account's biggest spender, whose hold rate I re-pinned live today at 3.28%.

Then she reaches the word "mom" and often stops, because she has concluded it means an eligibility rule rather than an identity. If she gets past that she wants a credential, and the account offers her a peer filming herself at home. Per `advertising-to-older-audiences.md`, an unfamiliar creator carries none of the weight an expert or a news-style frame does for this group, and the only people in 1,342 comments who speak with recognized authority are brokers and agents, several of them pitching against the brand.

### Stage by stage

**Stage 1 — Cold scroll.**
*Mindset:* tired of this and willing to watch someone say so.
*Entry triggers:* `the-claim-fight` above all, plus `found-out-the-number` in its slower form.
*What moves her forward:* recognition. The only creative in the corpus that earns agreement instead of argument is the denial skit, and nearly all of the roughly 12 recognitions sit there. "'It's out of network' 'But it's in the same building!' 'In a different hallway' 🤣🤣🤣🤣🤣 whoever came up with this ad deserves a raise!! Love this!"
*Drop-off risk:* fast cutting and a young cast. The older-audience method is blunt that rapid editing reads as chaos rather than energy for this group, and that proof from a much younger face does not transfer because she does not see herself in it.
*Best touchpoint:* Facebook feed, longer runtime, slower cuts.
*Key emotion:* recognition, the relief of being described accurately.

**Stage 2 — The scan.**
*Mindset:* engaged and reading carefully. She reads the whole list.
*What moves her forward:* legibility. Big type and one clear thing on screen, which the older-audience method names as the whole game rather than a nicety.
*Drop-off risk:* `aged-past-the-word-mom`, and this is her defining drop. Sixteen comments across 7 ads, carried on 1,322, ask whether she still counts. "What if your kids are over 18, do I still qualify as a Mom?" Nobody answers on the thread.
*Key emotion:* the injury of being excluded by a brand that used her name.

**Stage 3 — The verification hunt.**
*Mindset:* wants a credential, not a testimonial.
*What moves her forward:* an authority. For this group the trust shortcut is a licensed professional or a format that looks like something established, and the brand has a compliant version available in its own partner agents, who are real and licensed and already inside the funnel. The one ad that cast a clinician, `MOMS30 - 1 - V20`, put a pediatrician on screen and never let her speak; it returned 381 leads at a $19.44 cost per lead on a 2.44% hold rate, which is exactly what an opener that promises authority and a body that never delivers it would produce.
*Drop-off risk:* she finds nothing, or she finds the pasted summary claiming Reddit considers the brand a scam, which has sat under a live ad since 2025-01-13 with 14 likes and 10 replies.
*Key emotion:* suspicion, expressed as a flat request for evidence.

**Stage 4 — The handover.**
*Mindset:* value-conscious and unhurried.
*What moves her forward:* the value spelled out plainly. The older-audience method is clear that this group is price-sensitive and that scarcity games and hype underperform against a legible explanation of what you get.
*Drop-off risk:* `phone-number-guarding`, shared with Persona 1. Her version of the question carries 17 likes: "How many calls will I get if I try to see how this works?"
*Key emotion:* suspicion.

**Stage 5 — The call.** Dark, with one twist specific to her. She is often healthy enough to pass underwriting and expensive enough to care, which on the face of it makes her closer to the product's real buyer than a woman in her late twenties with a newborn. That is `inferred` from her stated deductible figures and her age band, and nothing available can confirm it.

**Stage 6 — After.** Dark. She is also the persona most likely to become the credentialed guard in someone else's stage 3, whether the brand serves her or not: "From a former insurance agent who is only offering advice since I am no longer selling."

### T-E-E-P decomposition, cold scroll to handover

**Trigger.** She has been in Trigger for years, which is unusual and important. She does not need the problem built; she needs it named. The account has proof this works and has funded it at roughly 0.5% of spend.

**Exploration.** This is her long stage and the account has nothing in it. What lands here is a point of view and the emotional texture of being a customer, not features. Per the older-audience method she will follow a longer, problem-aware story rather than bailing at three seconds, so the format that fits is the one the account has never made.

**Evaluation.** Her objection is eligibility, not category trust. One explicit line telling her she is included would move her, and direct callouts pull relevance for this group while subtlety underperforms.

**Purchase.** Legibility and a plain statement of value.

### The critical transition

**Stage 2 to stage 3: from "this is not for me" to "this includes me."**

It matters because it is the cheapest fix in the entire document. She is not objecting to the product, the price or the trustworthiness. She has quietly concluded she is not eligible, on the strength of one word, and she is asking politely whether she is wrong. That is a line of copy against a question 16 comments across 7 ads are already asking in public.

Marked **inferred** on the volume, because comment count almost certainly undercounts her badly. She absorbs 30% to 38% of grievance-ad spend and leaves 16 comments, which suggests she watches and does not type.

### Drop-off pattern and win-back

**Where she drops:** stage 2, on the word "mom," and stage 3, on the missing credential.

**The win-back move that fits her:** an authority-led explainer with an explicit age or life-stage callout, slow cuts and large type. What does not fit her is the account's current instinct, which is a faster, warmer, younger cut of the same thing.

---

## Persona 3 - The One Who Built It Herself

`built-it-herself` · emerging · confidence **thin**

Her journey is the longest and the most considered of the three, and the account barely touches it. She is not reacting to an ad; she is running a slow, deliberate search that may take months, and she reads everything before she talks to anyone. The brand gives her nothing to read.

**A caution that governs this whole map.** This persona rests on roughly six relevant comment records plus a stated brand ICP. The journey below is more `inferred` than the other two and should be read as a hypothesis about a person who may or may not be in this audience.

### The journey arc

She is not scrolling idly; she is periodically working the problem. Her trigger is a moment of stability rather than a moment of pain: a good month, finishing her taxes, anything proving the business is real enough to insure. That is `stated` by the brand and not corroborated by the corpus.

She arrives already knowing the trap she is in, and she can describe it better than the ad can: "There is no middle class on the marketplace unfortunately. You either pay next to nothing or almost all of it with no subsidy," 2025-08-09. What she wants is a number she can plan against, because in a self-employed household every dollar already has a job. She will not phone anyone until she has read enough to know what she is walking into, and this brand's funnel offers no prices, no plan details and no comparison. So she leaves before stage 4.

### Stage by stage

**Stage 1 — Cold scroll.** *Mindset:* working a known problem. *Trigger:* `a-good-month`. *Drop-off risk:* every funded script assumes she has an employer plan she is overpaying on, which is a different situation entirely. *Key emotion:* structural indignation.

**Stage 2 — The scan.** *Mindset:* checking whether this is even a category match. *Drop-off risk:* `income-gap-rejection`. "But if you make under 30k a year you don't qualify smh," 2026-09-01.

**Stage 3 — The verification hunt.** *Mindset:* reading. *What moves her forward:* something substantial to read, which does not exist. The brand's own document says she "will read every FAQ on a website before she picks up the phone." *Drop-off risk:* the highest in her journey, and it is a content gap rather than a trust gap.

**Stage 4 — The handover.** *Drop-off risk:* `phone-number-guarding`, sharpest for her because her phone is her business line.

**Stages 5 and 6.** Dark, and thinner than for the other two, since almost nobody matching her has left a trace.

### T-E-E-P decomposition, cold scroll to handover

**Trigger.** She is past it. Building the problem for her wastes the opening.

**Exploration.** Her longest stage by far and the account's biggest hole for her. She needs a comparison she can finish alone.

**Evaluation.** Her objection is that she cannot see anything before committing. Naming a price range would move her more than any hook.

**Purchase.** Subtract. She has decided by the time she calls.

### The critical transition

**Stage 3 to stage 4: from "I have nothing to read" to "I know what I am walking into."**

Marked **inferred** throughout and thin.

**A hard constraint on this transition, stated plainly.** Her whole story is a comparison between two things the brand's compliance rules forbid naming. Section 8 of the brand context document bans government and ACA references and lists "ACA" among words never used in creative. Seventeen comments name Medicaid and fourteen name the marketplace, both carried on 1,322. Written without those two nouns most of her story survives: the income figure, the cliff, the plan that costs more than the house note. Written with them it is sharper and against the rules. That reconciliation belongs to the brand, not to this doc.

### Drop-off pattern and win-back

**Where she drops:** stage 3, on an absence of substance.

**The win-back move that fits her:** a page she can read, not a call. She is the one persona for whom a content asset would do more than any creative.

---

## Cross-persona patterns

Real findings visible across more than one persona, not summaries.

**One. The brand pays for the first half of a journey and grades itself on the handoff.** All three personas hit a wall at the same place, and it is the place the brand stops being able to see. The account's own conversion built to track a booked consultation returned no data at all in the window, and only 42 `Call` events fired against thousands of leads. Every persona's most consequential moment happens where nobody is looking.

**Two. Verification is a stage this category has and this brand has no answer for.** It shows up for all three, expressed three different ways: the comment section for `pays-and-still-owes`, a missing credential for `already-knows`, a missing document for `built-it-herself`. The brand has no review page, no third-party profile and no search presence, and customers have noticed and drawn a conclusion. "I tried to look at them through a regular internet browser and nothing comes up...the link only works through Facebook and they want all your information before they show you anything....sounds like a scam to me," 2025-01-20. For this audience, having no findable reputation is not neutral. It reads as concealment.

**Three. The single objection sitting on the click is shared by every persona and addressed by no creative.** What happens to my phone number. Fifteen comments across 10 ads, carried, and the sharpest carries 33 likes. This is the clearest case in the whole build of a known, repeated, high-agreement barrier with zero creative response.

**Four. A large share of this journey ends at a gate rather than a decision, and the brand is paying to create it.** The pregnancy exclusion runs 42 comments across 15 ads over fourteen months and the pre-existing screen 55 across 17, both carried. Neither appears on the brand's own stated objection list. Both groups reach stage 4, hand over their details, and are rejected at stage 5. Then they return to stage 3 as a voice in another woman's verification hunt. That is a loop the advertising funds and the funnel closes badly.

**Five. Advocacy runs in reverse, and the mechanism is visible.** A healthy stage 6 produces defenders. This one produces the replies under "Anyone actually have this and have insight?" Three defences exist in 1,342 comments and two come from a salesman. Meanwhile the women who were rejected are articulate, motivated and already in the thread.

**Six. The two positive records that do exist point at a person, not a product.** Both praise an agent who could not help them. "he was very kind and helpful and respectful." Both were told no. That is unusual enough to name, and it suggests the consultation itself carries value even when it produces nothing to sell. It is the only positive lifecycle signal this brand has and it sits at stage 5, the stage nobody can see.

## Critical-transition map

| Persona | Most important transition | Why it matters | Measured or inferred |
|---|---|---|---|
| `pays-and-still-owes` | Stage 3 to 4 — from "what happens to my number" to "this is safe" | It is the only thing the ad asks her to do, and the loudest voice in her comment section warns her against it. The largest audience meeting the loudest objection at the point closest to the money. | **Inferred.** No join exists between a comment and a lead. |
| `already-knows` | Stage 2 to 3 — from "this is not for me" to "this includes me" | The cheapest fix in the document. She is not objecting to price, product or trust. She thinks she is ineligible, on one word, and asks politely. | **Inferred** on volume; the age split behind her is **measured** through delivery. |
| `built-it-herself` | Stage 3 to 4 — from "I have nothing to read" to "I know what I am walking into" | She will not call before she reads and there is nothing to read. A content gap, not a creative one. | **Inferred**, and thin. |
| All three | Stage 4 to 5 — the handoff to the partner agency | Where the brand's two-gate winner definition actually resolves, and where it cannot see. | **Not measured at all.** |

## Recommendations

Only where the sources support them. Each names the persona, the stage, the action, the evidence and the limitation.

**1. Answer the verification question inside the creative, before she has to go looking.**
*Persona:* `pays-and-still-owes`, and it helps all three.
*Stage:* 3, moving to 4.
*Action:* say in the ad what happens after the form. Who calls, how many people, and what does not happen to her number.
*Evidence:* 15 comments across 10 ads, carried; the sharpest at 33 likes, third-highest in the corpus; the highest-liked question in all 1,342 is a request for a review at 15 likes and 6 replies. The one ad that names a hesitation out loud rather than adding pressure runs a $15.46 cost per lead against a roughly $22.63 average.
*Limitation:* nothing connects a comment to a lost lead, so the size of the win is unknown. The direction is well evidenced; the magnitude is not.

**2. Say that a mom is a mom whether her kid is four or twenty-four.**
*Persona:* `already-knows`.
*Stage:* 2, moving to 3.
*Action:* one explicit callout line naming her in.
*Evidence:* 16 comments across 7 ads, carried, asking exactly this and never answered. She absorbs 30% to 38% of grievance-ad spend and holds at 7.6% to 24.48% against the top spender's 3.28%, re-pinned live.
*Limitation:* her true size cannot be read from comment volume, since she appears to watch far more than she types.

**3. Build the long, slow, authority-led story the account has never made.**
*Persona:* `already-knows`.
*Stage:* 1 through 3.
*Action:* slower cuts, larger type, a longer problem setup, and a real licensed partner agent carrying the credential.
*Evidence:* the format age lever, re-pinned live today, with Skit at 31.5% of lifetime spend to the 45-and-over band against POV's 10.6%. The clinician ad that never let its clinician speak returned $19.44 per lead on a 2.44% hold rate. `advertising-to-older-audiences.md` on narrative tolerance, authority as the trust shortcut, legibility and age-matched proof.
*Limitation:* the sharpest single figure, Skit at 34.8% in the 90-day window, sits on only $712.20 of spend. Lean on the lifetime cut, not that one.

**4. Work the comment section as a lifecycle surface rather than a housekeeping chore.**
*Persona:* all three.
*Stage:* 3.
*Action:* answer the eligibility and phone-number questions where they are already being asked.
*Evidence:* 166 of 1,342 comments contain a question mark and 42 contain "qualify," both carried on 1,322. The brand does not answer. Rival agents do: 39 comments across 10 ads pitch competing offers, 17 of them under the single highest-spend ad.
*Limitation:* no measurement exists for what replying would do.

**5. Stop recruiting the two groups the funnel rejects.**
*Persona:* none of the three. This protects all of them.
*Stage:* 1.
*Action:* keep pregnancy and chronic-condition framing out of the creative and answer the objection honestly when it appears.
*Evidence:* 42 comments across 15 ads over fourteen months on pregnancy and 55 across 17 on pre-existing conditions, both carried; nine of the pregnancy comments open by quoting the brand's own name back at it.
*Limitation:* nobody outside the brand can count how many of the leads met the gate instead of the offer, which is loop 2 below.

**A recommendation deliberately not made.** No retention, repeat-purchase, subscription or loyalty recommendation appears here. Not because the sources are thin, but because the business as currently shaped does not generate those events anywhere Health For Moms can act on them. Making one would be forcing a lens the evidence rejects.

## Open loops

**1. Half of this brand's customer journey has never been observed by anyone who could act on it.**

Stages 5 and 6 are entirely dark. The account produced 4,421 leads in the trailing 90 days and the conversion built to track a booked consultation returned no data at all, with only 42 `Call` events firing. The brand's own winner definition needs gate two and gate two lives in the dark half.

*Pull: Gap.* Thousands of confirmed actions a quarter, and not one artifact of what happened next exists on any surface this brain can read.

*Question:* What happens to a woman after she hands over her phone number?

*Why it matters:* every persona ranking, every cost-per-lead comparison, and every creative call in this build grades the first half of a journey whose second half decides whether any of it worked. Nothing else in the lifecycle system matters as much as this answer.

*Territory: Product.* **Routed to the brand**, because the answer lives in the partner agencies' systems.

**2. Nobody knows how many women meet a gate instead of an offer.**

The pregnancy exclusion runs 42 comments across 15 ads over fourteen months and the pre-existing screen 55 across 17, both carried. One woman reported taking the qualifier twice with different answers and still being turned away.

*Pull: Tension.* The account is graded on cost per lead while an unmeasured share of the traffic it buys appears to be screened out after the click, and both cannot be the real picture at once.

*Question:* What share of the women who start the qualification flow are screened out?

*Why it matters:* if the share is large, the cheapest fix in the business sits upstream of creative, in who the ads invite, and no amount of hook testing touches it. If it is small, the objection is loud and cheap and the answer is a line of copy.

*Territory: Product.* **Routed to the brand**, because it needs the funnel's own screen-out data.

**3. Two groups of women describe opposite failures of the same handoff.**

One group reports being flooded with calls within minutes. Another reports that nobody ever called at all. Both describe the same funnel in the same window.

*Pull: Tension.* It fired when the two complaint families landed side by side and could not both describe one system behaving one way.

*Question:* What decides whether a woman who fills in the form gets flooded with calls or gets nothing?

*Why it matters:* these are opposite failures needing opposite fixes and both are killing conversion in public. If it turns out to be which partner agency the lead lands with, that is a routing problem the brand can act on this month.

*Territory: Product.* **Routed to the brand**, because it needs the handoff logs.

**4. Nobody knows whether a lead is worth anything after the first year.**

The brand hands a woman to a partner agency and she buys an annual policy from that agency. Health insurance renews every year, but no document in this brain records whether Health For Moms earns anything on a renewal, and there is no lifetime value, cohort or contribution margin figure anywhere.

*Pull: Curiosity.* A category that renews annually should have an obvious repeat economics story, and this brand's context document does not contain one at all.

*Question:* How much is one matched mom worth to this business over her whole relationship with the partner agency?

*Why it matters:* it sets the ceiling on what a lead can cost, and right now there is no ceiling to grade against, so "efficient" only means cheaper than this account's own trailing average rather than good for the business.

*Territory: Product.* **Routed to the brand**, because only the team and its partner agencies know the commercial terms.

**5. The most engaged woman in the account leaves almost no trace in its comment sections.**

`already-knows` absorbs 30% to 38% of grievance-ad spend and holds at up to 24.48% against the top spender's 3.28%, and she accounts for roughly 16 comments across 7 ads. The women the account spends most of its money reaching type far more and watch far less.

*Pull: Surprise.* The audience that watches longest being nearly silent is the opposite of what the setup would predict, and the gap between her attention and her volume is the signal.

*Question:* Why does the older woman in this audience watch so much more and say so much less?

*Why it matters:* every count in this build is a comment count, so if she systematically watches without typing then she is being undercounted everywhere in the persona system, and the brand is sizing her from the one instrument that cannot see her.

*Territory: Personas.*

---

This is everything I know about advertising to older audiences.
