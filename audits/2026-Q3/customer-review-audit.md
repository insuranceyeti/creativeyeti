---
brand: health-for-moms
doc: customer-review-audit
quarter: 2026-Q3
generated_on: 2026-09-04
refresh_by: 2026-10-04
review_sources_read: [none — every review surface this audit is built to mine returned zero. See the verification below]
review_sources_tested_and_empty: [Parker customer review store via search_customer_reviews_sql, unfiltered, run live 2026-09-04. Parker customer review vector store via search_customer_reviews_semantic, topK 50, similarity floor 0.01, run live 2026-09-04. Parker post-purchase survey store via semantic_search_post_purchase_survey in lookup mode, topK 50, run live 2026-09-04]
knowledge_docs_read: [parker-system/creative-strategy-context/expertise-routing.md, parker-system/creative-strategy-context/customer-review-mining-method.md, parker-system/creative-strategy-context/persona-research-and-creative-strategy-process.md, parker-system/creative-strategy-context/hooks.md]
context_docs_read: [running-notes/missing-context.md, running-notes/brand-rules.md, source-pulls/customer-reviews.md, source-pulls/post-purchase-surveys.md, source-pulls/ad-comments.md, source-pulls/reddit.md, sub-context-docs/reputation-analysis.md, audits/2026-09/monthly-hook-audit.md, BUILD-STATUS.md]
total_reviews_processed: 0
date_range: none. There is no first review and no last review, so there is no range
prior_audit: none. This is the first customer review audit for this brand
data_limitations:
  - "Health For Moms has zero customer reviews on every surface Parker can reach. Verified live today, 2026-09-04, by two tools hitting two different stores. The SQL tool returned `totalResults: 0` in 30ms on a completely unfiltered call with no keyword, no sentiment filter, no date bound and no product filter, with the message 'The database does not contain any customer reviews yet for this brand. No reviews have been uploaded or imported. This is not an access issue.' The vector tool returned `count: 0`, `totalReviewsAnalyzed: 0`, `uniqueReviews: 0` and, critically, `collectionExists: true` at topK 50 with the similarity floor dropped to 0.01. The collection is wired up and it is empty."
  - "Post-purchase surveys are zero as well, verified live on the same day. `semantic_search_post_purchase_survey` in lookup mode returned `count: 0`, `uniqueResponses: 0` and `totalResponsesForBrand: 0`, again with `collectionExists: true`. No survey platform is connected and no CSV has been uploaded."
  - "So both surfaces the prompt names as required sources are empty, and they are the top two rungs of the evidence ladder in `persona-research-and-creative-strategy-process.md`. There is no third surface to fall back to that belongs in this audit: no retailer, no marketplace, no app store, and no third-party review profile. `source-pulls/other-reviews.md` covers the third-party check separately and reaches the same result."
  - "This audit deliberately does NOT substitute the brand's 1,322 Facebook ad comments for reviews. `running-notes/missing-context.md` permits that substitution elsewhere in this brain when it is clearly labelled, and `source-pulls/ad-comments.md` performs it properly at full depth. Doing it here would break the thing this document exists to record and would launder a one-source, brand-controlled corpus into a two-source picture the persona synthesis would then over-trust. Where the comment corpus holds the material a section would have carried, this audit points at it by name rather than reprinting it."
  - "The result is that every one of the seven sections is a named blank. Quote counts against the prompt's targets read 0 of 10-20 comment-response candidates, 0 of 20-40 golden nuggets, 0 of 10-20 objection clusters, 0 personas, 0 of 10-20 FAQ patterns and 0 of 10-20 emotional stories. The denominator on every one is zero."
  - "There is no trajectory read, because there is no prior audit and no corpus to have moved. The prompt asks for a picture of change over the quarter. That is not available and will not be until a corpus exists across at least two runs."
  - "There is no `get_current_time` tool on this MCP surface. The 2026-09-04 date comes from the session clock and matches the date stamped on the most recent docs in this build."
  - "`refresh_by` is set 30 days out rather than the 90-day quarterly cadence in `parker-system/system/refresh-cadence.md`. That doc names a meaningful jump in the review corpus as a refresh trigger, and at a corpus of zero the very first review that lands is that jump. Re-checking costs one tool call, so check monthly rather than in a quarter."
---

# Customer review audit — Health For Moms — 2026-Q3

## Executive summary

**Health For Moms has no customer reviews. Not few. None. This audit is the record of that, and the record is the deliverable.**

