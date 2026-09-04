---
brand: health-for-moms
doc: post-purchase-surveys
generated_on: 2026-09-04
refresh_by: 2026-10-04
sources_read:
  - Parker MCP semantic_search_post_purchase_survey, brand aed0ff06-555d-4f4f-9bf8-31178e2fb977, run live 2026-09-04 in lookup mode with no query and no filters beyond the brand, topK 50. Returned count 0, uniqueResponses 0, totalResponsesForBrand 0, collectionExists true
  - Parker MCP lookup_post_purchase_survey, same brand, run live 2026-09-04 against questionId q_01 across all four numeric question types. Returned surveyResponseIds empty, count 0, matchedAnswers 0, totalResponsesForBrand 0
  - Parker MCP search_customer_reviews_sql, run live 2026-09-04, to confirm that the sibling top-tier source is also empty. Returned totalResults 0
  - running-notes/missing-context.md, running-notes/brand-rules.md, running-notes/success-definition.md
  - source-pulls/ad-comments.md, source-pulls/customer-reviews.md, source-pulls/brand-self-echo-detection.md, sub-context-docs/reputation-analysis.md, read as context for what this blank costs
  - Method docs, read before analysis - persona-research-and-creative-strategy-process.md, customer-review-mining-method.md, expertise-routing.md
responses_read: 0 of 0. No survey exists, so there is no window, no question set and no denominator
survey_platform_connected: none
questions_asked_by_the_brand: none
data_limitations:
  - There is no post-purchase survey for this brand on any platform. Two different Parker tools were run live today, one in lookup mode and one against a numeric question id, and both returned zero against a collection that exists. No KnoCommerce, no Zigpoll, no CSV upload.
  - This is the strongest evidence tier in the persona method and it is entirely absent. The second-strongest tier, first-party reviews, is also at zero. See source-pulls/customer-reviews.md.
  - The account has no purchase event at all. 4,336 leads and zero purchases in the last 90 days, verified in the Phase 0 pull on 2026-09-03 and recorded in running-notes/brand-rules.md. So there is no post-purchase moment for a post-purchase survey to attach to.
  - Northbeam is not connected, so the discovery question this doc normally reads for persona signal is dark on the quantitative side too. All attribution is Meta-reported.
  - There is no get_current_time tool on this MCP surface. The 2026-09-04 date comes from the session clock and matches the most recent doc in this build.
  - refresh_by is set 30 days out rather than the 180-day persona-source cadence in parker-system/system/refresh-cadence.md. This is a blank waiting on a decision the brand has not made yet, and the moment a survey is switched on the doc changes completely. Re-checking costs one tool call.
---

# Post-purchase surveys — persona signal — Health For Moms

## What this doc is, and why it is short

**Health For Moms has no post-purchase survey.** Zero responses, no platform connected, no file uploaded.

I checked it live today through two different tools that reach the data in two different ways, because a single empty result is worth less than two.

The first was a lookup. I passed only the brand and asked for up to 50 rows with no query at all, which enumerates everything the store holds for this brand rather than ranking anything. It came back with `count: 0`, `uniqueResponses: 0`, `totalResponsesForBrand: 0`, and `collectionExists: true`. The collection is built and connected. There is nothing in it.

The second went at the numeric side, which lives somewhere else. Survey ratings and scores are not embedded as vectors, so they are queried through a separate path. I asked it for any response with an answer to question `q_01` across all four numeric types, nps, rating, star and currency. It returned `matchedAnswers: 0` and again `totalResponsesForBrand: 0`, with the message "This brand has no post-purchase survey responses yet."

So both halves of the survey store, the text side and the number side, are empty. `running-notes/missing-context.md` recorded this on 2026-09-03 from the Phase 0 surface test, and it holds today.

The right output is a short honest document. This brand does have a substitution rule that lets Facebook ad comments stand in for customer evidence elsewhere, clearly labelled, and `source-pulls/ad-comments.md` uses it well across 1,322 comments. **That substitution does not belong here.** This doc is the record that the surface itself is empty. Padding it with comment data would hand the persona synthesis a false top tier, and the whole point of the evidence ladder is that the top tier means something.

## The deeper problem: there is no purchase

Before the sections, one thing has to be said, because it changes what "switch on a survey" would even mean for this brand.

