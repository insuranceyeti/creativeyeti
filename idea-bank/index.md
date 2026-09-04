---
brand: health-for-moms
brand_id: aed0ff06-555d-4f4f-9bf8-31178e2fb977
doc: idea-bank-index
phase: 3
generated_on: 2026-09-04
refresh_by: none. The idea bank is always-on and captured continuously rather than refreshed on a calendar, per `parker-system/system/refresh-cadence.md`. It goes stale by dependency instead: when the strategic roadmap changes, the bank gets re-graded by `/evaluate-ideas`.
run_type: "Phase-3 backfill on a freshly built brain. The backfill branch of parker-system/prompts/ideas-and-briefs/brand-idea-bank.md, run against the whole existing vault rather than against a week's fresh feeds."
entries_written: 20
corpus_denominator: "The Facebook and Instagram ad comment corpus is 1,342, re-pinned live 2026-09-04 with the Parker MCP. Counts carried from docs generated 2026-09-03 sit on 1,322 and say so at every use."
live_pulls_run_on: "2026-09-04. Five Parker MCP calls were made in this pass rather than carrying everything from the vault: search_chat_history in listThreads mode twice (17 threads across web and Slack), search_chat_history in getMessages mode on three threads, search_facebook_ad_comments_sql sorted by like_count for the top 30 rows, two keyword comment sweeps (paycheck, self pay), and search_tiktok_videos twice for all 23 library rows with live engagement counts and viewable links."
sources_read:
  strategy: "strategy/strategic-roadmap.md (2026-09-04, status drafted and awaiting review, approved_by null), persona-strategy-input.md, product-priority.md, messaging-strategy-input.md, creator-talent-strategy-input.md."
  sub_context: "sub-context-docs/brand-profile-narrative.md read in full; brand-identity-analysis, website-and-product-audit, category-and-market-research, competitive-landscape, reputation-analysis, marketing-calendar-and-campaigns, community-and-forums, operations-and-team, visual-vocabulary, ad-account-evaluation, performance-targets-and-metrics, organic-channels-inventory read for the specific figures cited."
  personas: "personas/personas-profile.md (all three identity blocks read in full), persona-voice-library.md, lifecycle-journey-maps.md, cross-persona-bias-notes.md, and the eleven voice-of-customer files. voc-metaphor, voc-pain-phrase, voc-trigger-moment, voc-objection, voc-anti-language, voc-category-jargon, voc-aspirational, voc-outcome-phrase and voc-surprise-delight were mined snippet by snippet."
  source_pulls: "source-pulls/ad-comments.md as the denominator source; customer-reviews, post-purchase-surveys, other-reviews and reddit read as the four named blanks; brand-reputation and brand-self-echo-detection for the echo verdicts carried here."
  audits: "audits/2026-Q3 — gaps-opportunities-inspo, quarterly-whitespace-analysis, 90-day-creative-strategy-audit, 90-day-diversity-audit, 90-day-performance-audit, customer-review-audit. audits/2026-09 — monthly-hook-audit, monthly-organic-tiktok-audit, monthly-tiktok-mining, monthly-performance-report, biweekly-iterations-report, weekly-performance-snapshot."
  loops_and_notes: "open-loops/open-loops-roll-up.md, hypotheses/2026-09-04-go-subdomain-measurement.md, validations/2026-09-04-go-subdomain-measurement.md, running-notes/brand-rules.md, success-definition.md, missing-context.md."
  team_conversations: "Parker chat history, 17 threads across 1 web account and 1 Slack channel, 2026-09-03 to 2026-09-04. Four threads produced material: the TikTok inspiration search brainstorm, the Ethos life-insurance ad adaptation, the reaction-script thread, and the intake message confirming there are no reviews. Two entries in this bank come from that surface."