That is not a note carried forward from an earlier pass. I ran it fresh this morning through two different tools that hit two different stores, and I set the second one up so that almost any vector would clear the bar. The SQL pull was completely unfiltered, no keyword, no sentiment, no dates, no product, and it came back `totalResults: 0` in thirty milliseconds with the message that the database contains no reviews for this brand and that this is not an access issue. The vector pull asked for fifty results at a similarity floor of 0.01, which is close to accepting anything, and came back with `count: 0` and `totalReviewsAnalyzed: 0` against a collection the tool confirms exists. Then I checked the surface this audit is allowed to lean on when reviews are thin, post-purchase surveys, and it returned `totalResponsesForBrand: 0`. Three empty stores, all confirmed live on 2026-09-04.

The team said the same thing themselves in Slack on 2026-09-03, before any of this ran: *"we don't have reviews but you can pull from competitor reviews or health insurance Reddit etc."* So a SQL tool, a vector tool, a survey tool and the people who own the brand all agree.

**There is a structural reason, and it changes what "fix this" means.** This account is lead generation, not ecommerce. The last ninety days produced **4,336 leads at a $22.67 cost per lead and zero purchases**, and `running-notes/brand-rules.md` records that as the account working as designed rather than failing. Verified from the Phase 0 pull on 2026-09-03. The business is a match and consult referral: a mother answers a few questions, her details go to a partner insurance agency, and an agent calls her. So there is no purchase moment, no product in her hands, and no page where a star rating would live. Whatever happens to her next happens on a phone call with a different company. That read is *inferred*. What is *verified* is the zero purchase count, the referral model as the brand describes it, and the three empty stores. What I am inferring is the link between them.

**What the blank costs is precise, and it is the most important thing in this document.** This audit's single job is to produce a database of proof, actual customer quotes in volume, that a creative team mines for hooks, scripts, ad copy and persona work. It produced none. Every downstream doc that would have pulled from here is now pulling from somewhere weaker. `persona-research-and-creative-strategy-process.md` ranks customer evidence strongest first: post-purchase survey data, then first-party reviews, then order data, then retail reviews, then organic comments and community, then, weakest, competitor and category signal. **Health For Moms has nothing above rung five.** No surveys, no reviews, no order data because there are no orders, no retail. What it has is ad comments and category signal. Every persona, every voice-of-customer entry and every script this brain produces currently rests on the second-weakest tier of a six-tier ladder, and it should stay marked that way.

**The most expensive specific loss is the one this audit's section two would have delivered.** The comment-response format is the highest-value format a review corpus feeds, because it turns a real customer sentence into a hook. This brand has a comment-response gap on both sides at once: no reviews to source hooks from, and no comment-response ad ever run in the account despite the format sitting at number seven on its own untested list. Meanwhile it holds **1,322 real Facebook and Instagram comments across 112 ad IDs and 79 ad names, dated 2025-01-08 through 2026-09-03**. Those are not reviews and this audit will not call them reviews. But they are the closest raw material this brand owns, they are read in full in `source-pulls/ad-comments.md`, and the honest statement is that the comment-response section of this audit is empty while the comment-response opportunity is not.

**And one thing sharpens all of it.** `source-pulls/brand-self-echo-detection.md` ran every phrase from the brand context document's Customer Language section against all 1,322 comments and found **not one of them appears**. Every phrase returns zero hits. The section of the brand's own context document that is labelled as the customer speaking has no support anywhere in the only customer-adjacent corpus this brand holds. Reviews are the surface that would normally settle whether that language is real. Without them, it stays unsettled, and any doc downstream that treats those phrases as customer language is treating brand copy as evidence.

Below, each of the prompt's seven sections is a named blank, with what the section would have carried, what the absence costs, and where the nearest real material actually lives.

## Comment-response ad fuel

**Named blank. Zero candidates out of the ten to twenty this section calls for, against a corpus of zero.**

This section exists to find the sentences in a review corpus that would stop a stranger mid-scroll if they appeared on screen as a comment. The bar is specific and worth restating so the next run knows what it is hunting: the candidate has to read like something a real person typed without thinking about it, not like something a happy customer sat down to write. Skeptics, converts, confessions, genuine disbelief, unexpected specificity, anything that opens a gap only the response can close. If it reads like a review, it is not a candidate. If a stranger would read it out loud to whoever is next to them, it is.

There is no corpus, so there are no candidates. I am not going to promote ad comments into this section and let them sit under a review heading, because that is exactly the substitution that would corrupt the confidence ceiling downstream.