A post-purchase survey needs a purchase. This account does not have one.

Over the last 90 days the Meta account spent $98,276.68 and produced **4,336 leads at a $22.67 cost per lead, with zero purchases**. That is verified from the Phase 0 pull on 2026-09-03, and `running-notes/brand-rules.md` records it as the account behaving correctly rather than failing, because the business is lead generation. A mom answers a few questions and her details go to a partner insurance agency. An agent calls her. Whatever she decides, she decides on that call, with a different company.

So the moment this doc is built to capture, the instant right after someone pays, does not happen anywhere Health For Moms can see. **Inferred**, and I want to be clear about which part is which. Verified: the zero purchase count, the referral model, the empty survey store. Inferred: that the survey is missing because the buying moment sits outside the brand's walls, rather than because nobody got around to installing one.

That matters for what to do about it. If this were a store, the fix is switching on a tool. Here, the brand would have to decide to ask women something at a moment it invents, most likely just after the lead form or a week or two after the handoff. That is a business decision, not a task, and this doc's job is to make the decision legible rather than to file a ticket.

## What the absence costs the persona system, precisely

**This is the top rung of the evidence ladder, and it is gone.** `persona-research-and-creative-strategy-process.md` ranks the evidence strongest first, and post-purchase survey data sits at the top. It calls it the gold standard, because it ties a real buyer to why and when they bought. The doc goes further and says that when the strongest tiers are missing, the honest move is to name the gap and recommend the brand stand up a post-purchase survey rather than round the persona up into false certainty. That recommendation applies to this brand exactly as written.

**Nothing here is anchored to a confirmed buyer.** This is the only source in the whole system that starts from a real transaction and asks the person directly. Every other source struggles to prove the speaker ever bought. `source-pulls/ad-comments.md` says outright that a commenter is not a buyer, and that author_name is null on all 1,322 rows so no comment can even be tied to a person, let alone to one of the 4,336 leads. With this doc empty, **the brain has no record anywhere of a single confirmed Health For Moms customer.**

**The cashmere lesson cannot be run.** The discipline this prompt is built on is that a survey answer is the conscious, presentable account someone gives after the fact, never the subconscious thing that actually moved them, and the job is to capture the claim and hunt for where it parts ways with behavior. Running that hunt needs a stated reason to exist in the first place. There is none. So for this brand there is no place to set what a customer says against what she did, and `source-pulls/customer-reviews.md` records that the review side of the same comparison is empty too.

**Discovery is dark from both directions at once.** Normally this doc reads the "how did you hear about us" answer for persona signal while the attribution work handles the accounting. Here there is no survey answer, and Northbeam is not connected either, so all attribution is Meta-reported single-platform. That means nobody in this build can say how a mom found this brand, in her own words or in a number.

**The persona confidence ceiling stays capped at thin to mixed.** With the top two rungs empty, every persona in this brain rests on rung five, ad comments, plus category signal. No amount of recurrence inside that one brand-controlled corpus promotes a persona to verified. Any downstream doc writing a persona for this brand as settled truth is overstating the evidence.

## Identity signals observed

**Named blank. No responses, so no identities from this surface.**

The prompt asks for the self-conceptions the answers reveal, read especially from free text where a buyer picks her own words. There is no free text, because there are no answers.

The identity picture this build does hold lives in `source-pulls/ad-comments.md`, which logs nine identity signals against the full 1,322-comment corpus. Read them there, with their own marks. What none of them carry, and cannot carry until this surface fills, is the one thing a survey provides: proof that the person speaking actually went through with it.

## Stated reasons, frequency-ranked

**Named blank. No stated reasons exist, because nobody was asked.**

There is no ranking to give, no free text, no forced choice, and no menu.

The absence is sharper here than in most sections, because the brand does have a written account of why moms buy, and it turns out to have nothing behind it. `source-pulls/brand-self-echo-detection.md` ran every phrase in the brand context document's Customer Language section as a substring search against all 1,322 comments. **Every one returned zero hits.** Not one of the four outcome phrases the document lists as how customers talk, among them *"I finally understand my insurance"* and *"My family is covered, no matter what"*, appears anywhere in the only customer language this brand has. The document itself calls those lines "the brand's own articulation" in one place and lists them as customer speech in another.