knowledge_docs_read:
  - "parker-system/creative-strategy-context/expertise-routing.md — the routing map for this doc type. Not a reasoning doc, carries no sign-off."
  - "parker-system/creative-strategy-context/ideation-and-brainstorming.md — read in full. The capture-is-a-transfer rule, the spark and its articulation test, the hunt lanes, the freshness bar that keeps the brand's own known assets out, and the idea/concept/brief split. No sign-off line exists in this doc, so none is stamped."
  - "parker-system/creative-strategy-context/hooks.md — the format taxonomy, read in full at the Permission/Zone 1 and Comparison sections and at the format list. No sign-off line exists in this doc, so none is stamped."
  - "parker-system/creative-strategy-context/emotional-delivery-and-timing.md — read in full. The valence and intensity read, the landing-state rule, and TEEP, which decides where several entries place the buyer. No sign-off line exists in this doc, so none is stamped."
  - "parker-system/creative-strategy-context/creative-consumption-analysis.md — read in full. It is the method the far-transfer lane entry hands off to. No sign-off line exists in this doc, so none is stamped."
  - "parker-system/creative-strategy-context/iterations.md — read at Step Zero, the optimization hierarchy, the signal-change ladder and the highest-confidence iteration list. Its stamp is carried at the foot of this doc."
  - "parker-system/creative-strategy-context/scriptwriting.md — read at the core philosophies and hook sections. No sign-off line exists in this doc, so none is stamped."
  - "parker-system/creative-strategy-context/advertising-to-older-audiences.md — read in full, and it governs two entries. Stamped at the foot of this doc."
  - "parker-system/creative-strategy-context/static-ad-design.md — read in full. Hierarchy, the money shot and message-image congruency sit under the colour-comparison entry. Stamped at the foot of this doc."
  - "parker-system/creative-strategy-context/seasonality.md — read at the shifts-underneath and layer-do-not-swap sections. Stamped at the foot of this doc."
  - "parker-system/creative-strategy-context/creative-strategy-by-brand-size.md — read in full, and it shapes the starving-for read at roughly $42.7k a month. Stamped at the foot of this doc."
  - "parker-system/creative-strategy-context/old-ads/README.md and INDEX.md — read. The corpus holds zero entries."
knowledge_docs_not_stamped: "creator-briefs.md carries a required sign-off and was read, but no entry here rests on it, because briefs are downstream of this bank. It is not stamped, since stamping a doc that did not shape the output would be false. non-problem-solution-creative.md and algospeak.md also carry sign-offs and were not opened in this run."
data_limitations:
  - "This is lead generation with zero purchase events. Every read here is cost per lead and lead volume. ROAS, AOV, add-to-cart and purchase value appear nowhere, per running-notes/brand-rules.md."
  - "Gate two is invisible. The brand's winner definition has two gates, cost per lead then lead quality, and gate two lives with the partner insurance agencies. No idea in this bank is called a winner and no cheap lead here is called a good one."
  - "One first-party language surface. Customer reviews and post-purchase surveys are verified empty, Reddit is unreachable, and author_name is null on all 1,342 comment rows. Eight of the twenty entries rest on comments under the brand's own paid ads. Every persona claim caps at mixed."
  - "No competitor read. Ethos is the only tracked external brand and it sells term life, not health coverage, so it is an affinity reference. Nothing here says whether an idea's lane is empty because it is valuable or empty because somebody already tried it."
  - "The old-ads corpus at parker-system/creative-strategy-context/old-ads/entries/ holds zero files, and the live web archives the corpus README names as the fallback are mostly unreachable from this environment: repository.duke.edu, www.ebay.de and adretro.com are all blocked by the network egress proxy. The historian lane produced one data-limited entry and two retrieval leads instead of real captures. This is a tooling gap, not a judgment call."
  - "The TikTok mining library is a fixed scrape of 23 videos taken 2026-09-03 from one keyword set of 18 phrases, and no fresh TikTok keyword search can be run from this environment. So there is no live trend lane in this bank, and the seven organic entries all come from that frozen pool."
  - "strategy/strategic-roadmap.md carries status: drafted, awaiting review and approved_by: null. It has NOT been approved by the brand. Every entry that references it says so. Nothing in this bank should be read as authorised direction."
  - "No human strategist has reviewed any doc in this stack. The whole vault this bank was mined from is model-generated from Parker pulls plus the brand's own intake."
