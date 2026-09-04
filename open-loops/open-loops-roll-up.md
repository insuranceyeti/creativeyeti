---
brand: health-for-moms
brand_id: aed0ff06-555d-4f4f-9bf8-31178e2fb977
doc: consolidated-open-loops
generated_on: 2026-09-04
refresh_by: 2026-10-04
version: 1
supersedes: "None. This is the brand's first consolidated roll-up. `open-loops/promoted/` and `open-loops/archived/` were empty at the time of this pass, as were `hypotheses/`, `validations/` and `re-validations/`, so no loop in this document was deduped against a prior verdict and nothing here revives an archive."
assembly_mode: "Vault synthesis, assembled 2026-09-04 with no live verification pull. The Parker MCP was disconnected and awaiting re-authorization, so no tool call was made in this pass and nothing here was re-checked against the account, the comment corpus, the mining library or the web today. This node is consolidation rather than fresh research, so it is workable without a pull — but every number below is carried from the document that raised it and carries that document's as-of date, never today's. Where two docs report the same figure on different denominators, both are labelled."
corpus_denominator: "The Facebook and Instagram ad comment corpus is 1,342 as of 2026-09-04. Docs generated 2026-09-03 ran on 1,322 and keep that denominator wherever their counts are carried here. Both are labelled at every use, per the convention set in `sub-context-docs/brand-profile-narrative.md`."
accounting:
  collected: 212
  closed_on_evidence_already_in_the_vault: 5
  killed_on_the_verdict_template: 13
  consolidated_into_survivors: 137
  shipped: 57
  tier_1: 14
  tier_2: 24
  brand_routed: 19
sources_read:
  sub_context_docs: "All 13 with open-loops tails — ad-account-evaluation, brand-identity-analysis, category-and-market-research, community-and-forums, competitive-landscape, customer-journey-and-persona-discovery, marketing-calendar-and-campaigns, operations-and-team, organic-channels-inventory, performance-targets-and-metrics, reputation-analysis, visual-vocabulary, website-and-product-audit. Generated 2026-09-03 and 2026-09-04."
  personas: "personas-profile, persona-voice-library, lifecycle-journey-maps, cross-persona-bias-notes, all 2026-09-04, plus voice-of-customer and its ten extraction nodes (voc-corpus-profile 2026-09-03; the other nine 2026-09-04)."
  source_pulls: "All 8 — ad-account, ad-comments, brand-reputation, brand-self-echo-detection, customer-reviews, other-reviews, post-purchase-surveys, reddit. Generated 2026-09-03 and 2026-09-04."
  audits: "audits/2026-Q3 — 90-day-creative-strategy-audit, 90-day-performance-audit, 90-day-diversity-audit, customer-review-audit, quarterly-whitespace-analysis. audits/2026-09 — weekly-performance-snapshot, biweekly-iterations-report, monthly-hook-audit, monthly-performance-report, monthly-organic-tiktok-audit, monthly-tiktok-mining."
  running_notes: "success-definition.md and brand-rules.md, both 2026-09-03. The two-gate winner definition in success-definition.md is the standard every score below was weighed against."
  method_docs: "parker-system/creative-strategy-context/ — expertise-routing.md, creative-strategy-fundamentals.md (the open-loops reasoning layer), persona-research-and-creative-strategy-process.md, killer-performance-ads.md, ad-account-analysis.md, seasonality.md, advertising-to-older-audiences.md, andromeda-v2.md. parker-system/system/open-loops-system.md for the pipeline architecture and refresh-cadence.md for the stamp. Of these, seasonality, advertising-to-older-audiences and andromeda-v2 carry required sign-off lines and are stamped at the foot of this document. The others carry none."
data_limitations:
  - "No live pull. The Parker MCP was disconnected and needed re-authorization, so this roll-up was assembled entirely from documents on disk on 2026-09-04. No figure was verified today. Every loop carries the as-of date of the document that raised it."
  - "No past-conversation pull. `search_chat_history` could not run for the same reason. Four Parker threads exist (one web, three Slack) and several upstream docs already mined them; what those docs carried forward is used here as stated brand input, attributed to them, and no thread was read fresh."
  - "`sub-context-docs/brand-profile-narrative.md` — the Novelty-check source named in the prompt's required sources — landed at 18:52 on 2026-09-04, part-way through this pass, and carries no open-loops tail yet. Its opening read was used for the Novelty check and it corroborates every Tier 1 finding below, but it was not harvested for loops. Re-check it on the next roll-up. This is a reading flag."
  - "The competitor branch is deferred, so no competitor profile, no external audit cut and no rival library fed this pass. Two territories in `competitive-landscape.md` — Personas and Creators and talent — were left empty upstream for that reason, not because they are clean."
  - "No human strategist has reviewed the upstream audit stack. Eighteen fidelity reviews were still in flight when this ran, per the build ledger, archived at `prompts-run-log/BUILD-STATUS-final-2026-09-04.md`. Two cross-document errors have already reached documents through that gap and both are recorded as closures below."
team: creative-strategy
scope: org-wide
---

# Consolidated open loops

This is the first consolidated roll-up for Health For Moms, and it is the last node of Phase 1. Forty-seven documents were built during this cold start and every one of them ends in an open-loops tail. Those tails held **212 loops**. That is the raw, unfiltered set, exactly as intended — generation was told to capture everything with a real pull and a real justification, and the cut lives here.

Running the verdict template on all 212 killed 13, closed 5 on evidence already sitting in the vault, and folded 137 into the questions they were really asking. **Fifty-seven loops survive.** Fourteen are promoted. Twenty-four sit in backlog. Nineteen can only be answered by the brand.

A word on the size of the promoted set. A steady-state monthly pass should promote a handful. Fourteen is high, and it is high for an honest reason rather than a soft cut: this is a twenty-one-month-old account that has never had a roll-up, so the agenda below is the accumulated question backlog of the brand's entire history arriving at once, not one month's worth. The Tier 1 list is ranked, and the top five are what Parker runs first.

Two things shape almost everything on this list, and they are worth saying plainly before the loops start.

**The brand's own bar has two gates and Parker can only see one.** `running-notes/success-definition.md` records the team's north star verbatim: *"CPL is important to scale but then we look at the lead quality as well before really scaling."* Gate one is cost per lead, visible on every ad. Gate two is lead quality, which lives with the partner insurance agencies. The account fired **42 `Call` events against 4,336 leads** in the trailing 90 days and the `invitee_meeting_scheduled` conversion returned no data at all [`verified`, `source-pulls/ad-account.md`, 2026-09-03]. So gate two has no data. Ten separate documents arrived at that finding independently. It is the single largest thing in this roll-up and it is brand-routed, because no tool reaches it.

**Every persona signal in this brain rests on one surface the brand controls.** Reviews are verified empty. Post-purchase surveys are verified empty. Reddit was unreachable. No competitor is tracked. That leaves the comment sections under the brand's own paid ads — and `personas/voice-of-customer/voice-of-customer.md` found that 60.1% of those comments sit on a single creative family and 64.0% inside two months. Read against the evidence ladder in `persona-research-and-creative-strategy-process.md`, where post-purchase survey data is the gold standard and organic comments sit second-weakest, this brand is running its whole persona system off the second-weakest tier, sampled from a ten-week window under one ad. `brand-profile-narrative.md` caps every persona at mixed confidence for exactly this reason. Getting an independent read is Tier 1 below, and it gates several other Tier 1 loops.

---

## Tier 1 — what Parker runs next

Fourteen loops, ranked. Each line points into its territory section, where the full four-part loop and its score live.

| # | The question | Score | Territory |
|---|---|---|---|
| 1 | What does this audience believe she has the power to change about her own coverage? | 19/20 | Messaging |
| 2 | Why is nobody else advertising health insurance to mothers? | 18/20 | Product |
| 3 | How do moms outside this brand's comment sections describe high deductibles and being priced out of coverage? | 18/20 | Personas |
| 4 | What does a mother find when she looks this brand up before she hands over her phone number? | 18/20 | Messaging |
| 5 | What decides which new files in this account get delivery in their first week? | 18/20 | Messaging |
| 6 | What does a mother in this category treat as proof that a health insurance offer is real? | 18/20 | Messaging |
| 7 | How much of this account's audience mix is being set by the words and pictures in the creative rather than by the targeting? | 18/20 | Personas |
| 8 | What is it about watching someone find out the real price that makes this many people talk? | 18/20 | Messaging |
| 9 | What would tell this team that its creative got better, if cost per lead cannot? | 17/20 | Messaging |
| 10 | How many of the women this account reaches can actually buy what it sells? | 17/20 | Product |
| 11 | What is the pain this audience recognizes without being shown a price? | 17/20 | Messaging |
| 12 | What is different about the mother who clicks in December compared with the one who clicks in November? | 17/20 | Personas |
| 13 | What is happening between the stop and the form fill that makes a high-distress opener cost so much more per lead? | 17/20 | Messaging |
| 14 | What does this audience believe about a brand that uses a synthetic person to sell insurance? | 17/20 | Creators and talent |

**The sequencing note.** Loops 3 and 6 unlock others. Getting an independent read of how mothers in this category talk (loop 3) is what makes the two Tier 2 loops on the employer-plan mother and on the switching moment answerable at all — both were held at Researchability 3 purely because the language they need does not exist on any surface Parker can currently reach. Run loop 3 early and two backlog items move up behind it.

**The clock.** Open Enrollment starts 2026-11-01, which is 58 days out, and the brand plans creative two months ahead — so the planning deadline was 2026-09-01 and it has already passed. Loops 5, 12 and 13 are the three on this list that change what gets produced in the next four weeks. Everything else can run behind them.

**The parallel track.** Nineteen brand-routed loops sit in their own section below. They are not backlog. They are a single conversation with the team and their partner agencies, and several of them — the lead-quality gate, the two claims running on most of spend, the statics decision — outrank most of this table on stakes. They are routed rather than tiered because Parker cannot answer them, not because they matter less.

---

## Personas — are we advertising to the right people

Fourteen loops. This is the territory the whole roll-up bends toward, which is what `system/open-loops-system.md` predicts: the answer here routes nearly everything downstream, and this brand's persona spine is the thinnest thing it owns.

### 1. Every persona in this brain rests on a surface the brand pays for

**Observation.** One comment out of 1,322, pasted on 2025-01-13 under the ad `IMG 6`, summarizes Reddit discussion as calling Health For Moms *"generally considered not legitimate and likely a scam."* It drew 14 likes and 10 replies, which makes it one of the most engaged records in the corpus, and nothing in it was ever verified. Behind that single fragment sits the structural fact: reviews are verified empty, post-purchase surveys are verified empty, Reddit was unreachable at pull time, no competitor is tracked, and all 1,322 comments sit directly under this brand's own ads. The team named the substitute themselves in Slack on 2026-09-03: *"we don't have reviews but you can pull from competitor reviews or health insurance Reddit etc."*

**Pull — Gap.** It fired on an absence where presence would be expected. The one source that would settle half the verdicts in the echo detection has been named as available by the team and has never been opened.

**Question: How do moms outside this brand's comment sections describe high deductibles and being priced out of coverage?**

**Justification.** It is the only thing that would move any persona in this system above mixed confidence. It also decides whether the account's own creative language is category-standard or genuinely distinctive, which is the difference between a defensible message architecture and a brand reading its own echo back to itself. `source-pulls/brand-self-echo-detection.md` could not settle five verdicts without it.

**Score:** Stakes 5, Confidence 5, Researchability 4, Novelty 4. **Total 18/20. Tier 1.**
Researchability is 4 rather than 5 because Reddit was blocked in this build; the question is answerable through deep research across forums, category communities and public discussion without needing any brand-held data, which is what keeps it out of the brand-routed cohort.

**Consolidates** (9 upstream loops): `cross-persona-bias-notes.md` 1 (2026-09-04) · `source-pulls/brand-self-echo-detection.md` 2 and 3 (2026-09-03) · `source-pulls/reddit.md` 1 and 3 (2026-09-03) · `personas/voice-of-customer/voice-of-customer.md` 3 · `voc-corpus-profile.md` 1 (2026-09-03) · `voc-pain-phrase.md` 2 · `persona-voice-library.md` 4.
**Marks carried:** the Reddit verdict is `stated` and unverified — it is one commenter's paste of a summary, not a read of Reddit. The corpus-concentration counts are `verified`.
**Tags:** team `creative-strategy`, scope org-wide.

### 2. The creative is picking the audience, and nobody planned that

**Observation.** Three ads with no targeting difference between them produced three completely different age distributions. The self-employed static put **54.4%** of its spend on women over 45. The skit family put **40.2%** there. The silent-clinician ad went the other way, **52.7%** to women aged 25 to 34. The account overall sends **21.2%** to women over 45. Read by format rather than by ad, the same split holds: POV puts 43.6% on 25-to-34 and 9.4% on 45-to-54, while Skit does close to the reverse at 11.9% and 34.7%. None of it was a targeting choice. All of it is broad delivery reacting to what the creative says.

**Pull — Surprise.** It fired because the format mix and the copy were never designed as a targeting tool and appear to be acting as one anyway, which is not what the setup would predict.

**Question: How much of this account's audience mix is being set by the words and pictures in the creative rather than by the targeting?**

**Justification.** The brand's own stated testing priority is *"All different ages of moms with ages of kids."* If a sentence is the lever that reaches a forty-eight-year-old, then the persona-allocation problem and the creative-brief problem are the same problem, and the fix is a line of copy rather than an ad set. It also reframes the whole served-audience read: what the account is doing is casting an audience, not targeting one.

**Score:** Stakes 4, Confidence 5, Researchability 5, Novelty 4. **Total 18/20. Tier 1.**
Researchability is 5 because this closes entirely inside the ad account — creative-derived format tags against per-ad demographic delivery, spend-weighted per the cohort rule in `creative-strategy-fundamentals.md`. It is the cheapest Tier 1 on this list.

**Consolidates** (4 upstream loops): `quarterly-whitespace-analysis.md` 3 (2026-09-04) · `sub-context-docs/ad-account-evaluation.md` 4 (2026-09-04) · `90-day-diversity-audit.md` 4 (2026-09-03) · `90-day-performance-audit.md` 1 (2026-09-03).
**Marks carried:** all four delivery splits `verified` from per-ad breakdowns.
**Tags:** team `creative-strategy`, scope org-wide.

### 3. December turns against this brand and November does not

**Observation.** November 2025 held cost per lead almost flat at **$13.08**, up 6.6% from $12.27, while CPM rose 31.6% — because CTR rose 41.3% and paid for it. It was the year's biggest lead month. December then broke the trade: the most expensive impressions of all thirteen readable months at **$29.34** CPM, cost per lead up 39.8% to **$18.28**, and the share of landing page views becoming leads falling from 18.7% in October to 14.2% in December, on largely the same creative and the same funnel. Separately, nine of the 19 relevant videos in the category mining library, 47.4%, were posted between October 1 and December 31 across three different years.

**Pull — Surprise.** It fired because everyone in this brain, the brand included, has been treating Open Enrollment as one window with one answer, and the account says the two halves of it behave in opposite directions on a near-controlled comparison.

**Question: What is different about the mother who clicks in December compared with the one who clicks in November?**

**Justification.** `seasonality.md` says the useful question inside a season is never whether demand spikes but what shifts underneath it — the buyer, the angle, the context — and that the ICP itself can flip inside a window. This brand's own numbers say something about the buyer changes between those two months. The answer decides whether December gets budget, different creative, or neither, and it has to be decided before 2026-11-01.

**Score:** Stakes 4, Confidence 5, Researchability 4, Novelty 4. **Total 17/20. Tier 1.**
Confidence is 5 because the November-to-December comparison is close to controlled: same creative, same funnel, adjacent months.