A survey is exactly the instrument that would settle that. It would either produce those phrases from real buyers or fail to, and either result is worth having. Right now the brand's stated reasons are the brand's own copy, unchecked.

## Stated-versus-revealed divergences

**Named blank, and this is the most expensive absence in the document.**

The prompt calls this the heart of the doc and the gold the persona system exists to find. It needs two halves from the same person: what she says drove it, and what she actually did.

Neither half exists. There is no stated reason, because there is no survey. There is no revealed behavior tied to a named person either, because there are no purchases, no reviews, no repeat orders, and no way to join a comment to a lead.

So the honest statement for the whole build, and it belongs in this section as much as in the review one: **Health For Moms has no source in which a confirmed customer both states a reason and reveals a behavior.** Every stated-versus-revealed divergence anyone proposes for this brand is a hypothesis about a person nobody has met.

I will name one thing the surveys cannot reach but that the synthesis should hold as a hypothesis rather than a finding, since the prompt asks for exactly that where the survey data cannot get there itself. The comment corpus is full of women saying the barrier is trust in what happens next, not the price of a plan. One from 2026-05-17 asks *"How many calls will I get if I try to see how this works?"* and carries 17 likes, which is high for this corpus. A survey would show whether the women who did fill in the form say the same thing, or say something else entirely. Hypothesis only, from a surface that cannot confirm it.

## How buyers found the brand

**Named blank on both sides.**

Nobody was asked, so there is no self-reported discovery answer. And Northbeam is not connected, so there is no multi-touch view either. Everything is Meta-reported.

What can be said is limited and comes from delivery data rather than from any buyer. Meta reports the audience the account actually reaches as **95.2% female, 81.2% aged 25 to 44, 99.5% mobile**, split roughly 60% Facebook and 39% Instagram, verified in the Phase 0 pull. That is who the platform served. It is not who found the brand, and the two are different populations.

`sub-context-docs/reputation-analysis.md` adds a shape worth carrying: a woman looking this brand up does not reach a review site or a comparison page, because none exists. Public search on 2026-09-04 returned the brand's own Facebook page and its own site and essentially nothing else. So discovery for this brand appears to be a single door, the paid feed. That is **inferred** from the absence of any other findable surface rather than from anyone reporting it.

## Behavioral-signal states observed

**Named blank. No responses, so no purchase-moment states.**

This section normally captures the situational state a buyer was in when she paid, held as an overlay on a person rather than as the person herself. The survey is unusually good at it, because the answer is captured within minutes of the decision while the state is still live.

Nothing here. `source-pulls/ad-comments.md` logs the state signal this build does have, drawn from the comment corpus, and it carries the limit that those states belong to people who saw an ad rather than to people known to have acted.

## Survey gaps and brand-self-echo

Every question this doc would want is a gap, because no question exists. Naming the specific ones is still useful, because it is the shortest route from this blank to a survey worth running.

**What the brand has never asked anyone.** Why she looked today rather than last month. Who the coverage is for. What she was using before. What almost stopped her. Where she first heard about it. What happened after the agent called. Whether she ended up enrolling at all.

That last one is worth pausing on. The brand does not currently know, through any surface Parker can reach, how many of the 4,336 women it sent to partner agencies came out the other side with coverage. `running-notes/success-definition.md` records the team's north star as two gates, cost per lead and then lead quality, and states plainly that gate two lives with the partner agencies and Parker cannot see it. The survey blank and that blind spot are the same hole seen from two sides.

**On brand-self-echo, there is a real risk sitting in the future rather than the past.** No survey exists, so no menu answers have been written and nothing has been echoed back yet. But the prompt warns that a fixed menu of reasons the brand wrote will hand the brand its own marketing back dressed as customer truth, and this brand is unusually exposed to that. Its written Customer Language section already contains twelve phrases flagged as its own copy filed under a customer heading, with zero support in 1,322 real comments. If those phrases become the answer options on a future survey, the survey will confirm them, and the brand will have built a machine for agreeing with itself.

So the recommendation is specific: **when a survey is built, the first questions must be open text.** Let her use her own words before offering her any list. Forced choice can come later, once there is real language to build the options from.

## Recurrence and spread