**What the absence costs, precisely.** `hooks.md` treats the comment-response hook as one of its top formats, and its whole mechanic is that the hook is written by a customer rather than by a copywriter. This brand cannot currently write one from a customer, because it has no customer it can quote. That is a real constraint on a format the account has already flagged as untested and that has a working in-category example sitting in its own TikTok mining library, covered in `audits/2026-09/monthly-tiktok-mining.md`.

**Where the nearest real material lives, and what it is not.** `source-pulls/ad-comments.md` holds all 1,322 Facebook and Instagram comments, read at full depth, with dates, ad names and like counts attached. Some of them would clearly clear the comment-response bar. Read them there, labelled as ad comments, with their own honest confidence marks. They are not reviews, they sit underneath the brand's own paid creative, and using one as a hook is a different creative and legal decision from using a customer review, because the person who wrote it was reacting to an ad rather than describing an experience with the product.

## Golden nuggets

**Named blank. Zero nuggets out of the twenty to forty this section calls for, against a corpus of zero.**

This is normally the largest section in the audit and the one the creative team actually opens. It collects the reviews where the customer nailed it, the vivid phrase, the comparison the brand would never have drawn, the sensory detail, the confession, the metaphor. `customer-review-mining-method.md` is clear that a positive review is not a golden nugget, that most lift-able language sits buried in the middle of an otherwise unremarkable review, and that metaphor and alliteration are the two highest-priority signals most passes walk past. All of that requires reviews to walk past.

**What the absence costs, precisely.** The three-way hunt that method describes cannot run at all. Not the golden nugget, not the messaging opportunity, not the whole-review concept. And the third of those is the one this brand loses hardest, because a whole-review concept is a single review whose entire arc maps to a producible ad, and it is the highest-leverage artifact review mining produces. This brand has never had one and cannot have one until someone who went through with it writes about it.

**The knock-on effect is already visible in the voice bank.** With no reviews to mine, the brand's voice of customer work has to build from ad comments and category language, and the echo check above says the brand's own stated customer phrases do not appear in that corpus even once. So the language the creative team is writing from is currently either the brand's own copy or a prospect's reaction to an ad. Neither is a customer describing what happened to her.

## Biggest objections

**Named blank on this surface. Zero objection clusters out of the ten to twenty this section calls for, against a review corpus of zero.**

This is the one section where the blank is genuinely misleading if left unqualified, so I want to be exact. **Health For Moms is not short of objections. It is short of objections from customers.** The distinction is the whole point of this section and it is worth spelling out. A review-sourced objection comes from someone who bought and is telling you what nearly stopped her. An ad-comment objection comes from someone who saw an ad and is telling you why she is not going to. They are different evidence about different people at different points, and collapsing them would make this brand look better informed than it is.

The objection material this brain holds is large, live and read in full, and it lives in `source-pulls/ad-comments.md`. The four biggest clusters there run to 42 comments across 15 ads, 55 across 17, 103 across 13 and 160 across 17, and every one of them is marked mixed confidence rather than verified for exactly the reason this audit exists to record: there is no buyer source to check them against.

**What the absence costs, precisely, and this one is sharp.** The brand's own stated objection list, from the brand context document, names five: "Is this legit?", "I don't want to get on a call and be sold to", "I don't have time", "My state probably isn't included", and "I should just wait for open enrollment." *Stated.* The widest objection in the brand's own comment sections is not on that list. A customer review corpus is the normal way a brand discovers that its objection list is out of date, because a reviewer tells you what she worried about before she went ahead. This brand has no such surface, so the gap between what it thinks stops people and what actually does can only be read from prospects who did not go ahead. That is half the picture and it will stay half until a buyer source exists.

## Personas

**Named blank. Zero personas surfaced, because a persona surfaced from reviews requires reviews.**

This section normally names the distinct customer types visible in the corpus, gives each a prose profile, and hangs three to six quoted reviews under each one so the pattern is checkable. Then it cross-references against the brand's existing persona set and flags where the reviews reveal someone the brand has never named. None of that can run.

**What the absence costs, precisely.** This is the section that validates. `customer-review-mining-method.md` puts it plainly in its sequencing: the mining seeds and the customer analysis validates, and a nugget pass is not a substitute for the validation. Health For Moms currently has the seeding step and not the validating step. Its persona signal comes from ad comments, which are read carefully and honestly in `source-pulls/ad-comments.md` and which surface identities the brand's creative was not built for, including the mother who already has insurance and is still broke, the woman whose employer picks her plan for her, and the woman managing a chronic condition. Every one of those is inferred from someone who typed under an ad. Not one is confirmed to have gone through with anything.