**Consolidates** (5 upstream loops): `sub-context-docs/marketing-calendar-and-campaigns.md` 2 (2026-09-04) · `performance-targets-and-metrics.md` 3 (2026-09-04) · `monthly-tiktok-mining.md` 2 (2026-09-04) · `customer-journey-and-persona-discovery.md` 4 (2026-09-03) · `category-and-market-research.md` 1 (2026-09-03).
**Marks carried:** all monthly figures `verified` from account pulls; the library's seasonal clustering `verified` on 19 relevant videos.
**Tags:** team `creative-strategy`, scope org-wide.

### 4. The brand's written record of its customer may be the brand talking to itself

**Observation.** The brand context document names five ICPs — Jen, Danielle, Marissa, Courtney and Nicole — described down to ages and life circumstances. At least one of them, Jen, matches Parker's own Slack message character for character at offset 4268, written on 2026-09-03 and then adopted into the canonical list. Every phrase in the document's Customer Language section returns zero hits across 1,342 comments, including *"We are super middle class — how are we stuck with everything?"* and *"They don't give a rat's butt about people like me."* The stated objection list names *"I should just wait for open enrollment"* as one of five main objections; the phrase "open enrollment" appears in **1 of 1,322** records and "enrollment" in any form in 2, while the pregnancy exclusion, which is on no stated list, appears in 42 across 15 ads. Separately, Parker's own relevancy scoring for this brand's TikTok library references two other ICP names, `Megan` and `Kelsey`, that do not appear in the current context document at all.

**Pull — Tension.** It fired because the same document calls these lines the brand's own emotional outcomes in one section and how customers describe outcomes in another, and both cannot be true as written.

**Question: What in the brand's written record of its customer came from a real customer?**

**Justification.** This one question covers the ICPs, the customer-language phrases, the outcome phrases and the objection list, because they all live in the same document and share the same provenance problem. The answer flips the value of the whole thing. If those lines came from real mothers on sales calls or in a research session, they are the best customer evidence this brand owns and every persona should be rebuilt with them. If a copywriter wrote them, the section is the brand talking to itself, and every writer who trusts it ships the brand's marketing back at the customer as her own voice. This is the loop the task brief points at when it says unsourced customer language is moving into landing-page copy.

**Score:** Stakes 5, Confidence 5, Researchability 1, Novelty 4. **Brand-routed** — Stakes 4 or higher with Researchability 2 or lower overrides the total of 15.
**The clarifying question for the team:** where did the five customer profiles, the Customer Language section, and the five stated objections in the brand context document come from — a research session, agent call notes, the partner agencies, or were they written?

**Consolidates** (9 upstream loops): `customer-review-audit.md` 3 (2026-09-04) · `cross-persona-bias-notes.md` 2 · `personas-profile.md` 3 · `brand-identity-analysis.md` 3 (2026-09-03) · `source-pulls/brand-self-echo-detection.md` 3 (2026-09-03) · `post-purchase-surveys.md` 3 (2026-09-04) · `voc-objection.md` 2 · `voc-corpus-profile.md` 4 (2026-09-03) · `voc-aspirational.md` 2.
**Marks carried:** the zero-hit counts are `verified`; the Jen match is `verified` against the Slack thread; the provenance of the other four ICPs is unknown, not inferred.
**Tags:** team `creative-strategy`, scope org-wide.

### 5. The only confirmed-buyer record this brand has is one nobody in this brain has read

**Observation.** The brand hands every lead to a partner insurance agency, and those agents have real conversations with these women, sometimes for hours. 39,569 leads lifetime at $18.78 each, 4,336 in the trailing 90 days at $22.67. There is a body of confirmed conversations with real people and no document in this brain has ever read one.

**Pull — Gap.** It fired when the review store came back empty and the search moved to where a confirmed customer might exist for this brand at all. The agencies are the only place one does.

**Question: Who do the partner agencies say is actually calling back and enrolling?**

**Justification.** Read against the evidence ladder in `persona-research-and-creative-strategy-process.md`, the agencies hold the top rung this brand is missing — a real buyer tied to a real reason. It would replace both missing tiers at once. If who enrols differs from who comments, every persona in this brain moves, and the served-audience read and the actual-buyer read finally have something to be compared against.

**Score:** Stakes 5, Confidence 5, Researchability 1, Novelty 4. **Brand-routed** — override.
**The clarifying question for the team:** can someone at the partner agencies describe the women who actually enrol — their age, their situation, and what they said on the call?

**Consolidates** (2 upstream loops): `source-pulls/customer-reviews.md` 1 (2026-09-04) · `personas-profile.md` 2 (partial — its ranking half sits with the Product gate-two loop).
**Tags:** team `creative-strategy`, scope org-wide.

### 6. The creative draws no line anywhere on money, so both the wrong moms and the right ones raise their hands

**Observation.** The creative never names a price. **202 of 1,322** records, 15.3%, contain a dollar figure, and in every one read the money is the plan she already has — there is no record anywhere objecting to what Health For Moms costs. Seven comments ask "how much," including *"How much is the monthly I can afford a lot"* on 2026-07-04, a buying signal with nowhere to go. At the other end, on 2026-04-09: *"So because I make under $30,000 and am under 63.. no othe questions that fit as to why I can't get coverage.. I'm a single mom not making enough to afford insurance so who's this plan for if not moms like me?"* Four records across four ads name an income floor, two of them naming $30,000 independently. Meanwhile the team said in Slack on 2026-09-03 that single moms are fine *"just as long as we also use lingo about them not being broke."*

**Pull — Tension.** The team's own rule says this buyer is not broke, the ads carry no signal at all about money, and both cannot be a fair description of who the account is inviting.

**Question: How much money does a mom need to have for this offer to actually work for her?**

**Justification.** It is the line between a lead that becomes a customer and a lead that wastes an agent's afternoon, and right now the creative draws no line anywhere. Knowing the floor changes who the ads invite and how the money trigger is written, and part of the answer sits in the brand's own closed-lead data.

**Score:** Stakes 4, Confidence 4, Researchability 2, Novelty 4. **Brand-routed** — override.
**The clarifying question for the team:** is there an income floor on the qualifier, and what does a typical monthly premium actually land at?