Zero responses read, out of zero available. No window, because there is no data to bound. No free text and no forced choice, because there are no questions. No platform connected and no CSV uploaded.

Two live pulls today, 2026-09-04, through two different tools reaching two different halves of the store, both returning zero against a collection that exists. Prior verification on 2026-09-03 by other agents in this build reached the same result. So the finding has been reproduced on two dates by more than one route.

There is nothing to weigh and no denominator. The denominator is zero.

## Open loops

Three loops. The territories this doc normally hunts in, the divergence between stated reason and behavior and the identity the survey reveals, are genuinely empty rather than unexplored, so I have not manufactured loops to fill them. Per the prompt's rule, "there is no survey" is a missing source and sits in the frontmatter's data limitations rather than becoming a loop.

### Loop 1 — What does a mom say about why she filled in the form, right after she fills it in?

**Observation.** 4,336 women completed a lead form in 90 days, and the brand asked none of them anything afterwards. The thank-you page is the one moment in this entire business where a real person has just taken a real action and is still on the brand's own screen.

**Pull — Gap.** It fired on the size of the number. Thousands of confirmed actions, and not one question asked of any of them.

**Question.** Why does a mom say she filled in the form, in her own words, in the minutes right after she does it?

**Justification.** One open text box on the thank-you page would create the confirmed-speaker tier this brain has none of, and it would do it inside the brand's own funnel without needing anything from the partner agencies. It would move every persona in this brain off a single brand-controlled source.

**Territory.** Personas.

**Routing.** Only the brand can answer. It needs a question added, not a tool call.

### Loop 2 — Where does a mom first hear that a service like this exists?

**Observation.** Discovery is dark from both directions. No survey answer and no Northbeam, so all that is known is which platform served the ad. Meanwhile the category itself seems to have no visible front door: public search on 2026-09-04 surfaced no review site, no comparison page and no third-party profile for this brand.

**Pull — Gap.** It fired when the discovery section came up empty on the self-report side and I checked the attribution side to see if it could cover, and found that dark too.

**Question.** Where does a mom first hear that a service like this exists?

**Justification.** If the answer is a friend, a Facebook group, a search, or only ever a cold ad, that changes where the money should go and what the creative has to do. Right now the brand is guessing.

**Territory.** Product, the buyer journey side.

### Loop 3 — What does a mom say she got out of it, after she has actually been through it?

**Observation.** The brand's written account of customer outcomes lists phrases like *"I finally understand my insurance"* and *"No more worrying every time my kid gets sick."* Those phrases appear **zero times** across all 1,322 comments. There is no survey to check them against either, so the brand's outcome story currently rests on language nobody has been recorded saying.

**Pull — Tension.** Two things cannot both be true as stated. The brand says this is how its customers talk, and the only customer language that exists contains none of it.

**Question.** What does a mom say she actually got out of this, once she has been through the whole thing?

**Justification.** Outcome language is what the creative promises and what the landing page repeats. If the real answer is different from the written one, every claim in the funnel is built on a phrase the brand made up about itself.

**Territory.** Messaging.

## What would fill this doc

**The smallest thing that would work, and it is genuinely small.** One open text question on the lead form's thank-you page. "In your own words, what made you look into this today?" No platform purchase needed, no integration, no survey tool. Export it as a CSV and Parker can read it, since this collection already accepts CSV upload. That single box would create this brand's first confirmed-speaker record.

**The second step, once the first is running.** A short follow-up a week or two after the handoff, asking what happened on the call and whether she ended up covered. That is the closest this business model can get to a real post-purchase moment, and it would answer the lead quality gate the team named as its own north star.

**The thing that would be worth the most.** A route into the partner agencies, so enrolment outcomes come back. That is the confirmed-buyer tier for a referral business, and no survey the brand runs on its own site can substitute for it.

**What will not fill it.** More analysis of the 1,322 ad comments. That corpus is already read in full and re-reading it in another shape does not create a second source or move anything up the evidence ladder.

**One design rule for whoever builds it.** Open text first, menus later. This brand has already written down what it believes its customers say, and none of it survives contact with the real comment corpus. A survey built from those phrases would launder them into evidence.

When any of this lands, re-run this prompt rather than editing the file. Take this version in as context first, so the record of the blank and the dates it was verified carry forward.