---

# Idea bank index — Health For Moms

Twenty ideas, captured 2026-09-04 in a backfill of everything this brain already holds. Each one is a source-backed thing a strategist could go act on, and none of them is a plan.

**Read the four standing constraints in `README.md` before you read a single number here.** The short version: this account is lead generation, so every figure is cost per lead; the only first-party language surface is comments under the brand's own paid ads; no competitor is tracked; and a winner needs two gates while Parker can only see one.

**And one labelling note that applies everywhere.** `strategy/strategic-roadmap.md` is **drafted and awaiting review. The brand has not approved it.** Several entries point at directions that roadmap also names. That agreement is not authorisation.

---

## The bank

| # | Concept | Source type | Winning elements | Awareness | Status | Source path |
|---|---|---|---|---|---|---|
| 1 | [You do not have to take your job's plan](entries/2026-09-04-you-dont-have-to-take-your-jobs-plan.md) | customer language | angle, hook, offer frame, headline | unaware | worth testing | `personas/personas-profile.md`, `audits/2026-Q3/gaps-opportunities-inspo.md` |
| 2 | [The correction economy](entries/2026-09-04-the-correction-economy.md) | customer language | proof, angle, creator, comment mechanic | most aware / solution aware | worth testing | `personas/voice-of-customer/voc-objection.md` |
| 3 | [The worst number wins](entries/2026-09-04-the-worst-number-wins.md) | customer language | comment mechanic, hook, angle, emotional frame | problem aware | worth testing | `personas/voice-of-customer/voc-pain-phrase.md` |
| 4 | [The paycheck that came back empty](entries/2026-09-04-the-paycheck-that-came-back-empty.md) | customer language + organic | hook, visual, trigger moment, pacing | problem aware | worth testing | `audits/2026-09/monthly-organic-tiktok-audit.md`, live comment pull |
| 5 | [Coverage is luck, not a choice](entries/2026-09-04-coverage-is-luck-not-a-choice.md) | customer language | emotional frame, angle, hook | unaware / problem aware | raw idea | `personas/voice-of-customer/voc-metaphor.md` |
| 6 | [Legal scam, forced scam](entries/2026-09-04-legal-scam-the-qualifier.md) | customer language | headline, hook, angle, emotional frame | problem aware | raw idea | `personas/voice-of-customer/voc-metaphor.md` |
| 7 | [Still a mom when they're grown](entries/2026-09-04-still-a-mom-when-theyre-grown.md) | customer language | angle, headline, hook, creator | problem aware | raw idea | `personas/voice-of-customer/voc-objection.md` cluster nine |
| 8 | [January first, and it all starts over](entries/2026-09-04-january-first-it-all-starts-over.md) | customer language | trigger moment, angle, hook, offer timing | problem aware | raw idea | `sub-context-docs/marketing-calendar-and-campaigns.md` |
| 9 | [The real call, not the skit](entries/2026-09-04-the-real-call-not-the-skit.md) | organic video | format, hook, proof, visual, pacing | problem / solution aware | worth testing | `audits/2026-09/monthly-tiktok-mining.md` |
| 10 | [Red against green](entries/2026-09-04-red-against-green.md) | organic video | visual, format, headline, proof | solution aware | worth testing | `audits/2026-Q3/gaps-opportunities-inspo.md` opening 3 |
| 11 | [The flat confession](entries/2026-09-04-the-flat-confession.md) | organic video | hook, pacing, emotional frame, format | unaware / problem aware | worth testing | `audits/2026-09/monthly-hook-audit.md` |
| 12 | [The pinned comment, answered out loud](entries/2026-09-04-the-pinned-comment-answered-out-loud.md) | organic video | comment mechanic, format, hook, proof | solution / most aware | worth testing | `audits/2026-09/monthly-organic-tiktok-audit.md` |
| 13 | [A hill I will die on](entries/2026-09-04-a-hill-i-will-die-on.md) | organic video | hook, format, creator, pacing, emotional frame | unaware / problem aware | raw idea | `audits/2026-09/monthly-hook-audit.md` |
| 14 | [The second task that frees the eye](entries/2026-09-04-the-second-task-that-frees-the-eye.md) | organic video | format, pacing, visual, creator | format agnostic | raw idea | `sub-context-docs/visual-vocabulary.md` |
| 15 | [The faceless bill pan](entries/2026-09-04-the-faceless-bill-pan.md) | organic video | visual, format, hook, proof | problem aware | raw idea | `audits/2026-09/monthly-organic-tiktok-audit.md` |
| 16 | [Mom mental load as the format source](entries/2026-09-04-mom-mental-load-as-the-format-source.md) | user conversation | format, creator, angle, emotional frame | unaware | worth testing | Parker chat history, Slack thread `1788538777.074209` |
| 17 | [The heavy line over a mundane task](entries/2026-09-04-heavy-line-over-a-mundane-task.md) | inspiration ad (affinity) | hook, visual, format, pacing, offer framing | problem aware | raw idea | Parker chat history, web thread `7edd320e-3e00-4dd9-a3c4-268b3936102b` |
| 18 | [You did everything right](entries/2026-09-04-you-did-everything-right.md) | cold-brainstorm | hook, emotional frame, angle | problem aware | raw idea | `personas/personas-profile.md` Persona 1 |
| 19 | [A number I can plan against](entries/2026-09-04-a-number-i-can-plan-against.md) | cold-brainstorm | angle, offer framing, headline | solution aware | raw idea | `personas/personas-profile.md` Persona 3 |
| 20 | [One family in every seven](entries/2026-09-04-one-family-in-every-seven.md) | old-ad-corpus | headline | unaware / problem aware | raw idea | `parker-system/creative-strategy-context/old-ads/INDEX.md` (empty) |

Nine are marked **worth testing** and eleven **raw idea**. Nothing is adapted, used, rejected or stale yet, because this is the bank's first day.

## Where the ideas came from

| Source surface | Entries | What it gave |
|---|---|---|
| Customer language, meaning commenters under the brand's own paid ads | 8 | The counter-bid, the luck frame, the scam qualifier, the correction economy, the permission sentence, the grown-kids question, the paycheck moment, the January reset |
| Organic video, the 23-video TikTok mining library | 7 | The real phone call, the colour ledger, the flat confession, the pinned comment, the unfinished-sentence hook, the second task, the faceless bill |
| User conversations with Parker | 2 | The mental-load far-transfer lane, and the Ethos reference the team asked to adapt |
| Parker's own cold pass | 2 | The permission line, and predictability as a promise |
| Old print ads | 1 | One headline mechanic, and it is data-limited |
| Competitor paid ads | 0 | Nothing is tracked. Ethos is affinity, not a rival |
| Reviews, surveys, Reddit, community | 0 | Verified empty or unreachable |

## Lane coverage, and what this bank is starving for

The `hunt_lane` field on every entry makes this readable. What it says about the backfill:

**Customer language is the deepest lane and it is one surface deep.** Eight entries, all from the same comment corpus, and six of the eight cluster inside one creative family and one spring. `personas/voice-of-customer/voc-pain-phrase.md` is blunt about it: 197 of the 207 "deductible" comments land inside an 83-day window that starts the day the `MOMS38` creative went live. That is a compliment to the creative and a warning about the corpus. The bank is rich in her language and poor in *unprompted* language.

**The historian lane is essentially empty and it is the biggest hole.** One data-limited entry. The shipped corpus holds zero files and the archives are blocked from this environment. `parker-system/creative-strategy-context/ideation-and-brainstorming.md` calls old print ads the gold mine and the highest-value source Parker can have, precisely because nobody else in a category is mining it. This brand has a static library that already proved out and no historical reference to build the next one from.

**The trend lane does not exist.** The mining library is a frozen scrape from 2026-09-03. There is no live read of what moved in this space this week, so nothing here is fresh in the way a trend keeper is meant to be.

**Far transfer got one lane and no videos.** Entry 16 defines the lane and does not contain a single reference from it, which is honest but thin. The method asks for two or three unrelated categories per hunt, rotated and logged. This backfill ran one, and it came from the client rather than from Parker.

**Creators and talent is the thinnest territory of all.** Only two entries touch casting, and the account has found an audience the category's own feed cannot supply a reference for. That is loop 3 below.

**What the bank is heavy on:** documents. Five of the twenty put a bill, a stub, a screen or a ledger in frame. That is a real bet on one device, and the account's only proven version of it buys the cheapest clicks in the file and converts them worst among real spenders. Read entries 4, 10 and 15 together before anyone decides how much of a round goes to paper.

**What it is light on:** anything that is not the problem. `personas/voice-of-customer/voc-metaphor.md` found that all fifteen images in the corpus are about the problem, and this bank inherits that shape. There is almost nothing here about what life looks like after. That may be right for a brand in this state, and it should be a choice rather than an accident.

**One read from spend level.** At roughly $42,700 a month this account sits in the middle band, where `parker-system/creative-strategy-context/creative-strategy-by-brand-size.md` says two things matter most: reaching genuinely new audiences rather than sweeping up existing demand, and checking what you think you know about the customer, because brands at this size are often confidently wrong about who is buying. This whole bank is an argument that the second one has already happened here.

---

## Open loops

Four questions this pass left behind. Each is about the *bank* rather than about the account, and each could change which ideas get built rather than how they get built.

**1. Thirteen of the twenty ideas here came out of a comment section the brand has never once posted in.**

The comment threads produced the counter-bid, the luck frame, the scam qualifier, the correction economy, the permission sentence and the grown-kids question, and they are the raw material behind the pinned-comment format too. In 1,342 comments over twenty months the brand has never replied. Meanwhile rival brokers answer in its place, 39 poaching comments across 10 ads.

*Pull: Gap.* It fired because there is an enormous amount of usable material in one place and nothing has ever been done with it, in the single surface where this brand's audience is already talking to it directly.

*Question: What happens in these threads when the brand answers?*

*Why it matters:* if replying changes the shape of what people say next, then the comment section is a creative input the brand can steer rather than only mine, and several ideas in this bank get cheaper and better evidenced at the same time. If it changes nothing, the threads stay a read-only research surface and the effort belongs in production instead.

*Territory: Messaging.*

**2. Every idea here that names a dollar figure gets bid up, and every idea that names an experience gets agreed with.**

The account's numbers get answered with bigger numbers: 82 of 1,342 comments open with "mine is," and 84% of the figures beat the ad's. The one creative family that earned recognition instead of argument is the phone skit, where roughly 12 clear recognitions sit, including "'It's out of network' 'But it's in the same building!' 'In a different hallway' whoever came up with this ad deserves a raise!!"

*Pull: Pattern.* It fired because the same split keeps showing up across independent audits and across every entry in this bank, which is what a real behaviour looks like rather than a coincidence.

*Question: What can this account put on screen that she cannot answer with a bigger number?*

*Why it matters:* it sorts this bank into two piles. If the answer is experiences and moments, then entries 3, 4, 9 and 11 rise and anything that leads with a figure drops, including the account's current top of funnel. If figures work when they are framed differently, the sorting is wrong and a lot of cheap capture gets thrown away for no reason.

*Territory: Messaging.*

**3. The one buyer this bank keeps pointing at is a woman the category's own creators cannot supply a single reference for.**

Four entries lean toward a woman 45 and over or toward the calm register she responds to. Meta's delivery finds her without anyone aiming at her, at 21.2% of lifetime spend and falling to 16.2% last quarter. And of the 19 relevant videos in the whole mining library, exactly one creator reads as over 40 and **zero** read as over 45.

*Pull: Tension.* It fired because two instruments this brain trusts cannot both be a fair picture: the account keeps finding her, and the feed she supposedly lives in contains nobody who looks like her.

*Question: Where does this brand find the woman who is 45 and over, if the feed her buyer watches does not contain her?*

*Why it matters:* the brand names casting and creator sourcing as its number one creative bottleneck. If the reference pool for her genuinely does not exist on this surface, then every idea in this bank aimed at her needs a different sourcing route before it can be produced, and the ones aimed at the 25 to 44 band should be built first.

*Territory: Creators and talent.*

**4. A quarter of this bank puts a document in frame, and the account's one document ad buys the cheapest clicks in the file and converts them worst.**

`moms-53 3` holds the account's best click through rate at 3.15% and the cheapest link click in the file, and then turns 5.97% of those clicks into leads against `moms-63 2b`'s 12.25% in the same window.

One thing worth flagging while it is in view, because it is a conflict inside the vault rather than a finding. **Three docs give three different costs per link click for this same ad**: $0.69 in `sub-context-docs/brand-profile-narrative.md`, $0.96 in `strategy/strategic-roadmap.md` in two separate places, and $0.67 in `audits/2026-09/monthly-hook-audit.md`.

**RESOLVED 2026-09-04 by a live pull, and it is not a data error — it is two different metrics wearing one label.** `verified live`, `search_facebook_ads_sql`, ad `120247254787160519`, window 2026-06-06 to 2026-09-03, Meta default attribution.

Over that 90-day window `moms-53 3` spent **$2,041.42** and bought **2,962 clicks but only 2,127 link clicks**. Those are different denominators, so they give different answers on the same money:

- **Cost per click, all clicks: $0.69.** Matches `brand-profile-narrative.md` exactly. The lifetime figure is $0.68, which is almost certainly what `monthly-hook-audit.md` read as $0.67 when it pulled one day earlier.
- **Cost per *link* click: $0.9598.** Matches the roadmap's $0.96 exactly, in both places.

So all three docs were right and none of them was talking about the same thing. The gap is real: **28% of this ad's clicks are not link clicks** — they are likes, comments, shares, profile taps and expands. **Use cost per link click ($0.96) whenever the question is what it costs to get someone to the site, which is nearly always the question here.** Cost per click flatters the ad by counting engagement the brand cannot convert. No doc needs correcting; each should say which metric it means.

**And the pull turned up something nobody had recorded.** The sibling group `moms-53 3 - Copy` (three variants, $497.42 across the window, `ADSET_PAUSED` today) points at **`quiz.healthformoms.com/#/indvfam`** and returned **9 landing page views against 511 link clicks** — a click quality of **1.76%**, against **76.12%** on `moms-53 3` itself, which points at `www.healthformoms.co/save/`. Same creative, same hook, same body copy, different destination, and one of them essentially registers no arrivals.

**The honest reading, stated as two possibilities because the data cannot separate them:** either almost nobody who clicks actually lands on the quiz, or they land and the pixel does not fire on that domain. Both are urgent and neither is a creative problem. This is the same shape as the `go.healthformoms.co` break the roll-up routed to the operational owner, on a different destination. `verified live`, 2026-09-04. **Do not build a brief on any figure sourced from a `quiz.healthformoms.com` ad until this is settled.**

*Pull: Surprise.* It fired because the device this bank leans on hardest behaves in exactly the opposite direction to what every craft doc would predict, on the account's own money.

*Question: Who is the person who stops for a document in this account and then does not fill in the form?*

*Why it matters:* five entries here rest on paper. If the document is recruiting a browser rather than a buyer, those five are attention ideas rather than lead ideas and they should be graded that way. If it is the state list specifically that turns people away, then the device is fine and the content of that one document is the problem.

*Territory: Personas.*

**Product is genuinely clean at the bank level and is left empty rather than filled.** The product questions this pass ran into — what a lead is worth, why the statics stopped, what "up to 30%" compares against — are already graded and routed to the brand in `open-loops/open-loops-roll-up.md`, and restating them here would be noise.

---

## Sign-offs

This is everything I know about advertising to older audiences.

This is everything I know about static ad design.

This is everything I know about seasonality in creative.

This is everything I know about tailoring creative strategy to brand size.

This is based on everything I have learned about making iterations 2.0