**Consolidates** (3 upstream loops): `customer-journey-and-persona-discovery.md` 5 (2026-09-03) · `voc-objection.md` 4 and 5 (2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

### 7. The older woman the grievance creative keeps reaching, and nobody has written her a message

**Observation.** Ads that open on a distressed face and a complaint screenshot deliver **30% to 38%** of their spend to women 45 and over. Ads that open on a warm aspirational montage deliver **7% to 12%** there. Same offer, same state list, same product. She also watches three to five times longer, with hold rates of 7.6% to 17.1% against 2.4% to 4.3%, and the denial skit holds **24.48%** against the top spender's **3.28%**. The format cut reproduces it: Skit sends 31.5% of its lifetime spend to women 45 and over against POV's 10.6%. No ad in the library was built for her on purpose, and the one that speaks to her age directly got **$34.21** before it was paused. Across the 19 relevant videos in the category mining library, exactly one creator reads as over 40 and none over 45.

**Pull — Pattern.** The same split appeared independently through two different instruments — nine per-ad delivery breakdowns and a separate format-tag pull — which turned a curiosity about one ad into a question about the whole account.

**Question: What is the woman over 45 that the grievance creative keeps reaching actually coming to this offer for?**

**Justification.** She is roughly a fifth of the spend and the most attentive audience the account has. `advertising-to-older-audiences.md` says this group tolerates more narrative rather than less, converts from further up the funnel, and trusts an authority frame over a peer — all three of which describe creative this account has never made. If her situation differs from the young partnered mother's, and the watch time suggests it does, she needs her own message rather than a harder version of the same one.

**Score:** Stakes 4, Confidence 5, Researchability 3, Novelty 4. **Total 16/20. Tier 2.**
Researchability is 3 and it is the honest constraint: she barely comments. `cross-persona-bias-notes.md` counts roughly 16 comments from her against 30% to 38% of grievance-ad spend, so the instrument this brain listens with cannot see her. Answering her properly depends on the independent language read in Tier 1 loop 3. **This is the first Tier 2 loop to activate when a Tier 1 resolves.**

**Consolidates** (8 upstream loops): `source-pulls/ad-account.md` 2 (2026-09-03) · `personas-profile.md` 1 · `cross-persona-bias-notes.md` 3 · `lifecycle-journey-maps.md` 5 · `persona-voice-library.md` 5 · `monthly-hook-audit.md` 4 (2026-09-03) · `monthly-organic-tiktok-audit.md` 3 (2026-09-04) · `90-day-diversity-audit.md` 4 (partial).
**Tags:** team `creative-strategy`, scope org-wide.

### 8. The audience knows more about insurance than the creative assumes

**Observation.** **103 comments across 13 ads** say the ad describes an out-of-pocket maximum, not a deductible, and self-identified brokers, agents and medical billers are among them. This sits on the account's highest-spend creative. Beyond the correction, commenters trade real technical terms with each other unprompted: out of pocket at 74 records, pre-existing condition at 33, coinsurance at 30 across three spellings, Obamacare at 15, marketplace at 14, plus guaranteed issue, medical underwriting, level-funded plans and allowed amount. The brand's ten highest-spending ads use four terms total. Row `052aa855` names deductible, out-of-pocket maximum, coinsurance, the 80/20 split, high-deductible health plans, HSA cards and premiums correctly and in order, in a single unprompted comment.

**Pull — Surprise.** Given creative built on explaining a confusing number, the volume of people who already understand the number better than the script does is not what the setup would predict.

**Question: How much does the woman this brand targets already know about health insurance before an ad reaches her?**

**Justification.** It decides the register of every ad. Talking down to a fluent audience reads as either misleading or amateur, and both cost credibility on the account's highest-spend creative. Talking up to a confused one loses her entirely. `creative-strategy-fundamentals.md` draws the distinction that matters here: a misconception to overturn is a different creative move than a value barrier to reframe, and right now nobody knows which one this account is running.

**Score:** Stakes 4, Confidence 5, Researchability 4, Novelty 3. **Total 16/20. Tier 2.**
Novelty is 3 because three separate docs already reached a partial answer — the corpus itself says the audience is more fluent than the script. What is genuinely open is the size and the split, not the direction.

**Consolidates** (4 upstream loops): `source-pulls/ad-comments.md` 3 (2026-09-03) · `source-pulls/reddit.md` 4 (2026-09-03) · `voc-category-jargon.md` 1 (2026-09-04) · `voc-objection.md` 6.
**Tags:** team `creative-strategy`, scope org-wide.

### 9. The mother on an employer plan, and why she has never looked

**Observation.** `moms-63 3e` is the only ad in the top ten that opens by voicing the objection *"I already have health insurance, this doesn't apply to me,"* and it produced the second-best cost per lead in the group at **$15.14** on the cheapest CPM at $18.60. The account has run this objection once, at **4.7% of spend**. The same belief shows up unprompted in the comments: *"I already have a $0 deductible and have free insurance from my job! I'm covered!"* and *"But how? If your job offers insurance you have to pick an insurance. They make you pay for one."* Twenty-four comments mention an employer, and this family is the most durable in the corpus, running from March through August while everything else went quiet after May. One woman had to be told by a stranger that declining employer coverage is allowed.

**Pull — Pattern.** It fired when the same sentence turned up as a winning script's opening line and as a viewer's rebuttal in the comments on a different ad, within the same ninety days.

**Question: How do mothers on employer plans describe the reason they have never looked at anything else?**

**Justification.** This is the largest audience the brand is not speaking to, and the brand's own competitive read names employer coverage as its most common alternative. If Parker knew the actual belief holding these women in place — the tax credit, the payroll deduction, the assumption that employer plans are cheaper, or simply never having been given a reason to look — the messaging lane would be obvious and the top of the funnel would open. Right now the account has one accidental data point and no understanding underneath it.

**Score:** Stakes 4, Confidence 5, Researchability 3, Novelty 4. **Total 16/20. Tier 2.**
Researchability is 3 for the same reason as loop 7: this language does not live on any surface Parker can currently reach. It moves to 4 the moment Tier 1 loop 3 resolves.

**Consolidates** (4 upstream loops): `90-day-creative-strategy-audit.md` 3 (2026-09-03) · `voc-pain-phrase.md` 4 (2026-09-04) · `source-pulls/ad-comments.md` 2 (2026-09-03) · `voc-pain-phrase.md` 3.
**Tags:** team `creative-strategy`, scope org-wide.

### 10. The moment she decides to look

**Observation.** The transcripts of the ten highest-spend ads, carrying **$743,218.09** of lifetime spend between the account's 1,558 ads, all open on a standing condition, a category argument, or a statistic. Not one opens on an event. Meanwhile the comment threads under those same ads hold a hysterectomy diagnosis, a surgery scheduled for tomorrow, a father's death, a birth a month away, and a child's ear operation blocked by a $1,500 deposit. And the classic switching triggers leave no trace at all: "laid off" returns 0 of 1,342, "cobra" 0, "divorce" 0, "turning 26" 0, "open enrollment" 1. Three separate women describe work and coverage changing hands at the same moment — one lost free insurance when she went back to work, one had a rehire open a window she is unsure about, one is job hunting specifically to get better insurance.

**Pull — Gap.** There is a pile of dated, specific, first-person moments sitting in the brand's own comment sections, and three quarters of a million dollars of creative has never used one.

**Question: What is the moment a mother decides to look for different coverage?**

**Justification.** `persona-research-and-creative-strategy-process.md` defines a persona as a trigger-anchored identity — who she is plus the situation that activates her — and says to name personas by the trigger rather than the demographic bucket. This account has no trigger read at all. Its personas are demographic buckets. The answer would give the persona set its missing spine and it would give the creative something a viewer cannot counter-bid, which is the failure mode the pain pass already found.

**Score:** Stakes 4, Confidence 4, Researchability 3, Novelty 5. **Total 16/20. Tier 2.**
Novelty is 5: in $743,218.09 of lifetime creative, the account has never once opened on an event. Researchability is 3 because the standard triggers leave no trace in the only corpus available, which again points at Tier 1 loop 3 first.

**Consolidates** (4 upstream loops): `voc-trigger-moment.md` 1, 2, 3 and 4 (all 2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

### 11. The word the whole brand is built on may be reading as a rule rather than an identity

**Observation.** "Insurance" appears in **284 of 1,322** records, 21.5%. "Mom" appears in at most **73**, 5.5%, and that figure is inflated because the string also matches "moment." Sixteen comments across 7 ads ask whether grown children still count; 16 across 12 ask about dads, husbands and sons. Most are sincere eligibility questions, not complaints, and nobody answers on the thread. Meanwhile "wife of the year energy," the phrase carrying roughly two thirds of recent spend, appears **0 times in 1,342 comments**, re-verified live on 2026-09-04.

**Pull — Surprise.** For a brand named Health For Moms whose entire creative device is that one word, the audience using the category word nearly four times as often is not what the setup would predict.

**Question: How does this audience describe who she is when she talks about buying health insurance?**

**Justification.** It decides whether "mom" is the identity the creative should lead with or a wrapper quietly generating eligibility confusion, and that routes the naming, the casting and the callout line in every brief downstream. `advertising-to-older-audiences.md` is blunt that a direct identity callout is what pulls relevance and that subtlety underperforms — but only if the callout names an identity the viewer actually holds.

**Score:** Stakes 3, Confidence 5, Researchability 4, Novelty 4. **Total 16/20. Tier 2.**
Stakes is 3, not 4, and that is the honest read: the answer changes the naming, the callout and the casting brief, which is a framing decision rather than a change of road.

**Consolidates** (4 upstream loops): `personas-profile.md` 4 (2026-09-04) · `voc-corpus-profile.md` 3 (2026-09-03) · `source-pulls/ad-comments.md` 7 (2026-09-03) · `voc-aspirational.md` 3.
**Tags:** team `creative-strategy`, scope org-wide.

### 12. The state list is being shown to moms in states that are not on it

**Observation.** On 2026-09-02 a commenter asked, under the approved-state-list ad, *"Why is this being shown in IL if it's not on the list???😭🤦🏼‍♀️"*. Two more in the same seven days name Georgia and Texas: *"Ofc Georgia ain't on there 🤣"* and *"What a joke!! They don't have quote for me In tx."* The Approved State List runs to 32 to 34 states across all thirteen ads read at full media depth, and it sits behind roughly **92.7%** of the 90-day spend.

**Pull — Pattern.** Three separate commenters in seven days say the ad reached them somewhere it cannot serve them.

**Question: How much of this account's spend lands on moms in states the product cannot sell into?**

**Justification.** If the share is meaningful, the cheapest efficiency gain available before Open Enrollment is a geo exclusion rather than a creative change, and the brand's stated objective is efficiency before volume.

**Score:** Stakes 3, Confidence 5, Researchability 5, Novelty 3. **Total 16/20. Tier 2.**
Researchability is 5 — regional delivery against the approved list is one pull. Stakes is 3 because it is an efficiency fix rather than a strategic fork, which is what holds it out of Tier 1 despite being the single cheapest thing on this whole list to answer. Texas and Georgia are two of the largest uninsured states in the country, so the number may be large.

**Consolidates** (3 upstream loops): `weekly-performance-snapshot.md` 3 (2026-09-04) · `monthly-performance-report.md` 4 (2026-09-03) · `source-pulls/brand-reputation.md` 2 (partial).
**Tags:** team `creative-strategy`, scope org-wide.

### 13. The woman doing this math before she has children

**Observation.** The highest-conversation video in the whole category mining library, at a **1.79% comment rate and 557 replies from 31,200 views**, belongs to a creator whose own hashtags are `childlessmillennial` and `dink`. She has no children and is working out whether she can afford to. The brand's five stated ICPs all already have kids, and the library was scraped on mom-and-insurance keywords, so she arrived unbidden. Separately, 16 comments across 7 ads in the brand's own corpus come from women whose children are grown or who have none.

**Pull — Surprise.** It fired when the row's hashtags were read after the transcript, having assumed from the video that she was a mother like everyone else in the pool.

**Question: Who is the woman running these numbers before she has a child?**

**Justification.** She showed up unbidden in a mom-keyword scrape and out-talked every mother in it. If that audience is reachable and near the brand's product, she is a buyer nobody in the category speaks to. If she is not, the brand should know that the loudest voice in its category belongs to someone it cannot sell to.

**Score:** Stakes 3, Confidence 4, Researchability 4, Novelty 5. **Total 16/20. Tier 2.**

**Consolidates** (1 upstream loop): `monthly-tiktok-mining.md` 3 (2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

### 14. Men keep showing up, month after month

**Observation.** Male-attributed spend rose in every single month of the last six, from **1.9% in March to 4.6% in August**, while female share fell from 97.5% to 94.8% across the same run. Sixteen comments across 12 ads ask about dads, husbands and sons.

**Pull — Pattern.** One month would be noise. Six consecutive months moving the same way across independent monthly pulls is something accumulating.

**Question: Who are the men this account is reaching?**

**Justification.** Health insurance is bought for a household. If dads are quietly becoming a real slice of the funnel, that is either a second buyer worth speaking to or wasted delivery worth excluding, and those call for opposite actions.

**Score:** Stakes 2, Confidence 4, Researchability 4, Novelty 4. **Total 14/20. Tier 2.**
Stakes is 2 and that is the honest cut: 4.6% of spend on a rising line is real, but the net business outcome riding on it is small next to anything else on this list. It stays in backlog rather than the archive because the trend is six months old and still moving.

**Consolidates** (1 upstream loop): `90-day-performance-audit.md` 5 (2026-09-03).
**Tags:** team `creative-strategy`, scope org-wide.

---

## Product — the right product, the right way, the business case

Thirteen loops. This is the territory where the brand-routed cohort concentrates, because almost everything Parker cannot see about this business sits past the lead handoff.

### 1. Nobody else is advertising health insurance to mothers

**Observation.** Parker holds 3,716 brands. The keyword `health insurance` matched **15,335 ads** across them, and the top 15 by impression rank contain senior life insurance, burial coverage, telehealth and supplements — but no health coverage aimed at American mothers. Health For Moms has spent **$743,218.09** in that exact lane since December 2024. Separately, five insurance and finance lead-gen brands checked in the wider library each run large static libraries, from 191 statics at Insurify to 856 at Ethos, so the category is neither small nor quiet. It is just not here.

**Pull — Gap.** An absence sitting where you would expect a crowd, in a category with plenty of money in it.

**Question: Why is nobody else advertising health insurance to mothers?**

**Justification.** `creative-strategy-fundamentals.md` says to interrogate an empty lane before claiming it, because an absence has three very different explanations and each routes a different response: it has been tried and failed, a real constraint blocks it, or it is genuinely open. If carriers or platform rules block it, this brand's position is far more fragile than it looks and the right move is to protect the mechanism it has. If it is genuinely open, the moat is real and worth spending hard against before Open Enrollment. Nothing else on this list changes the aggression of the whole plan the way this does.

**Score:** Stakes 5, Confidence 4, Researchability 4, Novelty 5. **Total 18/20. Tier 1.**
Researchability is 4 and deliberately generous, per the scoring rule: public ad libraries, carrier and platform advertising policy, state insurance advertising rules and the FTC's own enforcement record are all reachable, and the brand's own running creative is itself evidence of what has already survived a compliance loop.

**Consolidates** (2 upstream loops): `competitive-landscape.md` 3 (2026-09-04) · `90-day-diversity-audit.md` 2 (partial — its category-static comparison).
**Marks carried:** the 3,716-brand and 15,335-ad counts are `verified`; the absence is `verified` against impression rank, which `analyzing-public-ad-accounts.md` treats as a proxy rather than spend.
**Tags:** team `creative-strategy`, scope org-wide.

### 2. The account keeps buying attention from people the product turns away

**Observation.** Roughly **108 records across five separate objection clusters** are about being turned away, and no single extraction could see the size of it because each cluster looked moderate alone: maternity at 36, pre-existing conditions at 42, silent rejection at 11, state exclusion at 15 as a floor, and the income floor at 4. That is about **8.2% of 1,322**, and the true distinct count is somewhat lower because maternity and pre-existing share at least two records. Even discounted it is by a wide margin the largest single thing in the voice-of-customer library. The expecting mom is the widest objection in the corpus, 42 comments across 15 ads over fourteen months, and pregnancy is 63.2% of the category's organic feed — twelve of 19 relevant videos, including the three largest by view count. The plans are medically underwritten, so both groups are screened out, and both keep arriving because a broad audience of women 25 to 44 always contains them. The only two records in 1,342 that praise this brand's service both come from women who were told no.

**Pull — Pattern.** The same collision surfaced independently in the comment corpus, the website audit, the reputation read and the category feed, always with the brand's own name used as the setup for the complaint.

**Question: How many of the women this account reaches can actually buy what it sells?**

**Justification.** `creative-strategy-fundamentals.md` says to size the opportunity before asking how to capture it, and nobody has sized this one. At $22.67 per lead across 4,336 leads in ninety days, the difference between a targeting problem and a creative problem is the whole media plan. If a large share of delivery is structurally unqualifiable, the fix is upstream of any script and no hook testing touches it.

**Score:** Stakes 5, Confidence 5, Researchability 3, Novelty 4. **Total 17/20. Tier 1.**
Researchability is 3, not 2, which is what keeps this out of the brand-routed cohort and in the promoted queue. The full screen-out rate needs the partner agencies. But the qualifier itself is a public flow on the brand's own site, medical underwriting rules for private plans are public, and the delivery demographics are in the account — enough to size the answer within a wide band without waiting for anyone. The precise number is brand-routed and is loop 3 below; the size of the problem is not.

**Consolidates** (11 upstream loops): `voice-of-customer.md` 2 · `quarterly-whitespace-analysis.md` 5 (2026-09-04) · `source-pulls/ad-comments.md` 1 and 6 (2026-09-03) · `website-and-product-audit.md` 3 (2026-09-03) · `source-pulls/brand-reputation.md` 2 (2026-09-04) · `lifecycle-journey-maps.md` 2 · `customer-journey-and-persona-discovery.md` 3 (2026-09-03) · `monthly-tiktok-mining.md` 1 · `category-and-market-research.md` 2 (2026-09-03) · `voc-pain-phrase.md` 3.
**Marks carried:** the comment counts are `verified`; the underwriting screen is `inferred` from the comment record and the site, not confirmed by the brand.
**Tags:** team `creative-strategy`, scope org-wide.

### 3. Gate two of the brand's own winner definition has no data

**Observation.** The account produced **4,336 leads in the trailing 90 days** and **39,569 lifetime**. The custom conversion built to track a booked consultation, `invitee_meeting_scheduled`, returned **no data at all** in the window, and only **42 `Call` events** fired. Every cost per lead in this brain is the cost of a phone number, not the cost of a customer. Meanwhile the account's cost per lead did not move across two structurally different quarters — $22.65 to $22.64 — while spend fell 73.5%, the dominant format collapsed, the dominant emotion swapped from anger at 55.2% to pride at 49.5%, and hold rate fell from 11.09% to 3.83%. And the comment section's largest substantive cluster is people finding out they do not qualify *after* clicking.

**Pull — Tension.** The account ranks its creative confidently on cost per lead while the one number that would say whether a cheap lead is a good lead is missing, and those two things cannot both be trusted.

**Question: What happens to a Health For Moms lead after it reaches the partner agency?**

**Justification.** `running-notes/success-definition.md` records the brand's own bar as two gates, and this is gate two. If a meaningful share of leads is disqualified downstream, the metric the whole account steers by has been rewarding creative that produces unqualified clicks, and every creative decision made this quarter was optimised against the wrong signal. It also decides something concrete for November: whether the ads to scale are the ones with the lowest cost per lead or a different set entirely. Nothing else in this roll-up matters as much as this answer.

**Score:** Stakes 5, Confidence 5, Researchability 1, Novelty 5. **Brand-routed** — override. **This is the highest-stakes loop in the document.**
**The clarifying question for the team:** for the August creative against the April creative, what share of leads reached a real conversation, and what share enrolled?

**Consolidates** (10 upstream loops): `90-day-creative-strategy-audit.md` 1 (2026-09-03) · `source-pulls/ad-account.md` 8 (2026-09-03) · `personas-profile.md` 2 · `lifecycle-journey-maps.md` 1 · `performance-targets-and-metrics.md` 1 (2026-09-04) · `operations-and-team.md` 4 · `website-and-product-audit.md` 1 (2026-09-03) · `biweekly-iterations-report.md` 4 · `monthly-performance-report.md` 5 (2026-09-03) · `other-reviews.md` 3.
**Independent convergence:** ten documents, written by different agents against different sources, arrived at this question without seeing each other. That is the strongest convergence signal in the roll-up and it is why this heads the brand-routed list.
**Tags:** team `creative-strategy`, scope org-wide.

### 4. There is no ceiling, so nothing can be called too expensive

**Observation.** The brand's tiers say a $22.63 lead is "meh" — under $15 fantastic, over $25 not good — but no customer value, gross margin, lifetime value or maximum tolerable cost per acquisition was ever captured. `running-notes/brand-rules.md` lists unit economics as an open intake item. The account has been in the "meh" band for six straight months and nobody can say whether that is survivable or comfortable. Health insurance renews every year, and no document in this brain records whether Health For Moms earns anything on a renewal.

**Pull — Curiosity.** A brand with a precise four-tier grading scale and no unit economics behind it is grading itself against a number whose origin nobody in this brain can explain.

**Question: What is one matched mom worth to this business over her whole relationship with the partner agency?**

**Justification.** It sets the ceiling on what a lead can cost. Without it, "efficiency first" means efficiency relative to the account's own trailing number, which drifts, rather than to a threshold that holds — and efficiency first is the brand's stated objective.

**Score:** Stakes 5, Confidence 5, Researchability 1, Novelty 5. **Brand-routed** — override.
**The clarifying question for the team:** what does the brand earn on one enrolled family, and does it earn anything on the renewal?

**Consolidates** (2 upstream loops): `performance-targets-and-metrics.md` 2 (2026-09-04) · `lifecycle-journey-maps.md` 4.
**Tags:** team `creative-strategy`, scope org-wide.

### 5. The cheapest leads this account ever bought came from the format it stopped making

**Observation.** Lifetime, statics carry **529 ads, $168,907.73 and 13,735 leads at a $12.30 cost per lead**, against video's 1,593 ads, $574,310.36 and 25,834 leads at $22.23. Statics took **22.7% of the money and delivered 34.7% of the leads**. Not one has run in the last 180 days. The two cheapest ads at real scale in the account's history are both statics that name a specific person in a specific moment, and both are dark — including `B1 samar- Copy`, $35,219.98 lifetime for 3,046 leads at **$11.56**, headline *"Didn't know I could ditch my job's health plan… until I did."* The brand has since decided to *"focus mostly on video ads."*

**Pull — Gap.** The lever the method docs and this account's own history both point at hardest is the one lever nobody has pulled. `andromeda-v2.md` puts format at the top of the differentiation hierarchy — a video-to-static change is the single strongest signal available to Meta — and this account has iterated its most-used text hook four times without once changing the format.

**Question: What made the team stop making statics?**

**Justification.** Statics are the fastest way to raise this brand's stated capacity of one to five net-new concepts a month before November 1, and four of the strongest moves available assume they are on the table. If it was a staffing or agency change, they come straight back. If something was learned — a lead-quality problem from static form-fills, a platform issue, a failed test — that reason is a hard constraint nobody has written down, and it changes several recommendations at once.

**Score:** Stakes 4, Confidence 5, Researchability 1, Novelty 5. **Brand-routed** — override.
**The clarifying question for the team:** what happened around March that took statics out of the account?

**Consolidates** (5 upstream loops): `quarterly-whitespace-analysis.md` 1 (2026-09-04) · `ad-account-evaluation.md` 1 · `visual-vocabulary.md` 3 · `source-pulls/ad-account.md` 1 (2026-09-03) · `biweekly-iterations-report.md` 2.
**Note:** the premise "this account has never run a static," carried by three 90-day audits, was overturned by a lifetime pull and is recorded as a closure below. What stays open is why they stopped, not whether they ran.
**Tags:** team `creative-strategy`, scope org-wide.

### 6. Three quarters of the budget disappeared and the account shows no scar

**Observation.** Monthly spend went from **$156,716 in April to $18,390 in July** and back to $42,749 in August — a **73.5% fall** across the quarter — while cost per lead moved one cent, $22.65 to $22.64. Leads fell by exactly the same percentage as spend, which is what a tap being turned down looks like rather than a machine breaking.

**Pull — Surprise.** A collapse that size normally leaves a mark on efficiency somewhere, and this one left none at all.

**Question: What drove the drop in monthly spend from April through July?**

**Justification.** Whether this was a budget decision, a partner-capacity limit on how many leads the agencies could absorb, or something else entirely changes what the word "scale" can even mean for the November push. A capacity ceiling and a budget choice call for completely different plans on 2026-11-01.

**Score:** Stakes 4, Confidence 5, Researchability 1, Novelty 4. **Brand-routed** — override.
**The clarifying question for the team:** was the spring spend reduction a budget call, or did the partner agencies cap how many leads they could take?

**Consolidates** (2 upstream loops): `90-day-performance-audit.md` 2 (2026-09-03) · `performance-targets-and-metrics.md` 5 (2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

### 7. Two groups of women describe opposite failures of the same handoff

**Observation.** One group reports being flooded with calls within five minutes of submitting the form. Another group, five comments spread across fourteen months, reports that nobody ever contacted them at all. Both describe the same funnel in the same window. Alongside them, the third-highest-liked record in the corpus at 33 likes is a warning about what happens to your phone number, and the highest-liked question at 15 likes asks *"How many calls will I get if I try to see how this works?"* — with 49 of 1,322 comments, 3.7%, mentioning calls.

**Pull — Tension.** It fired when the two complaint families landed in the same search results and could not both describe one system behaving one way.

**Question: What decides how many times a woman who fills in the form gets contacted?**

**Justification.** These are opposite failures needing opposite fixes and both are killing conversion in public. If it turns out to be which partner agency the lead lands with, that is a routing problem the brand can act on this month, and it touches gate two directly.

**Score:** Stakes 4, Confidence 4, Researchability 1, Novelty 4. **Brand-routed** — override.
**The clarifying question for the team:** how is a lead routed after the form, and how many agencies can end up contacting the same woman?

**Consolidates** (2 upstream loops): `lifecycle-journey-maps.md` 3 (2026-09-04) · `source-pulls/brand-reputation.md` 1 (2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

### 8. "Nationwide" and the state list point in opposite directions

**Observation.** The brand's stated benefit list opens with *"Nationwide coverage — see any doctor, anywhere in the U.S."* The mechanism that closes nearly every ad says the opposite about availability: *"you have to live in one of those states, otherwise it's not gonna work."* The Approved State List runs to 32 to 34 states in all thirteen ads read at full media depth.

**Pull — Tension.** The brand's headline benefit and the brand's own qualifier point in different directions, and nothing in the brand's materials reconciles them.

**Question: What does Health For Moms have to offer a mom whose state is not on the Approved State List?**

**Justification.** The state gate is the brand's best-known creative device and its answer to a compliance requirement at once. If there is a real offer behind the gate for the other states, that is a whole audience the brand currently turns away at the door — and Texas and Georgia, both named in the comments, are among the largest uninsured states in the country. If there is not, then "nationwide" is describing something other than availability and the brand needs to say which.

**Score:** Stakes 4, Confidence 5, Researchability 1, Novelty 4. **Brand-routed** — override.
**The clarifying question for the team:** is there anything the brand can offer a mother in a state that is not on the list?

**Consolidates** (1 upstream loop): `brand-identity-analysis.md` 2 (2026-09-03). Cross-references the geo-waste loop in Personas 12, which sizes the spend landing off-list and is researchable.
**Tags:** team `creative-strategy`, scope org-wide.

### 9. The named mechanism nobody can describe

**Observation.** The brand's whole differentiation rests on a named, trademarked mechanism it calls the MomSmart Coverage Method — described as *"new tech that scans plans and matches each family with the right private health plan based on their needs, doctors, and budget."* That description is the only account of it anywhere reachable. The brand's guidelines build one of three sanctioned CTA frameworks on top of it, the Mechanism CTA, with a Tech/Scan framing.

**Pull — Curiosity.** A trademark symbol and a named method imply something specific exists, and nothing in the brand's own materials says what.

**Question: What is the MomSmart Coverage Method made of?**

**Justification.** A named mechanism is one of the strongest assets a brand in a crowded category can have and one of the easiest to overclaim. If there is real matching technology behind it, the brand can lead with it and get specific. If it is a name on a routing form, then a third of the CTA architecture is asking creative to promise something that cannot be shown, in a category where the FTC warned 21 health plan marketers and lead generators in December 2024 and sued a Florida operation in April 2026 over $91 million in alleged impersonation.

**Score:** Stakes 4, Confidence 4, Researchability 1, Novelty 5. **Brand-routed** — override.
**The clarifying question for the team:** what actually happens when the MomSmart Coverage Method runs — is there software, and can it be shown?

**Consolidates** (1 upstream loop): `brand-identity-analysis.md` 4 (2026-09-03).
**Tags:** team `creative-strategy`, scope org-wide.

### 10. Discovery is dark from both directions

**Observation.** No survey answer and no Northbeam, so all that is known is which platform served the ad. The brand names peer recommendation as a tipping point that can collapse the decision from weeks to minutes, and the account has scripted it twice — but in fourteen months and 1,322 comments, three mention a friend, none refers anyone to this brand, and a semantic sweep for referral language returns nothing at all. Meanwhile public search on 2026-09-04 surfaced no review site, no comparison page and no third-party profile for this brand. Everything after the form fill happens at a partner agency with its own name and, in all likelihood, its own review surfaces — none of which appear anywhere in this brain.

**Pull — Gap.** There is a whole discovery channel the brand talks about as if it exists, and the only unprompted surface Parker can read shows no trace of it.

**Question: Where does a mom first hear that a service like this exists?**

**Justification.** If the answer is a friend, a Facebook group, a search, or only ever a cold ad, that changes where the money should go and what the creative has to do. If referral is real but invisible, the brand is under-crediting a channel it could feed deliberately. If it is not real, discovery is one hundred percent paid, and every CPM increase before November lands directly on the business with nothing to cushion it. One open text box on the thank-you page would create the confirmed-speaker tier this brain has none of, without needing anything from the partner agencies.

**Score:** Stakes 4, Confidence 4, Researchability 2, Novelty 4. **Brand-routed** — override.
**The clarifying question for the team:** can a single question be added to the thank-you page asking how she heard about this — and which partner agencies do leads go to, so their review surfaces can be checked?

**Consolidates** (4 upstream loops): `post-purchase-surveys.md` 1 and 2 (2026-09-04) · `customer-journey-and-persona-discovery.md` 1 (2026-09-03) · `other-reviews.md` 3 (2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

### 11. The room keeps recommending a different product than the one the brand sells

**Observation.** The brand's whole story runs on a single villain, the system, and its rules forbid naming any specific alternative. In the comments the alternatives are named constantly and specifically: the marketplace **14 times across 8 ad-name groups**, Medicaid **17 across 5**, health shares 5, direct primary care 8, and going without insurance **33 across 10 ads** — all on a 1,322-comment corpus. Several of those recommendations come from licensed professionals. None of them is what this brand offers.

**Pull — Tension.** The brand says the fight is against a faceless system. The customer writes as if the fight is a shortlist of named options she is picking between, and both cannot be the right description of the decision.

**Question: What are moms actually comparing this offer against at the moment they decide?**

**Justification.** If the real comparison is a short list of specific alternatives rather than a vague broken system, the creative is answering a question the buyer is not asking, and it is doing so under a rule that stops it from answering the one she is. The rule is self-imposed rather than legal, so it can be revisited. `creative-strategy-fundamentals.md` says the brand's compliance loop is the operational answer to what can be said — and this rule has never been tested against one.

**Score:** Stakes 4, Confidence 5, Researchability 4, Novelty 3. **Total 16/20. Tier 2.**
Novelty is 3 because the brand already knows people mention alternatives; what is open is which one actually wins the decision.

**Consolidates** (2 upstream loops): `competitive-landscape.md` 2 (2026-09-04) · `community-and-forums.md` 4 (2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

### 12. Rival agents are working the comment section of the account's best ads

**Observation.** **39 comments across 10 ads** pitch competing offers. One operator posted the same Direct Primary Care and health-share script **at least nine times under `MOMS38 - 1 - V1` on a single day**, addressed to different women by name; another version of the same behaviour ran **fifteen pitches inside 54 minutes** on one evening. That ad has spent $54,173 lifetime and is not the account's biggest spender — it is the one people watch longest, holding **17.12%** against 3.81% on the current top spender. The same behaviour appears independently in the open category feed, where two creators are individual licensed agents doing organic lead generation in the comments, one closing with *"comment and I'll be in touch and we will run a quote."* And the most fluent voices in the brand's own threads — guaranteed issue, medical underwriting, level-funded plans, IUA, allowed amount — come almost entirely from brokers, billers and agents.

**Pull — Pattern.** The same behaviour turned up in two unconnected places on the same day of reading: the open category feed and the brand's own paid comment sections.

**Question: How much of the interest these ads create is picked up by other agents before it reaches the brand's own funnel?**

**Justification.** The brand pays for the attention and something else may be converting it. If individual agents are harvesting a meaningful share of the women who watch these ads, the leak is downstream of creative and no hook change fixes it — comment moderation becomes a performance lever rather than a housekeeping chore.

**Score:** Stakes 3, Confidence 5, Researchability 4, Novelty 4. **Total 16/20. Tier 2.**

**Consolidates** (4 upstream loops): `source-pulls/ad-comments.md` 4 (2026-09-03) · `voc-category-jargon.md` 2 (2026-09-04) · `competitive-landscape.md` 1 · `monthly-tiktok-mining.md` 4.
**Tags:** team `creative-strategy`, scope org-wide.

### 13. The account's money and the brand's calendar point at different months

**Observation.** The brand names November 1 as the single most important date on its calendar. Over the thirteen readable months, **November 2025 took 5.4% of spend and March through May 2026 took 58.9%**, with April alone running 4.6 times November. March scaled to 3.9 times February's spend while cost per lead *improved* from $23.39 to $20.85, which is not what a brand pushing into a season it does not belong in looks like.

**Pull — Tension.** The brand's stated calendar and the account's own spend history cannot both be a fair description of when this business makes its money.

**Question: What makes spring this account's biggest season?**

**Justification.** `seasonality.md` says to ask the brand which seasons matter and then validate the claim against the data, because brands are often wrong about their own patterns. This is that check failing. If spring demand is genuinely richer than November demand, the brand is planning its year around its second-best window and the whole production calendar should move. If the spring surge was a budget decision, November stands and has never been properly tested.

**Score:** Stakes 4, Confidence 4, Researchability 3, Novelty 5. **Total 16/20. Tier 2.**
Researchability is 3 because half the answer is the spend-decision question that is brand-routed above; the demand half is readable from CPM, CTR and lead-rate seasonality in the account.

**Consolidates** (1 upstream loop): `marketing-calendar-and-campaigns.md` 1 (2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

---

## Messaging — what is being said and shown

Twenty-six loops, the largest section, which is what the rubric predicts for the broadest and most observational territory.

### 1. The audience believes coverage happens to her, and every ad asks her to believe she can choose it

**Observation.** This is the cross-category convergence the voice-of-customer assembly exists to find, and four separately extracted categories say the same thing. The metaphors say coverage is luck: **11 records** treat another woman's plan as a lottery win, carrying three of the four highest like-counts in the whole library — 19 likes on *"Lucky! Mine is $11,000,"* 11 on *"I guess we're lucky,"* 10 on *"You are lucky. Mine is over $10k."* The trigger moments say the same in life events: what actually changed a woman's coverage in this corpus is a job, a state move, a marriage, an employer, a rehire, a death — almost never a decision she made. The objections say it outright: *"My job picks the plan that they offer."* And the aspirational phrases say it at the top of the funnel, where six records ask for the whole system to be replaced rather than shopped. Alongside it runs the counter-bid: the ad states $6,000 and **82 comments answer with "mine is," 76 with a specific figure, and 64 of those — 84% — name a number higher**. The words that recur are win, lucky and must be nice. Almost nobody answers the offer.

**Pull — Pattern.** The same belief keeps surfacing in four categories that were extracted separately, by different passes, from different slices of the corpus, and none of them could see the others.

**Question: What does this audience believe she has the power to change about her own coverage?**

**Justification.** If she believes the answer is nothing, then the account's entire persuasion premise is arguing with her worldview before it makes an offer, and no amount of hook testing fixes that. It would reshape the messaging strategy rather than tune it. It is also the deepest read available on why the account's central creative device — stating a number — reliably starts a contest instead of a conversation.

**Score:** Stakes 5, Confidence 5, Researchability 4, Novelty 5. **Total 19/20. Tier 1. The highest-scoring loop in the roll-up.**
Confidence is 5 on independent convergence: four extraction passes, blind to each other, landed on the same belief. Novelty is 5 because nothing in the brand's context document, its guidelines or its creative acknowledges it.

**Consolidates** (7 upstream loops): `voice-of-customer.md` 1 · `voc-metaphor.md` 1 (2026-09-04) · `voc-pain-phrase.md` 1 · `voc-aspirational.md` 1 · `community-and-forums.md` 3 (2026-09-04) · `voc-outcome-phrase.md` 3 · `voc-metaphor.md` 3.
**Note on supersession:** `voc-metaphor.md` filed a narrower version of this question from the luck evidence alone. `voice-of-customer.md` explicitly recorded that it supersedes rather than repeats the narrower one, and that supersession is honoured here.
**Tags:** team `creative-strategy`, scope org-wide.

### 2. She goes looking for proof and finds the FBI

**Observation.** Search "Health For Moms" and you get a federal website launched in May 2026 called Moms.gov, a Missouri state program, a Wikipedia article about a 1996 maternity law, and a rival at `betterhealthformoms.com`. Search the brand plus "legit" and you get the FBI and the FTC warning about health insurance scams, and nothing about this company. Three of the brand's own commenters say they searched and found nothing, including one who concluded from that alone: *"sounds like a scam to me."* Three separate platforms have generated topic pages around review-shaped searches for this brand — `Health For Moms Insurance Reviews`, `Is Health For Moms Insurance Legit`, `Healthformoms Insurance Review` — which get built because enough people run the query, and behind all three there is no review corpus at all. The most engaged reputation artifact anywhere is a pasted AI summary claiming Reddit considers this brand not legitimate, live under an ad since January 2025 with 14 likes and 10 replies. And the highest-liked question in the corpus, *"Anyone actually have this and have insight?"* at 15 likes on 2026-03-20, was answered by five strangers, four of them negatively, while the brand said nothing.

**Pull — Surprise.** A brand can be small and still be findable. This one is unfindable in a specific way, because its name is made of words that a decade of government and nonprofit health content already owns.

**Question: What does a mother find when she looks this brand up before she hands over her phone number?**

**Justification.** Verification is a real step in this buyer's journey — the corpus shows her taking it, first on Google and then in the comments — and it sits before the form rather than inside it. If the name itself is what makes the brand uncheckable, no amount of creative testing touches the problem and the answer is a searchable identity. If the name is fine and the brand is simply young, the work is publishing enough that a search finds something, which is a much smaller job. Those two situations call for very different amounts of work, and right now nobody knows which one this is.

**Score:** Stakes 4, Confidence 5, Researchability 5, Novelty 4. **Total 18/20. Tier 1.**
Researchability is 5: this is a search, a set of AI-assistant queries and a look at three topic pages. It is the cheapest Tier 1 on the list and it can be done today.

**Consolidates** (6 upstream loops): `reputation-analysis.md` 1 and 4 (2026-09-04) · `source-pulls/brand-reputation.md` 3 · `other-reviews.md` 1 · `source-pulls/reddit.md` 2 (2026-09-03) · `customer-journey-and-persona-discovery.md` 2 (2026-09-03).
**Marks carried:** search results `verified` on 2026-09-04; the Reddit verdict inside the pasted summary remains `stated` and unverified.
**Tags:** team `creative-strategy`, scope org-wide.

### 3. What this audience accepts as proof, when the brand has no customers to show

**Observation.** **72.9%** of the last 90 days of spend carries an authority claim, and the account's top creative runs the headline *"Approved by thousands of Mom's across America"* on ads carrying **$71,643.33 of the window's $98,276.81**. Against that: zero reviews, zero press, no Better Business Bureau profile, and two pieces of praise in 1,322 public comments — both from women who were told no. Meanwhile the audience answers the creative directly. From 2025-07-25: *"If you are using a fake person for your testimonial, it unintentionally sends a message to people that no real actual person would say this about your service. I think it's always better to have a real person. Especially with something that is famous for being a scam, like health insurance."* A licensed advisor tells viewers in the brand's own comments never to put their information online. And regulators are actively teaching this audience what to look for: the FTC warned 21 health plan marketers and lead generators in December 2024 and sued a Florida operation in April 2026 over $91 million in alleged carrier and government impersonation. The only people in 1,322 comments who speak with authority are brokers and agents, across 13 different ads.

**Pull — Tension.** The brand leans on authority and voices in its creative, and the audience is openly reading those voices as evidence that no real customer exists. Both cannot hold.

**Question: What does a mother in this category treat as proof that a health insurance offer is real?**

**Justification.** Trust is the binding constraint in this category, not attention — the hook rates are healthy and the doubt is loud. Proof strategy is therefore the whole messaging problem for a brand at this stage, and getting it wrong is expensive at $98,276 of spend a quarter. If the proof she wants is a carrier name, a licence number, a state filing or a real woman on camera rather than a testimonial, then a warm mom-to-mom voice is solving a problem she does not have and the brand's whole credibility stack is pointed the wrong way. This is the fork that routes proof, claims and casting together, which is why it is graded here under Messaging rather than split across two territories.

**Score:** Stakes 5, Confidence 5, Researchability 4, Novelty 4. **Total 18/20. Tier 1.**

**Consolidates** (8 upstream loops): `source-pulls/customer-reviews.md` 3 (2026-09-04) · `category-and-market-research.md` 4 (2026-09-03) · `source-pulls/reddit.md` 5 (2026-09-03) · `90-day-creative-strategy-audit.md` 4 (2026-09-03) · `ad-account-evaluation.md` 5 (2026-09-04) · `90-day-diversity-audit.md` 6 (2026-09-03) · `organic-channels-inventory.md` 3 (2026-09-04) · `source-pulls/brand-reputation.md` 4.
**Note on cross-territory collapse:** four of those loops were tagged Creators and talent upstream, asking who is credible on camera. That is the same fork wearing a second territory tag, so it collapses here under its primary territory. The casting question that survives separately is the AI-presenter loop in Creators and talent, which asks about production method rather than proof.
**Tags:** team `creative-strategy`, scope org-wide.

### 4. The category's biggest room is a woman finding out the real price on camera

**Observation.** One video in Parker's mining library holds **6.2 million views, 208,000 shares and 22,700 comments** — a doctor phoning around hospitals to get self-pay pregnancy pricing. That is **66.1% of every view in the library** and roughly seven times the next video. The 20 largest videos carry at least 27,337 comments between them, against 1,342 across this brand's entire advertising history. The mechanic is the same one the brand already owns: its scripted insurance call holds **24.48%** of viewers, the highest hold rate in its whole account and double the 12% craft floor — except the brand's ad set is named "20k skit v2," so the team classifies as comedy the exact structure a doctor used as documentary. The brand's version produces a **$30.91** lead, in its worst cost tier. Separately, the category's biggest video makes its entire case with red billed prices stacked against green cash prices and never says the word expensive, while the brand's whole colour language is 41 state names in grey with green checkmarks.

**Pull — Surprise.** Given a category everyone says is boring and confusing, a video of somebody doing paperwork out loud gathered two hundred times the audience this brand has gathered in twenty months.

**Question: What is it about watching someone find out the real price that makes this many people talk?**

**Justification.** If the audience will watch a genuine act of discovery but not a claim about savings, the account's whole format library is aimed at the wrong thing, and that reshapes the creative approach rather than one ad. The brand already has the best-holding format in its account sitting in this exact shape and is spending it on a punchline. It also has a scripted baseline to measure any answer against, which is rare.

**Score:** Stakes 4, Confidence 5, Researchability 4, Novelty 5. **Total 18/20. Tier 1.**
Novelty is 5: the account has never made anything in this shape deliberately, and the one time it landed near it, the ad set name shows the team did not know what it had.

**Consolidates** (4 upstream loops): `community-and-forums.md` 1 (2026-09-04) · `monthly-organic-tiktok-audit.md` 1 · `visual-vocabulary.md` 2 · `monthly-hook-audit.md` 5 (2026-09-03, partial — its Authority half sits with loop 3 above).
**Tags:** team `creative-strategy`, scope org-wide.

### 5. The account builds format variety and then starves it

**Observation.** Three separate drops inside three weeks, each collapsing onto a single file. The Moms53 drop of 2026-08-25 put seven files up at one timestamp and `moms-53 3` took **$1,955.60 of $1,960.50 — 99.75%**, leaving $4.90 for the other six. The Moms65 drop of 2026-08-27 put eleven up and `moms-65 1a` took **$1,283.97 of $1,375.03 — 93.4%**. The moms 68 drop of 2026-08-31 put fifteen up and the whole batch drew **$4.23 across 163 impressions in five days**, while three duplicates of existing winners took $2,080.15 in the same week. The starved files include real bets on angles the account has never tested at scale: the $4,600 MRI cash-price comparison at a $15.38 cost per lead on $46.13, a creator reshoot of the account's best-CTR hook that got $0.33, and the only split-screen reaction vehicle in the drop at $2.06. This is an account whose own diagnosis is that it lacks creative diversity.

**Pull — Surprise.** An account that built a batch of diversity and then gave it almost nothing, three times in a row inside seven days of each other.

**Question: What decides which new files in this account get delivery in their first week?**

**Justification.** Every format test this brand runs before November dies unmeasured if the answer is budget structure rather than performance, which makes it a media-buying problem wearing a creative problem's clothes. `andromeda-v2.md` names a specific mechanism that would explain it: Meta assigns an Entity ID by analysing visual content, especially the first three seconds, and files judged too similar get grouped — sharing delivery and data, with the second file piggybacking on the first and generating no incremental reach. Several starved files in these drops carry the same footage or the same verbal hook as the winner. If that is what is happening, the constraint on this brand's learning rate is the fingerprint of its creative, not its budget, and the fix is genuine format differentiation rather than a budget split. Either way, this decides whether the brand can learn anything at all in the 58 days it has left.

**Score:** Stakes 4, Confidence 5, Researchability 5, Novelty 4. **Total 18/20. Tier 1.**
Researchability is 5 — ad-set structure, budget settings, creation timestamps and per-file delivery are all in the account.

**Consolidates** (3 upstream loops): `weekly-performance-snapshot.md` 1 (2026-09-04) · `biweekly-iterations-report.md` 1 · `ad-account-evaluation.md` 2.
**Tags:** team `creative-strategy`, scope org-wide.

### 6. The number this team steers by did not move through a total creative overhaul

**Observation.** Cost per lead went **$22.65 to $22.63** across two quarters while spend fell 73.5%, ad count fell 70.4%, the dominant format collapsed into one container at roughly 70% of spend, the dominant emotion swapped from anger at 55.2% to pride at 49.5%, the awareness posture inverted, and spend-weighted hold rate fell from **11.09% to 3.83%**. The one metric everyone watches was the one metric that stayed still. Underneath it, the hold-rate picture runs backwards from the craft standard: the account's cheapest lead comes from an ad holding **2.39%** with a 3.38-second average play time, while its best-holding ads sit in the worst cost band at $29.78 to $38.09, and the craft floor is 12% to 15%. The formats with the strongest hold rates are also the most expensive — Educational at $32.00 per lead, Graphic Video at $31.82, Other at $33.62, against a POV blended $21.31.

**Pull — Tension.** A metric that survives that much upheaval untouched and a creative overhaul that large cannot both be describing the same account honestly.

**Question: What would tell this team that its creative got better, if cost per lead cannot?**

**Justification.** Every brief, every test verdict and every scale decision in this brain currently gets graded against a number that appears nearly blind to the thing it is grading. This is the re-formulation of a whole cluster of hold-rate loops: the surface question was whether hold rate matters here, and the real question underneath is what this account should be measuring at all. `ad-account-analysis.md` separates scale metrics from behaviour metrics for exactly this reason, and this account is reading a scale metric as if it were a behaviour metric. The honest partial answer already visible is that cost per lead is measuring the offer, and the offer did not change.

**Score:** Stakes 5, Confidence 5, Researchability 3, Novelty 4. **Total 17/20. Tier 1.**
Researchability is 3: the complete answer needs gate two, which is brand-routed. But a great deal is answerable from Meta's own funnel — cost per link click, landing-page-view rate, the click-to-lead rate, and the share of leads arriving from viewers who watched past three seconds. That is enough to build a working scoreboard while gate two is pending.

**Consolidates** (5 upstream loops): `performance-targets-and-metrics.md` 4 (2026-09-04) · `monthly-hook-audit.md` 3 (2026-09-03) · `ad-account-evaluation.md` 3 · `90-day-diversity-audit.md` 1 and 7 (2026-09-03, both killed separately below and folded here as evidence).
**Tags:** team `creative-strategy`, scope org-wide.

### 7. The one creative that earns agreement never mentions a number

**Observation.** Roughly **12 clear recognitions exist in 1,342 comments**, under 1%, and nearly all of them sit on the `MOMS38 - 2` denial skit, where one woman plays both the frustrated mother and the claims rep denying a claim because it happened on a Tuesday. That family holds **24.48%** of viewers against the current top spender's **3.28%**, and it has spent about **$3,774.02** against roughly **$110,205.90** on the peaceful-outcome montage nobody recognizes. Every other creative in the account earns argument. The one pain phrase found on that family names time and exhaustion rather than money: *"I literally was just on the phone for hours today figuring out something eith insurance...and still no answer."* The objection clusters confirm the same shape from the other side — the skit family draws essentially no objections while the `MOMS38 - 1` family absorbs the bulk of the correction, call-fear, state and legitimacy complaints. And the format tagger could not name what the skit is doing: `Other`, the bucket applied when no defined format can confidently be assigned, holds 11.49% spend-weighted and was the account's largest bucket last quarter at 36.9% of spend across 29 ads.

**Pull — Resonance.** The comments under that skit read completely differently from the comments under everything else in the account, and the reason it works is worth understanding before anyone scales it.

**Question: What is the pain this audience recognizes without being shown a price?**

**Justification.** The account's whole emotional vocabulary is financial, and the only creative earning agreement instead of argument dramatizes an experience rather than a bill. If the recognizable pain is the fight and the phone call rather than the deductible, the brand has a second messaging lane it has barely used — and it currently cannot brief more of it, because a format nobody can name is a format nobody can scale. A creator cannot be asked to make another `moms54-3` except by being shown the video.

**Score:** Stakes 4, Confidence 5, Researchability 4, Novelty 4. **Total 17/20. Tier 1.**

**Consolidates** (9 upstream loops): `source-pulls/ad-comments.md` 5 (2026-09-03) · `personas-profile.md` 5 · `persona-voice-library.md` 2 · `voc-pain-phrase.md` 5 · `voc-objection.md` 1 · `monthly-hook-audit.md` 2 (2026-09-03) · `visual-vocabulary.md` 1 · `90-day-diversity-audit.md` 5 (2026-09-03) · `voc-corpus-profile.md` 5 (2026-09-03).
**Independent convergence:** nine documents. `visual-vocabulary.md` arrived at the same place through a completely different lens — it noticed that the two things holding longest both put a second character in the frame, at 27.31% and 24.48%, while everything the account spends on is one woman at arm's length holding 3.28%. That is a mechanism read of the same finding and it is recorded as corroboration rather than a separate loop.
**Tags:** team `creative-strategy`, scope org-wide.

### 8. The account's cheapest attention produces its most expensive leads

**Observation.** The crying-mom openers stop more people than anything else in the account, at **57.02% and 52.40% hook rates**, and produce leads at **$29.85 and $38.09** against a $22.10 account average — while the calm POV and state-list openers stop fewer people and deliver leads at **$13.29 to $16.01**. The Moms54 set posted the best attention numbers anywhere in the account this month, a 57.02% hook rate with a 13.65% hold rate and an 8.08-second average play time, and the worst lead cost. The account is currently building more of that lane: six ads and climbing. Meanwhile not one of the nine niche organic videos in the category library opens on visible distress, and the strongest ones open calm and let the fact carry the shock.

**Pull — Surprise.** The ranking flipped when the account was sorted by hook rate versus by cost per lead, and the ad with the best stop rate in the whole account sits in the brand's worst cost tier.

**Question: What is happening between the stop and the form fill that makes a high-distress opener cost so much more per lead?**

**Justification.** Production is buying the distress lane right now. If intensity is actively working against lead cost, that production is buying the wrong thing, and the decision has to be made before the November build. It also has an unusually clean control: the same account, the same offer, the same state list, two emotional registers, opposite results.

**Score:** Stakes 4, Confidence 5, Researchability 4, Novelty 4. **Total 17/20. Tier 1.**

**Consolidates** (3 upstream loops): `monthly-hook-audit.md` 1 and 7 (2026-09-03) · `monthly-performance-report.md` 3 (2026-09-03).
**Tags:** team `creative-strategy`, scope org-wide.

### 9. The savings number nobody can trace

**Observation.** Every claim this brand makes about value rests on one figure, **"up to 30%,"** and nothing anywhere says what it compares to, how it was calculated, or whether any real family has hit it. The account has carried a flat **"20% or more"** across roughly two thirds of its lifetime static spend and a **"24% cheaper"** testimonial headline on another **$29,814.72** — while the brand's own guidelines call a flat savings claim non-negotiable and forbidden. On 2026-09-03 a commenter wrote that she called, spent hours, and was quoted $400 a month, under an ad whose text hook promises saving $400 a month; that hook carries the majority of the account's spend.

**Pull — Tension.** The brand's own hard rule and the brand's own running copy cannot both be right, and neither one names a basis for the number.

**Question: What does the "up to 30%" savings figure actually compare against?**

**Justification.** This number is the brand's central promise and the thing every ad ends on. If it compares against a specific baseline the brand can name, the claim gets stronger and more specific, which is exactly what the brand's own specificity principle asks for. If nothing sits behind it, the brand's biggest claim is its most exposed one, every asset carrying a flat version of it is a live risk, and the cheap-click-dear-lead pattern already visible on `moms-53 3` may be the funnel failing to close a promise it cannot keep.

**Score:** Stakes 5, Confidence 5, Researchability 1, Novelty 4. **Brand-routed** — override.
**The clarifying question for the team:** what is the "up to 30%" measured against, and what does a typical quote actually come back at?

**Consolidates** (2 upstream loops): `brand-identity-analysis.md` 1 (2026-09-03) · `weekly-performance-snapshot.md` 2 (2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

### 10. The approval nobody can see

**Observation.** The headline on the account's top creative reads *"Approved by thousands of Mom's across America,"* and it runs on ads carrying **$71,643.33 of the last 90 days' $98,276.81** — roughly three quarters of live spend. Verified against every checkable surface on 2026-09-04: zero reviews, zero press, no Better Business Bureau profile, and two pieces of praise in 1,322 public comments.

**Pull — Tension.** The brand asserts mass third-party approval and every independent surface is empty, and both of those cannot be the whole truth.

**Question: Where could a customer actually see the approval the ads claim?**

**Justification.** It decides whether this brand has an unused proof asset sitting in its partner agencies' call logs or an unsupported claim running on nearly three quarters of live spend — in a category where the FTC has warned twenty-one companies in this exact business about deceptive claims. Those two situations call for opposite actions, and one of them is urgent.

**Score:** Stakes 5, Confidence 5, Researchability 2, Novelty 4. **Brand-routed** — override.
**The clarifying question for the team:** what record sits behind "approved by thousands," and can any of it be shown?

**Consolidates** (1 upstream loop): `reputation-analysis.md` 2 (2026-09-04).
**Note:** this and loop 9 are the two unsupported claims the task brief flags as running on most of spend. Read together they carry roughly three quarters of the window's $98,276.81.
**Tags:** team `creative-strategy`, scope org-wide.

### 11. The anger lane got switched off and nobody wrote down why

**Observation.** Last quarter, five ads led by `MOMS38 - 1 - V1` with the text hook *"Health Insurance is a scam 🙄"* spent **$120,386.57** between them, at cost per lead figures from $20.03 to $25.48 and hold rates from **14.61% to 17.29%** — the best retention numbers in the account's history. This quarter all five have exactly zero spend, anger fell from **55.2% of spend to 2.6%**, and no ad anywhere in the current quarter holds above 7.60%. A direct pull of those five ad IDs against the current window came back with zero rows. Alongside them, six formats left the account entirely — Authority Figure, Street Interview, Infomercial/VSL, Humour, Offer Based and B-roll mashup with voiceover — and Stitch Hooks fell from $32,885.20 to $8.14, a 99.98% drop. The format count went from 20 to 15 in the three months since the brand told us its problem was too little creative diversity. Nothing in the brand context or the four Parker chat threads records a decision to stop.

**Pull — Surprise.** Five ad IDs that carried a third of the previous quarter's spend at the account's best-ever retention returning zero rows is not what the setup would predict.

**Question: What made the team move away from the scam-angle creative?**

**Justification.** If it was killed for a reason Parker cannot see — a platform warning, an agent complaint about lead quality, a brand-safety call — then that reason is a hard constraint that should shape every future concept and Parker is currently blind to it. If it simply drifted out while newer ads were built, the account has an unclaimed asset with the best hold rates it has ever produced sitting idle 58 days before Open Enrollment. Those two worlds call for opposite plans.

**Score:** Stakes 4, Confidence 5, Researchability 1, Novelty 5. **Brand-routed** — override.
**The clarifying question for the team:** were the scam-angle ads and the six missing formats stopped on purpose, and if so, what happened?

**Consolidates** (2 upstream loops): `90-day-creative-strategy-audit.md` 2 (2026-09-03) · `90-day-diversity-audit.md` 3 (2026-09-03).
**Tags:** team `creative-strategy`, scope org-wide.

### 12. A rule the brand marked non-negotiable and a live script in its own account disagree

**Observation.** The non-negotiable rules ban government and ACA references and put "ACA" on the never-used word list. Two ads created 2025-12-05 run a script saying the brand operates *"completely outside the marketplace system"* and is *"not locked into Obamacare rules."* They spent $170.46 for 9 leads at $18.94, and they are the only ads in the account's life that speak the income-gap mom's language — one of them: *"Making over 50k just disqualified this family from affordable health care, but it secretly qualified them for something way better."* Three ads in the account's history name a subsidy, all created that same day, totalling **$379.92 — 0.05% of lifetime spend**. Meanwhile the enhanced ACA subsidies expired on 2026-01-01, pushing roughly 4.8 million people out of coverage they could previously afford, with households just above the cutoff hit hardest. That is the brand's stated buyer.

**Pull — Tension.** A rule the brand marked non-negotiable and a live script in the brand's own account cannot both be describing what this brand is allowed to say.

**Question: What is the actual boundary on naming government programs in this brand's creative?**

**Justification.** `creative-strategy-fundamentals.md` says the brand's compliance loop is the operational answer to what can be said — if a claim has run in market, the compliance loop already filtered it. Two ads ran. So the question is whether the rule is a hard legal line or a strong preference. The income-gap mom is a stated ICP whose entire story is a comparison the rule forbids, and the market's single defining event of the last year is the one the account has spent $379.92 on. Knowing the boundary decides whether a whole persona is reachable or permanently off the table before November.

**Score:** Stakes 5, Confidence 5, Researchability 1, Novelty 5. **Brand-routed** — override.
**The clarifying question for the team:** is the ACA and government-program ban a legal requirement from the carriers or the partner agencies, or a brand preference?

**Consolidates** (2 upstream loops): `quarterly-whitespace-analysis.md` 4 (2026-09-04) · `marketing-calendar-and-campaigns.md` 4 (2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

### 13. The brand's biggest phrase has been said millions of times and come back zero

**Observation.** *"Wife of the year energy"* carries **67.8% of the account's 90-day spend** and produced 3,120 of 4,336 leads. In 1,342 comments, re-verified live on 2026-09-04, not one person uses the phrase. "Overpaying" appears once, about drug prices. *"Has your back"* closes five of the ten highest-spending ads and appears exactly once — from a woman quoting it in scare quotes to point out that she was excluded for being pregnant with type one diabetes. Meanwhile the phrases that do recur in customer language, the deductible arithmetic and the word scam at 48 instances across 15 ads, are ones the brand picked up from customers rather than the reverse. Nobody repeats the brand's phrase and nobody rejects it. Compare that with the AI presenter, which nobody was asked about and six people volunteered opinions on.

**Pull — Gap.** There is an enormous amount of paid repetition here and zero trace of it in what anyone says back, and nothing has been done with that fact.

**Question: What words do the moms who actually convert use for the moment they find a better plan?**

**Justification.** The brand is writing the winning moment in its own voice with no way to check it. If converting moms describe that moment differently, the hook carrying two thirds of the spend is built on invented language that happens to work, and the real version could work harder. It also decides whether the brand keeps writing its own metaphors or goes back to borrowing them — which is the choice separating the language that carries this account from the language sitting unused in its context document.

**Score:** Stakes 4, Confidence 5, Researchability 2, Novelty 4. **Brand-routed** — override.
**The clarifying question for the team:** can a thank-you-page question or a set of agent call notes capture how a woman describes the moment she found a plan that worked?

**Consolidates** (7 upstream loops): `source-pulls/brand-self-echo-detection.md` 1 (2026-09-03) · `persona-voice-library.md` 1 · `voc-anti-language.md` 4 · `voc-metaphor.md` 2 · `voc-aspirational.md` 2 · `voc-outcome-phrase.md` 1 · `post-purchase-surveys.md` 3.
**Tags:** team `creative-strategy`, scope org-wide.

### 14. Twenty months, 1,342 comments, and not one brand reply

**Observation.** Zero brand replies in 1,342 comments across twenty months and 112 ads, confirmed by two semantic searches on 2026-09-04, one deliberately loosened and still returning only customers and rival agents. **166 of 1,322 records, 12.6%, contain a question mark** and 42 contain the word "qualify." The highest-liked question in the whole corpus, *"Anyone actually have this and have insight?"* at 15 likes, sat unanswered while five strangers answered it, four of them negatively. In at least one case another commenter had to explain that declining employer coverage is allowed. In the same week the team asked Parker to help hide comments and to help ban a rival operator, and both are reasonable.

**Pull — Tension.** The brand describes its partner agents as friendly, approachable and pressure-free, and its own public conduct in the only room where people ask about it is silence followed by enforcement. Both cannot be the whole picture.

**Question: What is stopping the brand from replying in its own comment sections?**

**Justification.** The answer separates a real constraint from a habit, and the two lead somewhere completely different. If compliance or the partner agreement forbids the brand speaking about coverage in public, then moderation genuinely is the only lever and the strategy should stop expecting more. If nobody has simply ever owned it, then in a category where trust is the binding constraint, the cheapest available win is answering the question people keep asking — at the cheapest possible point in the funnel, before any form.

**Score:** Stakes 4, Confidence 5, Researchability 2, Novelty 4. **Brand-routed** — override.
**The clarifying question for the team:** is there a compliance or partner-agreement rule that stops the brand replying to comments about coverage?

**Consolidates** (4 upstream loops): `operations-and-team.md` 2 (2026-09-04) · `reputation-analysis.md` 4 · `voc-corpus-profile.md` 2 (2026-09-03) · `voc-objection.md` 6 (partial).
**Tags:** team `creative-strategy`, scope org-wide.

### 15. One mechanism, no second

**Observation.** The Approved State List appears in **all 13 ads read at full media depth** and sits behind roughly **92.7%** of the 90-day spend. No funded ad in the current window asks for the click on any other basis. The brand describes its winner as "the state angle" — verbatim from intake, *"State angle has worked very well if you see the account. Emotional and direct response."*

**Pull — Gap.** An entire account has been built on one mechanism, and there is no evidence anywhere in the current spend about what happens without it.

**Question: What makes a mom click when the state list is not the reason?**

**Justification.** The gate is a real asset and a single point of failure at once — a compliance qualifier, a scarcity device and a curiosity hook in one. If it fatigues or the state footprint changes, the account has no second mechanism and no idea what one would look like.

**Score:** Stakes 4, Confidence 5, Researchability 4, Novelty 3. **Total 16/20. Tier 2.**
Novelty is 3 because the account's own lifetime library partly answers it: the statics era ran non-state hooks at a $12.30 cost per lead, including *"Didn't know I could ditch my job's health plan… until I did"* at $11.56 on $35,219.98. That history time-discounts the question without closing it.

**Consolidates** (1 upstream loop): `source-pulls/ad-account.md` 7 (2026-09-03).
**Tags:** team `creative-strategy`, scope org-wide.

### 16. The angle nobody in the category has taken

**Observation.** The team's own Reddit research named the mental load as an untouched angle — the hours on hold, the explanations of benefits, the prior authorisation fights. Reading all 23 category videos afterwards found **no video that takes it as its subject**. The brand's own corpus points the same way: the one pain phrase attached to the only creative that earns agreement names time and exhaustion rather than money, and a woman offers to dig out her old notebook and phone a stranger about chronic Lyme disease while another walks a mother through the TEFRA and Katie Beckett programs — under paid insurance ads.

**Pull — Gap.** A whitespace the team identified from one source survived a completely independent second source without a single counter-example.

**Question: How much demand is sitting behind the invisible work of managing a family's insurance?**

**Justification.** `creative-strategy-fundamentals.md` says to size the opportunity before asking how to capture it, and this is the sizing question. The brand's lead ICP is defined by carrying more than anyone can see, so an angle nobody in the category speaks to may be the closest thing to open ground it has — but a 23-video library is thin evidence for a category-wide absence, and the honest first move is measuring the demand rather than briefing the ad.

**Score:** Stakes 4, Confidence 3, Researchability 4, Novelty 5. **Total 16/20. Tier 2.**
Confidence is 3 and that is the constraint: 23 videos, 19 relevant, is a small window on a category. The absence may be the library's rather than the world's.

**Consolidates** (1 upstream loop): `monthly-organic-tiktok-audit.md` 5 (2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

### 17. She thinks she has to wait, and nobody has ever told her she does not

**Observation.** **Zero of 2,122 ads** in the account's whole history contain the word "deadline." The brand's own document names *"I should just wait for open enrollment"* as a timing objection that can cause months of delay. The product genuinely has no enrollment window, because private medically underwritten plans have no enrollment period — a real and unusual advantage — and no ad has ever said so. Meanwhile the comments show women telling each other to wait for November, and being told by their state that they must.

**Pull — Gap.** There is a true, substantiable, differentiating fact about this product sitting right there, and in twenty-one months of advertising it has never been said out loud.

**Question: How many moms hold off on this product because they think they have to wait for a window?**

**Justification.** `creative-strategy-fundamentals.md` draws the line that matters here: a misconception to overturn is a different creative move than a value barrier to reframe. If the belief is common, the brand has eleven months of demand it is not speaking to. If it is rare, the year-round push is worth less than it looks.

**Score:** Stakes 4, Confidence 3, Researchability 4, Novelty 5. **Total 16/20. Tier 2.**
Confidence is 3 because the corpus shows almost nothing — "open enrollment" appears in 1 of 1,322 records — and the brand's stated objection list is exactly the record whose provenance is under question in the brand-routed loop above. The belief may be real and simply unspoken in comments, or it may be an assumption the brand wrote about itself.

**Consolidates** (2 upstream loops): `marketing-calendar-and-campaigns.md` 3 (2026-09-04) · `voc-objection.md` 2 (partial — its provenance half is brand-routed).
**Tags:** team `creative-strategy`, scope org-wide.

### 18. The listening post is closing

**Observation.** Of the 207 comments containing "deductible," only 5 predate 2026-03-10 — the day the MOMS38 family launched — and only 5 came after 2026-06-01. So **197 of 207, or 95.2%, land inside 83 days**. March 2026 holds 340 comments and April holds 506: **846 of 1,322, or 64.0%, in a 61-day window**, against all of 2025 at 227, or 17.2%, across twelve months. Since 2026-07-01 the corpus holds **86 comments**, and 36 of the 59 the account received in August are the single word "Help," all on one ad. `voice-of-customer.md` put it plainly: a fourteen-month corpus turns out to be, in practice, a ten-week corpus, and 60.1% of it sits on one creative family.

**Pull — Surprise.** For a brand still spending heavily, finding that its audience stopped talking to it four months ago is not what the setup would predict.

**Question: What is different about the creative running now that the audience no longer tells it anything?**

**Justification.** Comment sections are this brand's only source of customer language and its only check on any persona. If the current creative does not invite disclosure, the brand is losing its research pipeline while the spend continues, and every future refresh of the persona system gets thinner rather than richer. It also decides how much to trust the corpus at all: a messaging bank tuned to a campaign rather than a customer passes that bias to every downstream script.

**Score:** Stakes 3, Confidence 4, Researchability 4, Novelty 4. **Total 15/20. Tier 2.**
Confidence is 4 rather than 5 because of a confound the loop's own docs did not weigh: spend fell 73.5% across the same window. Some of the silence is simply less delivery. The comment drop is steeper than the spend drop, so something else is also happening — but the size of that something is smaller than the raw counts suggest, and this is a case where `creative-strategy-fundamentals.md`'s rule about mention count against denominator cuts against the loop rather than for it.

**Consolidates** (6 upstream loops): `voc-pain-phrase.md` 2 (2026-09-04) · `persona-voice-library.md` 4 · `cross-persona-bias-notes.md` 5 · `voc-corpus-profile.md` 1 (2026-09-03) · `voice-of-customer.md` 3 · `monthly-performance-report.md` 1 (2026-09-03, partial).
**Tags:** team `creative-strategy`, scope org-wide.

### 19. Ten to eighteen seconds of music before anyone says anything

**Observation.** The first spoken word lands at **0:11** on `moms-63 3e`, **0:10** on `moms-65 1a` and **0:18** on `Moms43 - 4 - V3` — the account's top spender. Average play times on those files are 4.03, 3.41 and 4.20 seconds. The one file that opens talking, `moms-53 3`, has the account's best deep retention by a factor of nine and its cheapest clicks at $0.85 to $0.97. Meanwhile ten of the 19 relevant videos in the category library are explicitly noted as having no background music at all, and exactly one uses a music bed as a real choice.

**Pull — Surprise.** An account whose whole diagnosis is that it cannot hold anyone has been opening its biggest ads with ten to eighteen seconds of music.

**Question: What is the silence at the front of these ads doing to the watch?**

**Justification.** `killer-performance-ads.md` treats the first second as the most important part of an ad and seconds one to three as the reason to keep watching; this account spends both on an acoustic track. If the silent runway is the cause of the hold-rate problem, the fix costs nothing and applies to the entire library at once, which would be the cheapest performance gain available before November. It also reframes what "no music" signals in this category — possibly that a real person is talking rather than an asset being played.

**Score:** Stakes 3, Confidence 4, Researchability 4, Novelty 4. **Total 15/20. Tier 2.**
Stakes is 3 because it is a production-note fix rather than a change of direction, but it is the cheapest item in the whole backlog.

**Consolidates** (2 upstream loops): `biweekly-iterations-report.md` 3 (2026-09-04) · `monthly-organic-tiktok-audit.md` 4 (2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

### 20. Strangers are doing unpaid care work inside space this brand pays for

**Observation.** Under `IMG 6`, a comment pasting Reddit's verdict on the brand drew 14 likes and ten replies — and four replies in, two women stopped talking about insurance and started swapping herbs, foods and prayer for chronic Lyme disease, asked each other what state they lived in, and arranged to talk on Messenger. The exchange ran **twenty-five days**. Elsewhere a woman walks a mother through the TEFRA and Katie Beckett programs. Row `052aa855` explains the entire deductible ladder in eight correct lines, unprompted, for a stranger. None of it is about the product, all of it happens under paid placements, and it spans January 2025 to the most recent months of the corpus. It is the only warm thing in 1,342 records.

**Pull — Resonance.** The most generous, detailed and useful writing anywhere in 1,342 comments is being done for free by the audience, and nothing in the brand's context explains why an insurance ad is where it lands.

**Question: What is it about these ads that makes women stop and help a stranger?**

**Justification.** Whatever triggers it is producing the highest-quality engagement in the whole account, and it is currently an accident. If the brand understood it, it could build creative that invites the helping instead of triggering the correcting — the same behaviour pointed at a much better outcome. It also decides whether the comment section is a liability to be moderated or the closest thing this brand has to a community it could host, and the brand is currently acting on the first reading without having asked the question.

**Score:** Stakes 3, Confidence 4, Researchability 3, Novelty 5. **Total 15/20. Tier 2.**

**Consolidates** (3 upstream loops): `voc-surprise-delight.md` 3 (2026-09-04) · `voc-category-jargon.md` 3 · `community-and-forums.md` 2 (2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

### 21. The most passed-on video in the category is one of the smallest

**Observation.** @friencine's forty-six second hospital indemnity video holds the **highest like rate at 14.28%, the highest share rate at 3.97% and the highest save rate at 9.02%** of all 23 videos in the library — on 175,800 views, which is 2.8% of the reach of the biggest video. The ranking completely inverted when rates were computed instead of raw counts.

**Pull — Surprise.** It fired when rates replaced counts and the leaderboard turned upside down.

**Question: What makes people keep and pass on a video in this category at a rate nothing else reaches?**

**Justification.** The brand's whole business runs on a mother telling another mother — peer recommendation is named in its own materials as a tipping point that collapses the decision from weeks to minutes. Whatever drives a share here is the closest organic proxy it has for its own referral mechanism, and referral currently leaves no trace anywhere in the brand's data.

**Score:** Stakes 3, Confidence 4, Researchability 4, Novelty 4. **Total 15/20. Tier 2.**

**Consolidates** (1 upstream loop): `monthly-organic-tiktok-audit.md` 2 (2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

### 22. Two ads, one script, a two-times gap in lead cost

**Observation.** `moms-63 2b` and `Moms43 - 4 - V4` carry the identical text hook, the identical offer and the identical state list. Their costs per lead are **$13.29 and $30.43**. The only material difference is the opening visual: an aspirational walk out of a beautiful home versus a mother lying in bed with a baby. Meanwhile the brand describes its winner as "the state angle," which is the part that does not vary.

**Pull — Tension.** The brand's account of why it wins and the account's own variance cannot both be the whole story, because the named winner is the constant and the difference lives in the variable.

**Question: How much of the cost-per-lead gap between two ads sharing one script is the opening frame carrying?**

**Justification.** Iteration budget follows this answer. If it is the opener, the team should be making twenty first-ten-seconds against one script. If it is the gate, the openers barely matter and the money should go to reach. `andromeda-v2.md` puts hook — the first three seconds, visual and audio — in Tier 2 of the differentiation hierarchy, which says the opening frame should carry a lot; this account has a natural experiment sitting in it.

**Score:** Stakes 3, Confidence 4, Researchability 5, Novelty 3. **Total 15/20. Tier 2.**

**Consolidates** (1 upstream loop): `source-pulls/ad-account.md` 6 (2026-09-03).
**Tags:** team `creative-strategy`, scope org-wide.

### 23. Fear of the phone call, sitting on the exact step every ad asks for

**Observation.** **49 of 1,322 comments, 3.7%, mention calls**, and the loudest ones describe a different company's form. One with 5 likes: *"I filled out something like this years ago- and got spam phone calls every 10 minutes for months!"* Another with 17 likes just asks: *"How many calls will I get if I try to see how this works?"* The third-highest-liked record in the whole corpus, at 33 likes, is a warning about sales calls. A licensed advisor in the same comment section tells people never to put their information online. And the FCC rule that would have banned multi-buyer lead sharing was struck down in January 2025 and formally repealed that September, so nothing is coming to fix it.

**Pull — Pattern.** The same fear keeps surfacing from independent people across fourteen months, aimed at the category rather than at this brand, and it sits on the exact step every ad in the account asks for.

**Question: How much of the gap between a click and a finished form is fear of the phone call?**

**Justification.** Every ad here ends by asking for a phone number. If the phone fear is the main leak, then hook rewrites and savings claims are working on the wrong part of the funnel, and the leverage moves to what the form promises about what happens next. The emotion closest to the click has no creative anywhere in the account.

**Score:** Stakes 4, Confidence 4, Researchability 3, Novelty 4. **Total 15/20. Tier 2.**
Cross-references the brand-routed handoff loop in Product 7 — the fear is measurable here, but what actually happens to her number is not.

**Consolidates** (2 upstream loops): `category-and-market-research.md` 3 (2026-09-03) · `persona-voice-library.md` 3 (2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

### 24. Twenty uses of one hook line and no measurable decay

**Observation.** The POV husband line has run **20 times across five months and $87,991.09**, and its hook rate has not moved — **45.76% lifetime against 45.55%** this window — though the newest copies drift down toward 32% to 43%.

**Pull — Curiosity.** Twenty uses of one line with no measurable decay is not what the fatigue model predicts.

**Question: How much further can one hook line be repeated in this account before attention falls off?**

**Justification.** The answer decides whether the team keeps milking a known winner or starts spending its limited production capacity — one to five net-new concepts a month — on net-new openers. With 58 days to Open Enrollment, that is a real allocation call.

**Score:** Stakes 3, Confidence 4, Researchability 4, Novelty 3. **Total 14/20. Tier 2.**

**Consolidates** (1 upstream loop): `monthly-hook-audit.md` 8 (2026-09-03).
**Tags:** team `creative-strategy`, scope org-wide.

### 25. More shares than comments, on the ad with the most hostile comment section

**Observation.** In the last 90 days `Moms43 - 4 - V3` earned **326 shares against 84 comments**, on $42,741.16 of spend, plus 385 saves. The comment section under that same creative contains the pregnancy objection, the correction thread, and a live rival-agent pitch.

**Pull — Curiosity.** A share is normally a good sign and a hostile comment section is normally a bad one, and here they sit on the same ad.

**Question: Why are people sharing these ads?**

**Justification.** If shares are mothers passing a real offer to a friend, that is the brand's only piece of organic advocacy and it is completely unmeasured. If shares are mothers passing along the joke about a company called Health For Moms that will not cover pregnancy, then the brand is paying to distribute its own worst objection. Those readings call for opposite actions.

**Score:** Stakes 3, Confidence 4, Researchability 3, Novelty 4. **Total 14/20. Tier 2.**

**Consolidates** (1 upstream loop): `reputation-analysis.md` 3 (2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

### 26. Every good outcome in this brand's threads credits somebody else

**Observation.** The best result story in 1,342 records is a woman explaining that insurance never made sense to her until she got the plan she has now, at $180 a month with no deductible. The nearest thing to relief language is a woman thanking her employer. The only "highly recommend" recommends her own existing plan. The account's creative is reliably getting people to describe good coverage, and reliably getting them to describe someone else's. Not a single metaphor in the corpus — fifteen images across 1,342 records — describes a solved situation, a good plan, or relief. Scam, joke, robbery, racquet, dead end, a crack to slip through, a nightmare, a game somebody else is playing.

**Pull — Pattern.** The same thing keeps happening across independent records under different ads, and it is the mirror image of what the creative is trying to produce.

**Question: What does this audience picture on the other side of the problem being fixed?**

**Justification.** The brand has no customer-built image of the good outcome to write toward, so it is currently inventing one — and `voc-outcome-phrase.md` already showed that the outcome language in its context document is the brand's own copy filed under a customer heading. If the ads open by naming a bad number and a bad number invites everyone with a better one to say so, the account is paying to fill its own comment sections with competitor testimonials, and the fix is a creative decision rather than a moderation one.

**Score:** Stakes 3, Confidence 4, Researchability 3, Novelty 4. **Total 14/20. Tier 2.**

**Consolidates** (2 upstream loops): `voc-outcome-phrase.md` 3 (2026-09-04) · `voc-metaphor.md` 3.
**Tags:** team `creative-strategy`, scope org-wide.

---

## Creators and talent — who is on screen and what it says

Four loops. This is the thinnest territory in the roll-up, and that is not because it is clean. Four of its strongest upstream loops asked who is credible on camera, which collapsed into the proof fork under Messaging — the same question wearing a second territory tag. What is left here is genuinely about the people, the roster and the production method.

### 1. The audience is rejecting how these ads are made, not only what they say

**Observation.** **Six records across three years and four ad families** reject the AI presenter, and the newest lands on `MOMS38 - 1 - V2`, a live flagship carrying **$41,592.95** of lifetime spend. Across the wider corpus, 32 comments call the creative AI-generated or fake. One of them argues the mechanism outright, on 2025-07-25: *"This is the problem with AI online commercials. If you are using a fake person for your testimonial, it unintentionally sends a message to people that no real actual person would say this about your service. I think it's always better to have a real person. Especially with something that is famous for being a scam, like health insurance."* Another, on 2025-08-08, replied to an ad simply: *"You don't qualify for Medicaid because you're an AI video.."* And on live creative: *"Creepy AI blonde lady ruins the ad tbh."* Nothing in the brand context acknowledges this. Nobody was ever asked about it — all six volunteered.

**Pull — Pattern.** The same rejection keeps appearing under unrelated creative, years apart, which is the durability that raw count in this corpus never provides.

**Question: What does this audience believe about a brand that uses a synthetic person to sell insurance?**

**Justification.** The account runs AI creative at scale, and trust is this brand's binding constraint rather than attention — its hook rates are healthy and its legitimacy is what people doubt. If the production method itself costs credibility in a category already assumed dishonest, then how the ad is shot is a messaging decision rather than a budget one, and it points the creator and production budget somewhere different. There is also a real tension worth resolving inside the answer: `advertising-to-older-audiences.md` holds that viewers roughly 50 to 70 do not penalise obviously AI-generated footage the way a younger, more media-literate feed does, and that authenticity beats polish for them. This account reaches both groups. The same creative may be costing credibility with one audience and costing nothing with the other, which would make it a casting-by-segment question rather than a blanket rule.

**Score:** Stakes 4, Confidence 5, Researchability 4, Novelty 4. **Total 17/20. Tier 1.**
Novelty is 4 despite `source-pulls/ad-comments.md` noting the objection went near-silent after April 2026. It is not stale: the newest rejection sits on a live flagship, and the silence coincides with the whole corpus going quiet, so it is more likely an artifact of the listening post closing than of the problem being solved.

**Consolidates** (4 upstream loops): `website-and-product-audit.md` 4 (2026-09-03) · `voc-anti-language.md` 1 (2026-09-04) · `source-pulls/ad-comments.md` 9 (2026-09-03) · `source-pulls/customer-reviews.md` 3 (partial — its proof half sits under Messaging 3).
**Tags:** team `creative-strategy`, scope org-wide.

### 2. The brand owns a credential it has never once shown

**Observation.** Across **147 ads with delivery**, every face is a mother talking about her own bill. Authority Figure creative ran four times last quarter and **zero** this quarter, and the account spent $8,884.74 on it last quarter against $0 now. The brand's whole model routes to real licensed advisors, and its compliance rules explicitly allow a real licensed professional while banning a fake doctor character. The one half-test, a pediatrician on screen who never speaks, returned leads at $19.44. In the same window the comment section produced *"don't believe this,"* *"Not recommend"* twice, and a real licensed health insurance advisor publicly telling viewers not to submit their information. Meanwhile the category's single biggest video, at 6.2 million views, is a credentialed person doing credentialed work in public.

**Pull — Gap.** It fired on reading the compliance rule about doctor characters and realising the brand already owns a credential it has never shown.

**Question: Who among the brand's partner agents could appear on camera?**

**Justification.** `advertising-to-older-audiences.md` is direct that authority is the trust shortcut for this demographic — "the news are their influencers" — and this account is already delivering 21.2% of spend to women over 45, rising to 40.2% on the skit family. The brand names casting as its top creative bottleneck. Whether a partner advisor can be filmed decides whether the strongest recommendation in three separate audits is a shoot or a fantasy.

**Score:** Stakes 4, Confidence 5, Researchability 1, Novelty 4. **Brand-routed** — override.
**The clarifying question for the team:** can a licensed partner agent appear on camera, and what would compliance let that person say?

**Consolidates** (2 upstream loops): `monthly-organic-tiktok-audit.md` 8 (2026-09-04) · `90-day-diversity-audit.md` 6 (2026-09-03, partial).
**Tags:** team `creative-strategy`, scope org-wide.

### 3. The only two happy comments about this brand are about a person, not a plan

**Observation.** In 1,322 comments, exactly two report a good experience, and **both women say plainly that no plan was found for them**. One: *"She didn't have anything that fit but pointed me in the right direction!"* The other: *"They weren't able to find a lower price for our particular situation but he was very kind and helpful and respectful."* Neither bought anything. Both left praise anyway. Against that, three defences exist in 1,342 comments and two of them come from someone who sells the plans for a living.

**Pull — Resonance.** Being told no and leaving praise is not normal, and whatever produced it is worth knowing.

**Question: What is the agent conversation giving these women that the product could not?**

**Justification.** The brand's whole positioning rests on agents who feel like "Mom BFFs," and these are the only two public data points showing whether that is true. If the consultation has standalone value, the brand owns a service story it has never told and a proof asset that does not depend on a plan being found — which matters enormously for a business where a large share of applicants are disqualified. Two records is a candidate, not a pattern, which is exactly why this is a question rather than a recommendation.

**Score:** Stakes 4, Confidence 3, Researchability 2, Novelty 4. **Brand-routed** — override.
**The clarifying question for the team:** can a handful of agent call recordings or debriefs be shared, so what happens on a good call can be described?
**Independent convergence:** `voc-surprise-delight.md` filed this loop and explicitly recorded that `voc-outcome-phrase.md` had reached the same question from the same two records through a different lens, asking the assembly to treat it as corroboration rather than two loops. That instruction is honoured here.

**Consolidates** (4 upstream loops): `source-pulls/ad-comments.md` 8 (2026-09-03) · `voc-outcome-phrase.md` 2 (2026-09-04) · `voc-surprise-delight.md` 2 · `source-pulls/brand-reputation.md` 4.
**Tags:** team `creative-strategy`, scope org-wide.

### 4. The roster that was cast and never funded

**Observation.** An ad led by a Black creator got **$206.08**. One led by an Asian-American creator got **$46.83**. One led by a woman in her mid-fifties got **$34.21**. Combined: $287.12. Yet the account's best cost per link click at **$0.93**, its best CTR at **3.15%** and the cheapest lead among the window's top spenders at **$16.07** all belong to `moms-53 3`, led by the account's only visibly mixed-race or Hispanic creator, who has a nose piercing and visible arm tattoos. The two best-holding talking-head units are fronted by women described as mid-forties and late forties to early fifties. Almost every dollar at scale sits on a white woman in her late twenties in a bright house. Separately, across 13 ads read in full, the children shown are infants and toddlers with almost no exception and no teenager appears in any of them — while 42.6% of spend delivers to women 35 to 44 and 12.7% to 45 to 54.

**Pull — Gap.** The creative was made and then starved, so the roster exists on paper and nothing was ever learned from it.

**Question: Who shows up on camera in the ads that perform outside this account's default casting?**

**Justification.** `creative-strategy-fundamentals.md` holds that talent must match persona as a first-order filter and that creative monoculture feeds thin signal density in algorithmic delivery. The one non-default creator who did get meaningful spend produced the best click economics in the account. That is one data point and it could be the script rather than the creator, but it is enough to make the untested roster worth a real budget instead of a rounding error — and casting the child is one of the cheapest variables in the whole production, so if the on-screen child is quietly filtering the audience, the brand is capping its reach with a wardrobe decision.

**Score:** Stakes 3, Confidence 4, Researchability 4, Novelty 3. **Total 14/20. Tier 2.**
Stakes is 3 and Novelty is 3 because this is close to the creative-picking-the-audience loop already promoted under Personas; what is distinct here is the roster question rather than the copy question, and it stays separate for that reason alone.

**Consolidates** (3 upstream loops): `source-pulls/ad-account.md` 4 and 5 (2026-09-03) · `visual-vocabulary.md` 4 (2026-09-04).
**Tags:** team `creative-strategy`, scope org-wide.

---

## Brand-routed — what only the brand can answer

Nineteen loops. Every one of them scored Stakes 4 or higher with Researchability 2 or lower, which triggers the routing override ahead of the total. They are not backlog and they are not lower priority — three of them outrank every promoted loop on stakes. They are here because Parker cannot answer them with any tool it holds.

Read as a whole, they are close to **one conversation with the team and their partner agencies**, and grouping them that way is how they should be asked.

**Group A — the partner agencies (six questions, one conversation).** This is gate two, and it is the largest thing in the roll-up.

| # | The question | Territory |
|---|---|---|
| A1 | What happens to a Health For Moms lead after it reaches the partner agency? | Product |
| A2 | Who do the partner agencies say is actually calling back and enrolling? | Personas |
| A3 | What is one matched mom worth to this business over her whole relationship with the partner agency? | Product |
| A4 | What decides how many times a woman who fills in the form gets contacted? | Product |
| A5 | What is the agent conversation giving these women that the product could not? | Creators and talent |
| A6 | What words do the moms who actually convert use for the moment they find a better plan? | Messaging |

**Group B — the claims and the rules (five questions).** These carry the most exposure. Two of them run on roughly three quarters of live spend.

| # | The question | Territory |
|---|---|---|
| B1 | What does the "up to 30%" savings figure actually compare against? | Messaging |
| B2 | Where could a customer actually see the approval the ads claim? | Messaging |
| B3 | What is the actual boundary on naming government programs in this brand's creative? | Messaging |
| B4 | What does Health For Moms have to offer a mom whose state is not on the Approved State List? | Product |
| B5 | What is the MomSmart Coverage Method made of? | Product |

**Group C — decisions the team already made and never wrote down (three questions).** Each one is a possible hard constraint that would reshape several recommendations at once.

| # | The question | Territory |
|---|---|---|
| C1 | What made the team stop making statics? | Product |
| C2 | What made the team move away from the scam-angle creative? | Messaging |
| C3 | What drove the drop in monthly spend from April through July? | Product |

**Group D — what the brand knows about its own customer (three questions).**

| # | The question | Territory |
|---|---|---|
| D1 | What in the brand's written record of its customer came from a real customer? | Personas |
| D2 | How much money does a mom need to have for this offer to actually work for her? | Personas |
| D3 | Where does a mom first hear that a service like this exists? | Product |

**Group E — permissions (two questions).**

| # | The question | Territory |
|---|---|---|
| E1 | Who among the brand's partner agents could appear on camera? | Creators and talent |
| E2 | What is stopping the brand from replying in its own comment sections? | Messaging |

Each loop's full four-part form, its score line and its clarifying question sit in its territory section above.

---

## Archived this pass

Eleven written verdicts, covering thirteen loop instances — the first one absorbs three. Each kill is recorded with its reasoning, because a loop that dies without written reasoning gets re-surfaced and re-litigated by the next pass, which wastes the cut. A future pass that re-raises any of these must find this verdict first, and reviving one requires new evidence that cites this reasoning.

**1. What happens to a click that lands on `go.healthformoms.co/save/`?**
Raised by `operations-and-team.md` 1, `website-and-product-audit.md` 2 and `monthly-hook-audit.md` 6.
**Killed on reason 5 — infrastructure.** The strategic question is closed: the destination leaks. Four ads pointing at `go.healthformoms.co` recorded 690, 511, 304 and 287 link clicks against 63, 9, 28 and 23 landing page views, with costs per lead of $273.15, no leads at all, $78.54 and $96.42, while the identical video files pointing at `www.healthformoms.co` produced the account's cheapest leads at an 83% to 88% arrival rate. The `USHA - CBO - OTP` campaign spent $3,633.54 in the last 90 days and turned 2,291 link clicks into 167 landing page views and 20 leads at $181.68 each. There is no strategy left in that; it is a broken redirect or a broken pixel, and the rubric routes a pipeline problem to the operational owner rather than into the loops.
**Routed to the operational owner, marked urgent.** Eleven live ads are still pointing at it, 58 days from Open Enrollment. This is not research, it is an afternoon's work, and it should be the first thing anyone does with this document. Two situations call for opposite actions and someone has to look: if the page or pixel is broken, money is being thrown away; if the page works and only the tracking is broken, those 20 leads are an undercount and the campaign is being graded on a number that is not real.

**2. What are the moms who comment "Help" on this ad actually asking for?**
Raised by `monthly-performance-report.md` 1. **Killed on reason 3 — domain knowledge resolves it.** Thirty-six of 59 August comments being the single word "Help" on one ad is a well-understood Meta comment behaviour: people who cannot find or will not tap the link ask in the thread. Routed as an operational note — a reply routine on that ad is cheap and probably worth doing — but it is not a strategic loop.

**3. Why does almost nobody who sees these ads follow the brand?**
Raised by `organic-channels-inventory.md` 2. **Killed on reason 3.** An account with 1,987,158 impressions and 116 page likes is a lead-generation account with no organic surface, no posting cadence and no reason for anyone to follow. The model's own knowledge resolves it, and the useful half of the observation — that the brand has no organic presence at all — is already carried in the promoted proof loop.

**4. What does the qualifier actually say to a woman it turns down?**
Raised by `voc-objection.md` 3. **Killed on reason 2.** Eleven comments across 7 ads describe reaching the end of the qualifier and being rejected with no reason given, and the screen is fully within the brand's control. But the answer changes a line of funnel copy rather than a business decision. Routed to the operational owner as a funnel fix. The strategic half — how many women hit the gate at all — is promoted as Product 2.

**5. What do people write underneath a video that only names the problem?**
Raised by `monthly-organic-tiktok-audit.md` 7. **Killed on reason 5 — infrastructure.** Parker holds the comment counts for the mining library and not one comment body. That is a data-pull gap, and the rubric routes it to data limitations rather than the loops.

**6. Which of these voices belong to the same woman?**
Raised by `voice-of-customer.md` 4. **Killed on reason 5 — infrastructure.** Every `identity_tag` and `behavioral_signal_tag` is null on all 167 snippets because `personas-profile.md` did not exist when the library was assembled. It exists now, generated 2026-09-04. This is a one-pass tagging job, routed to the persona work that owns the slugs, and it should be done before the next roll-up so the library can actually be queried by persona.

**7. Who actually makes these videos?**
Raised by `operations-and-team.md` 3. **Killed on reason 5 — infrastructure.** 147 ads were created in the 90 days to 2026-09-03 by a visible team of one operator and a business partner, across at least four outside naming conventions including sixteen ads batched from an animation supplier on a single day in May. That is a production roster question, and a roster is an operational fact to write down rather than a strategic question to research. **Routed to the operational owner** — and it gates delivery on several promoted loops, so it is worth writing down soon.

**8. What happens to lead volume when the brand answers the eligibility questions in its own comment sections?**
Raised by `voc-corpus-profile.md` 2. **Killed on reason 2, and it is a pre-specified test rather than a question.** The strategic version — what is stopping the brand from replying at all — is brand-routed as E2. Once that is answered, this becomes a test design for the hypothesis stage, not a loop.

**9. What happens to this account's cost per lead when its proven message runs as a static?**
Raised by `biweekly-iterations-report.md` 2. **Killed as a pre-specified test.** `creative-strategy-fundamentals.md` is explicit that naming the test is media-buyer work and the honest loop is the question the test would answer. That question is brand-routed as C1: what made the team stop. Once C1 is answered, this is the hypothesis, and it is a good one.

**10. How much of the cost gap between the formats that hold attention and the POV ads is explained by spend level rather than by the creative?**
Raised by `90-day-diversity-audit.md` 7. **Killed on reason 1 — the answer is obvious and the doc supplies it.** All three high-hold formats sit under $2,100 in spend, which the audit itself notes is thin enough that a handful of leads swings the number. The claymation ad holding 13.59% brought 12 leads; the silent bedroom montage holding 3.28% brought 1,934. That is a denominator problem, not a finding. Folded as evidence into the promoted measurement loop.

**11. What is Meta seeing in the low-hold formats that the hold-rate numbers do not show?**
Raised by `90-day-diversity-audit.md` 1. **Killed on reason 3 — domain knowledge resolves it.** Meta optimises delivery toward the conversion event it was given, which for this account is a lead, not watch time. A format can hold badly and still be the cheapest way to a form fill. `andromeda-v2.md` and `ad-account-analysis.md` both cover this. Folded as evidence into the promoted measurement loop, which asks the question that is actually open: what this account should be measuring instead.

---

## Movement since the prior roll-up

There is no prior roll-up. This is version 1, so everything here is opening movement rather than change.

### Closed — five loop instances answered by evidence already in the vault

These were live questions in the documents that raised them and are settled by later evidence in the same build. They are recorded as closed rather than archived, because the answer exists.

**1. What happens to this brand's cost per lead and lead volume during an Open Enrollment window?**
Raised by `90-day-performance-audit.md` 7 (2026-09-03), which noted the account history contained no prior Open Enrollment. **Answered.** The account did ramp for OE 2025: spend went **$17.4K in September to $21.7K in October to $34.2K in November**, CPM rose **31.6%**, CTR rose **41.3%**, and cost per lead moved only **6.6% — $12.27 to $13.08**. November was the largest lead month of 2025. So rising competition raised the price of impressions and rising intent paid for it, almost exactly offsetting. That is the answer to the question as asked. What replaced it is sharper and is promoted as Personas 3: November behaved as the category predicts and December did the opposite, so the live question is what changes between the two halves of the window, not whether the window works.

**2. Is the quiz destination leaking?**
Raised in three places as a landing-destination anomaly. **Answered, and it was a misattribution.** The break is **`go.healthformoms.co`** at a **9.1% landing rate and a $273.23 cost per lead**, not the quiz. The quiz destination is essentially unmeasured, carrying **$138.27 lifetime**, which is far too little to conclude anything about. The corrected finding is logged in `prompts-run-log/`. The operational item that survives is archived above as kill 1 and routed to the operational owner as urgent — so this closure corrects a premise rather than retiring a loop, and its three loop instances are counted under that kill, not here.

**3. Has this brand ever run statics?**
Three separate 90-day audits state that this account has never run a static, and `90-day-diversity-audit.md` 2 built a loop on it. **Answered and the premise was wrong.** A lifetime pull returned **529 static ads, $168,907.73 and 13,735 leads at a $12.30 cost per lead** — 22.7% of lifetime spend and 34.7% of lifetime leads — dormant for 180 days rather than never run. This changes the shape of the question completely: statics are production-proven dormant capacity, not an untested idea, which is why the surviving loop is brand-routed as C1 (why they stopped) rather than a test of whether they work. Two loop instances closed on this premise.

**4. How much of the account's budget could move to newly launched creative before its cost per lead starts rising?**
Raised by `90-day-performance-audit.md` 4 (2026-09-03). **Largely answered inside the build.** `monthly-performance-report.md` (2026-09-03) records that the share moved from **26.6% to 47.4%** and the new cohort came in about **$7 cheaper per lead** — 85 ads made inside August took 47.4% of spend at $17.28 clean, against five carryover ads at 52.6% and $24.26. The ceiling has not been found, but the question as asked has an answer and the account is still moving in the right direction.

**5. What are moms hearing in the first five seconds of the ads that still hold them?**
Raised by `90-day-performance-audit.md` 3 (2026-09-03). **Closed because its premise reversed.** The monthly report found that in August the high-hold ads were the expensive ones, which inverts the assumption the loop rested on — that holding people longer is the lever on lead cost. The live question that replaced it is promoted as Messaging 6 and Messaging 8.

### Reading flags for the next cycle

**The competitor branch is deferred and it left two territories artificially thin.** `competitive-landscape.md` deliberately left Personas and Creators and talent empty, not because they were clean, but because with no rival libraries there is no competitor casting or targeting to read. Every external audit cut was skipped with it. Add competitors in the Parker app and this roll-up gains a whole class of loops it currently cannot raise — which matters most for the empty-lane loop promoted as Product 1, whose answer would sharpen considerably against real rival behaviour.

**`brand-profile-narrative.md` landed mid-pass.** It was written at 18:52 on 2026-09-04, after this harvest ran, and carries no open-loops tail yet. Its opening read was used for the Novelty check and it corroborates every Tier 1 finding here, but it was not harvested. Check it first on the next roll-up.

**The fidelity-review backlog is still open.** The build ledger, archived at `prompts-run-log/BUILD-STATUS-final-2026-09-04.md`, records eighteen reviews in flight and names the review gate as hard. Two cross-document errors have already reached documents through that gap and both are recorded as closures above — the Open Enrollment history and the quiz destination figures. Both were caught by a later prompt reading a live source rather than by review. Every score in this roll-up inherits whatever else is still sitting unreviewed in that stack.

**The Parker MCP is disconnected.** No live pull ran in this pass and no past Parker conversation was read fresh. Reconnecting it is what makes the next roll-up a refresh rather than a rebuild, and it is a prerequisite for every Tier 1 loop above.

### Coverage check

All four territories produced surviving loops, so none is named clean this pass. The distribution is worth watching rather than correcting:

| Territory | Shipped | Tier 1 | Tier 2 | Brand-routed |
|---|---|---|---|---|
| Personas | 14 | 3 | 8 | 3 |
| Product | 13 | 2 | 3 | 8 |
| Messaging | 26 | 8 | 12 | 6 |
| Creators and talent | 4 | 1 | 1 | 2 |

Messaging is the largest, which the rubric predicts for the broadest and most observational territory. **Creators and talent at four is the number to watch.** It is thin partly for an honest structural reason — four of its upstream loops asked who is credible on camera, which is the same fork as the proof question and collapsed under Messaging — and partly because the competitor branch that would have supplied rival casting reads is deferred. It is not clean. Treat it as under-read for the next cycle.

**Product is where the brand-routed cohort concentrates**, eight of thirteen, which is the honest signature of a lead-generation business whose entire second half sits with partner agencies Parker cannot reach.

### Accounting

| | |
|---|---|
| **Collected** | 212 loops, from 47 documents |
| **Closed on evidence already in the vault** | 5 |
| **Killed on the verdict template** | 13 (11 written verdicts; the `go.` kill absorbs 3 instances) |
| **Consolidated into survivors** | 137 |
| **Shipped** | 57 |
| — Tier 1, promoted | 14 |
| — Tier 2, backlog | 24 |
| — Brand-routed | 19 |

Attrition from 212 to 57 is 73%, above the "roughly half" the rubric expects. Almost all of it is consolidation rather than killing, which is the right shape for a first pass across 47 documents written in parallel by agents who could not see each other. The convergence they produced is the finding, not the noise: ten documents independently arrived at the lead-quality gate, nine at the persona-provenance problem, nine at the recognition-versus-argument split, seven at the coverage-is-luck belief. Where that happened it is recorded on the loop, because three documents raising the same question is evidence of importance rather than repetition.

**Routing files.** The per-loop files in `promoted/2026-09/` and `archived/2026-09/` were not written this pass, by instruction — the deliverable named for this node was this single roll-up. Every promoted loop above carries its full four-part form, its score line, its consolidation trail and its as-of dates, so it stands alone as the input the hypothesis prompt needs. Split them out at the next pass if the pipeline wants the directory structure.

**What this feeds.** This is the bridge into Phase 2. The four strategy inputs each have their territory section waiting: `persona-strategy-input.md` takes the fourteen Personas loops, `product-priority.md` the thirteen Product loops, `messaging-strategy-input.md` the twenty-six Messaging loops, and `creator-talent-strategy-input.md` the four here — with the honest caveat that the last of those is thin and under-read. The strategic roadmap they synthesize into should be built knowing that nineteen of the questions underneath it can only be answered by a conversation with the team, and that six of those nineteen are one conversation with the partner agencies.

---

This is everything I know about seasonality in creative.

This is everything I know about advertising to older audiences.

This is everything I know about Andromeda v2.