**There is a second, quieter cost.** The brand context document names five ICPs: Jen, Danielle, Marissa, Courtney and Nicole. Nothing in this brain has been able to check any of them against a real buyer, because there is no real buyer on file anywhere. Separately, Parker's own TikTok relevancy scoring for this brand references two ICP names, `Megan` and `Kelsey`, that do not appear in the current brand context document at all, which suggests the persona set has already moved once without the tooling following. A review audit is where a drift like that normally gets caught.

## FAQs

**Named blank. Zero FAQ patterns out of the ten to twenty this section calls for, against a review corpus of zero.**

The FAQ section is built from the questions customers keep asking, whether asked outright or implied through confusion and complaint, and the prompt notes it is one of the highest-value sections for retargeting creative because every unanswered FAQ is a comment-response ad waiting to be made. Both halves of that are unavailable here: no questions from customers, and no comment-response format in the account to route them into.

**What the absence costs, and where the questions actually are.** Women are asking this brand questions constantly. They are asking them under the ads, and `source-pulls/ad-comments.md` logs the clusters with counts and dates. What a review-sourced FAQ would add is the question asked *after* the fact by someone who went through with it, which is a different question from the one a prospect asks before. A prospect asks whether she qualifies. A customer asks what happens next, whether the thing she was promised showed up, and whether it was worth it. **This brand has never heard the second kind of question from anyone.**

**One detail from the comment corpus is worth carrying here as a marker rather than as content.** The most useful answer to one of the brand's own recurring eligibility questions was written by another commenter rather than by the brand, telling a stranger she is allowed to decline her employer's coverage and shop for her own. When the audience is answering the audience, the FAQ surface is doing the brand's work without the brand's supervision. A review corpus would not fix that on its own, but it would tell the brand which answers are actually landing.

## Emotional stories

**Named blank. Zero stories out of the ten to twenty this section calls for, against a review corpus of zero.**

This section collects the reviews where a customer goes past the product and shares something real about her life, block-quoted at whatever length the story needs, because a long-form testimonial or a founder-talks-to-customer format is built directly from that raw narrative arc. It is the section a brand-storytelling team opens.

**What the absence costs, precisely, and this is the sharpest single consequence in the whole document.** **Health For Moms cannot run a testimonial ad.** Not because it has chosen not to, but because it has no customer language of its own to build one from, on any surface, at any confidence. And the audience has noticed the substitute. One comment from 2025-07-25 puts the problem better than a strategist would: *"If you are using a fake person for your testimonial, it unintentionally sends a message to people that no real actual person would say this about your service. I think it's always better to have a real person. Especially with something that is famous for being a scam, like health insurance."* That is an ad comment, not a review, and it is quoted here because it is the audience describing the exact cost of this blank back to the brand.

Held against the account, the shape is clear. **72.9% of the last ninety days of spend carries an authority claim**, per `sub-context-docs/reputation-analysis.md`, and the proof the brand leans on is credential rather than customer. That may be the right call for a category this trust-sensitive. What is certain is that it is currently the only call available, because the other kind of proof requires a corpus that does not exist.

## What would fill this audit

Plainly, so the team can act on it rather than read a complaint. `running-notes/missing-context.md` already carries these as open questions; this is the review-specific version.

**The fastest thing that would work.** Ask something after the handoff. One or two questions sent to a woman a week or two after her lead goes to a partner agency, asking what happened and whether it helped. That is not a product review and calling it one would be wrong. It would be the first record in this brand's history of a real person describing what she went through, and it would start the corpus that this audit and `source-pulls/post-purchase-surveys.md` are both waiting on. It is also the cheapest of the three by a wide margin.

**The thing that would be worth more.** A route into the partner agencies. Call notes, enrolment outcomes, or a standing monthly conversation with a few agents about who is actually signing up. That is the confirmed-buyer tier, and for this business model it is the only version of it that exists.

**What will not fill it.** More ad comment analysis. The 1,322-comment corpus is already read at 100%, and reading it again in a different shape does not create a second source. Every further pass adds detail to a picture that stays capped at one brand-controlled surface, and the persona confidence ceiling stays where it is no matter how many passes run.

**When any of that lands, re-run this prompt rather than editing this file.** Take this version in as context first, so the record of the blank and the dates it was verified survive into the next audit. The trajectory this doc could not produce this quarter starts the moment there are two runs to compare.

## Open loops

Three. Several of the territories this audit normally hunts in are genuinely empty here rather than unexplored, so I have not manufactured loops to fill them. The empty stores themselves are a missing source and sit in the frontmatter's data limitations rather than here, per the rubric. The loops that belong to the *source pull* rather than the audit, who the partner agencies actually enrol and where a mom talks after she fills in the form, are already open in `source-pulls/customer-reviews.md` and are not restated.

### Loop 1 — What does a woman in this category say after the outcome that she never says before it?

**Observation.** Every voice this brand can reach is speaking before anything has happened to her. The 1,322 ad comments are reactions to an ad. The TikTok library is strangers talking about the category. There is no surface anywhere in this brain where someone describes an outcome she actually got from this brand, and a review is the normal place that voice lives.

**Pull — Gap.** It fired when I finished checking three empty stores and realised the brand does not merely lack reviews, it lacks the entire class of speech that comes after a decision.

**Question.** What does a woman in this category say once the thing has actually happened to her?

**Justification.** Everything this brain writes is currently built on anticipation rather than experience, and those two registers do not sound alike. If the after-voice is different in tone, vocabulary or subject, then every script written from the before-voice is speaking a language the brand's actual customers do not use.

**Territory.** Messaging.

### Loop 2 — How much of this account's performance actually depends on the customer's own words?

**Observation.** This brand has never had a line of customer language in a single ad, and its ads work anyway. The account's cheapest lead, at a **$13.29 CPL**, comes from a staged conversation between a wife and her husband that a copywriter invented. Verified from `audits/2026-09/monthly-hook-audit.md`. Meanwhile the standard method treats the customer's own words as the single most valuable input into creative.

**Pull — Tension.** It fired when I set the value this audit is supposed to produce against the account's actual results, and the two could not both be as important as they are each described.

**Question.** How much of what makes an ad work in this account comes from language a real customer used?

**Justification.** The answer sets the price of the blank this document records. If it is low, the missing review corpus is a smaller constraint than the whole build currently assumes and the team should stop treating it as the bottleneck. If it is high, then this is the most expensive gap in the brand and it should outrank everything else on the list.

**Territory.** Messaging.

### Loop 3 — Where did the brand's five customer types come from?

**Observation.** The brand context document names five ICPs, Jen, Danielle, Marissa, Courtney and Nicole, described in detail down to ages and life circumstances. Nothing in this brain has ever been able to check one of them against a person who bought, because no such person is on file anywhere. Separately, Parker's own relevancy scoring for this brand's TikTok library references two other ICP names, `Megan` and `Kelsey`, that do not appear in the current brand context document at all.

**Pull — Curiosity.** It fired when the personas section came back empty and I went looking for what the existing five rest on, and found two different persona sets living in the same brain.

**Question.** Where did the brand's five stated customer types come from?

**Justification.** This audit is the surface that normally validates or corrects a persona set, and it cannot. If those five were observed from real buyers somewhere outside Parker, that source is the missing evidence tier and should be connected. If they were written rather than observed, then every doc downstream is building on a description rather than a finding, and the whole persona spine needs re-grounding.

**Territory.** Personas. **Routed to the brand.** Only the team knows where those profiles came from.

## Appendix - Parker media links

This audit read no reviews, so it holds no review artefacts. Four brand ads and one comment are referenced in the body and are indexed here so a strategist can reopen them.

**M001** — Brand ad `moms-63 2b`, ad 120247093361410519. The POV husband hook, the account's cheapest lead at a $13.29 CPL. Dashboard: `https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093361410519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — Video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399.mp4` — Discussed in: Open loop 2.

**M002** — Brand ad `B1 samar- Copy`. The ad carrying the 2025-07-25 comment about fake testimonials quoted in the emotional stories section. No dashboard link or media file for this ad was pulled in this run, and I am not inventing one. The comment itself is held with its ad name, date and full text in `source-pulls/ad-comments.md`.

**M003** — The full Facebook and Instagram ad comment corpus, 1,322 comments across 112 ad IDs and 79 ad names, dated 2025-01-08 through 2026-09-03, reachable through Parker MCP `search_facebook_ad_comments_sql` and `search_facebook_ad_comments_semantic` on brand `aed0ff06-555d-4f4f-9bf8-31178e2fb977`. Read in full at `source-pulls/ad-comments.md`. Referenced throughout as the nearest real material, and explicitly not used as review evidence in this audit.

**M004** — The Parker customer review store for this brand, `search_customer_reviews_sql` and `search_customer_reviews_semantic` on brand `aed0ff06-555d-4f4f-9bf8-31178e2fb977`. Returned zero rows against an existing collection on 2026-09-04. This is the artefact this audit is a record of.

**M005** — The Parker post-purchase survey store for this brand, `semantic_search_post_purchase_survey` on brand `aed0ff06-555d-4f4f-9bf8-31178e2fb977`. Returned `totalResponsesForBrand: 0` against an existing collection on 2026-09-04.
