---
brand: health-for-moms
brand_id: aed0ff06-555d-4f4f-9bf8-31178e2fb977
doc: product-priority
generated_on: 2026-09-04
refresh_by: 2026-10-15
status: provisional
status_note: "Provisional because the deciding economics are not brand-confirmed. No revenue per lead, no revenue model (per lead or per policy), no renewal terms, and no lead-quality data exist anywhere in this brain. The call below is built on gate one plus a gate-two inference, and the exact number that would confirm or overturn it is named in 'Confidence and what would raise it'."
refresh_note: "Cadence for the four Phase-2 strategy inputs is 90 days per parker-system/system/refresh-cadence.md, which would put this at 2026-12-03. Pulled forward to 2026-10-15 because two refresh triggers have already fired: Open Enrollment opens 2026-11-01 and this call is meant to govern that ramp, and a second funnel destination (quiz.healthformoms.com) went from 26 ads to 30 and grew a second path in the 24 hours before this doc was written."
sources_read:
  - "Live Parker MCP pulls run 2026-09-04 for this doc: search_facebook_ads_sql lifetime filtered to static (grouped by name), lifetime filtered to video, static filtered to last_180d, a 90-day efficiency ranking at a $1,000 spend floor, a last_7d account cut, an ad-level lifetime cut filtered to landing_url contains 'quiz.', and an ad-level lifetime cut filtered to landing_url contains 'go.healthformoms'"
  - "Parker MCP list_custom_metrics, run 2026-09-04: four auto-detected pixel events, zero formulas"
  - "Parker MCP search_facebook_ad_comments_sql, four substring counts run 2026-09-04: 'pregnan', 'existing', 'qualify', 'deductible'"
  - "Parker MCP search_chat_history, run 2026-09-04: listThreads plus getMessages on two Slack threads dated 2026-09-04. This is a new source that no prior doc in this brain has read."
  - "sub-context-docs/website-and-product-audit.md (2026-09-03, carrying two 2026-09-04 corrections) — the funnel-surface map, the underwriting evidence, the five known product issues, the entry-point hypothesis this doc resolves"
  - "sub-context-docs/performance-targets-and-metrics.md (2026-09-04) — the cost-per-lead tiers, the two-gate winner definition, thirteen months of history, the lifetime static/video split"
  - "sub-context-docs/ad-account-evaluation.md (2026-09-04) — the account diagnosis and the nine findings"
  - "sub-context-docs/brand-profile-narrative.md (2026-09-04) — the whole-brand picture this call sits inside"
  - "sub-context-docs/organic-channels-inventory.md (2026-09-04) — the paid-only footprint and the unworked comment surface"
  - "sub-context-docs/customer-journey-and-persona-discovery.md (2026-09-03) — the two-half journey and the five buyer states"
  - "audits/2026-Q3/quarterly-whitespace-analysis.md (2026-09-04) — the lifetime per-lane spend map and the employer-plan finding"
  - "personas/lifecycle-journey-maps.md (2026-09-04) — the six-stage lifecycle variation and the critical transitions"
  - "open-loops/open-loops-roll-up.md (2026-09-04) — the graded loop set, the thirteen Product loops, the nineteen brand-routed questions"
  - "hypotheses/2026-09-04-go-subdomain-measurement.md and validations/2026-09-04-go-subdomain-measurement.md — the destination verdict this doc acts on"
  - "running-notes/success-definition.md and running-notes/brand-rules.md (2026-09-03) — the two-gate bar and the standing constraints"
knowledge_docs_read:
  - parker-system/creative-strategy-context/expertise-routing.md
  - parker-system/creative-strategy-context/creative-strategy-fundamentals.md
  - parker-system/creative-strategy-context/persona-research-and-creative-strategy-process.md
  - parker-system/creative-strategy-context/killer-performance-ads.md
  - parker-system/creative-strategy-context/ad-account-analysis.md
  - parker-system/creative-strategy-context/customer-review-mining-method.md
  - parker-system/creative-strategy-context/andromeda-v2.md
  - parker-system/creative-strategy-context/static-ad-design.md
  - parker-system/creative-strategy-context/seasonality.md
  - parker-system/creative-strategy-context/creative-strategy-by-brand-size.md
knowledge_docs_note: "Of the ten, four carry a required sign-off line and all four are stamped at the foot of this document: andromeda-v2, static-ad-design, seasonality, creative-strategy-by-brand-size. The other six carry none. advertising-to-older-audiences.md was deliberately not loaded this run; the call below does not rest on an older-audience read, and stamping it would be a false proof-of-read."
corpus_denominator: "The Facebook and Instagram ad comment corpus is 1,342 as of 2026-09-04. Docs generated 2026-09-03 ran on 1,322 and keep that denominator where their counts are carried. Both are labelled at every use."
data_limitations:
  - "No unit economics. No revenue per lead, no gross margin, no lifetime value, no payback window, no maximum tolerable cost per acquisition. Every use of the word efficient here is relative to this account's own trailing number, never to a profit line. This is why status is provisional."
  - "Gate two is dark. Lead quality lives with the partner insurance agencies. The `invitee_meeting_scheduled` pixel event returned no data and `Call` fired 42 times against 4,336 leads in the 90-day window. The gate-two argument in this doc is an inference and is marked as one everywhere it appears."
  - "The brand's own site has never been opened in any build session, including this one. The qualification questions, the state list, the income screen and the consent language are all named blanks."
  - "No competitors are tracked and no review corpus or post-purchase survey exists. Every customer verbatim here comes from comments under the brand's own paid ads. The honest sentence is always 'commenters under the brand's paid ads said,' never 'customers said.' Personas stay capped at mixed confidence."
  - "Reach and frequency are not returned for this account, so no saturation check can be run on any recommendation below."
  - "Northbeam is not connected. Every figure is Meta-reported on the Meta default attribution window. Nothing here is multi-touch."
  - "This is the first product-priority call for this brand. There is no prior version to carry forward and nothing here is a flipped call."
---

# Product priority — Health For Moms

## The frame, before the call

**This brand has no catalogue and no SKU, so the prompt's usual question does not apply and forcing it would invent a product line that does not exist.** Health For Moms sells nothing. A mother sees an ad, answers about four questions on a landing page, and her details go to a partner insurance agency where a licensed agent tries to enroll her in a private, medically underwritten plan. Lifetime the account has spent **$743,218.09 for 39,569 leads and exactly zero purchases**, by design. (`verified`, lifetime pulls run 2026-09-04.)

So "which product should we lead with" maps onto four real decisions this brand actually gets to make:

1. **Which offer** opens the relationship. The savings number, or something else.
2. **Which funnel destination** the money points at. There are three live and they behave nothing alike.
3. **Which qualification path** the buyer walks, and how early the gate becomes visible to her.
4. **Which format** carries the offer, because in this account the format turns out to be an economic decision rather than a craft one.

Everything below answers those four. Where a section of the standard shape has no honest equivalent here, it says so rather than filling itself in.

## The call

**Lead with the switch, not the saving. Put the weight behind the mother who already has insurance through a job, tell her plainly that she is allowed to leave it, and carry that message as a static pointed at `www.healthformoms.co/save/`.**

That is one direction with four decisions inside it. Stated flat:

- **The offer is the permission, not the price.** Not "save $400 a month." The line the account has never said out loud is that she can decline the plan her employer offers and go buy her own. Right now a stranger in the comments teaches her that and the brand watches.
- **The format is static, and this is the load-bearing part.** Statics are not a new bet here. They are 308 ad-name groups, **$168,907.73 and 13,735 leads at a $12.30 cost per lead**, and they have been switched off for more than 180 days. (`verified`, two live pulls 2026-09-04, including a static-filtered `last_180d` cut that returned zero results.)
- **The destination is `www./save/`, and the four live `go.` ads should be switched off today.** Not next sprint. Today.
- **The qualification gate moves into the creative.** The brand told Parker on 2026-09-04 who it does not want. The account has never once said so to a buyer.

**The runner-up, and it is close.** Put the Approved State List in the first frame of the video half of the account, the way `moms-53 3` does. It earns the runner-up slot rather than the lead for a specific reason found in this run's pulls, and that reason is in "Alternatives considered."

**What this call costs.** It moves money away from the savings hook that currently carries most of the account. It restarts a production lane the team switched off in roughly March for a reason nobody wrote down. And it points the brand at the one buyer whose saving may be hardest to actually deliver, because employer premiums come out of payroll before tax and a private plan has to beat a discounted number. That last one is a real risk and it is a gate-two risk, which means nobody can currently see it. It is named in full below.

## Why — the economics

**Read the economics first, because they govern the call.** Here almost every economic that should decide this sits on the other side of a handoff Parker cannot see, so this section does two things: it uses the numbers that do exist honestly, and it marks the missing ones rather than inventing them.

### The modality split is the largest economic fact in this business, and it is bigger than the headline number suggests

Everyone in this brain has carried the static story as a cost-per-lead comparison: $12.30 against video's $22.23. That comparison is real and I re-verified it live today. But it can be argued with, because the static months and the video months are different months, different auctions and different seasons, so some of that gap could be the calendar rather than the format.

**So I ran the comparison on the one ratio that cannot be argued with, and the gap gets wider.**

The `go.` subdomain validation on 2026-09-04 established something the whole account should now be read through: **landing page views are an unreliable counter on this account, and `click_quality` is that same unreliable number wearing a second name.** What survived as trustworthy is leads divided by link clicks, because link clicks are counted on Meta's side of the boundary and leads are counted at the far end, and neither depends on the page-view pixel.

Run the modality split on that ratio, from today's pulls:

| Modality | Spend | Link clicks | Leads | Leads per link click | CPL | CPM | CTR |
|---|---|---|---|---|---|---|---|
| **Static** | $168,907.73 | 82,871 | 13,735 | **16.57%** | **$12.30** | $17.99 | 1.76% |
| **Video** | $574,310.36 | 312,052 | 25,834 | **8.28%** | $22.23 | $23.68 | 2.28% |

(`verified`, two lifetime pulls run 2026-09-04. 308 static ad-name groups against 1,259 video groups.)

**A static's click turns into a lead at exactly twice the rate of a video's click.** That is 16.57% against 8.28%, computed by hand from raw counts, on 82,871 and 312,052 link clicks respectively. Those are not thin denominators.

And look at the direction of the CTR, because it is the part that makes this a real finding rather than a flattering one. **Video buys more clicks per impression and statics buy better ones.** Video runs a 2.28% click-through rate against static's 1.76%, so video wins the click by 30%. Then it loses the lead by half. The account has been optimising toward the thing that wins clicks and away from the thing that wins form fills, and because cost per lead barely moves in this account no alarm ever went off.

Statics also buy impressions **24.0% cheaper**, $17.99 against $23.68. Read through the auction logic in `ad-account-analysis.md`, cheaper impressions plus a better conversion rate at the far end is the shape of a modality Meta finds easy to place and buyers find easy to act on.

### Inside the statics, one lane is the cheapest thing this account has ever bought

Two static ad-name groups carry the employer-plan message. Pulled live today, grouped by name:

| Ad | Headline | Spend | Link clicks | Leads | Leads per link click | CPL | CPM |
|---|---|---|---|---|---|---|---|
| `B1 - Copy 7` | *"Left my big insurance company for a mom-focused one. 24% cheaper and I choose my own doctor 😌"* | $30,339.32 | 11,845 | 2,584 | **21.82%** | **$11.74** | $15.89 |
| `B1 samar- Copy 1` | *"Didn't know I could ditch my job's health plan… until I did."* | $14,633.08 | 8,193 | 1,231 | **15.03%** | **$11.89** | $15.05 |
| **Together** | | **$44,972.40** | **20,038** | **3,815** | **19.04%** | **$11.79** | |

(`verified`, lifetime static pull grouped by name, 2026-09-04.)

A note on reconciliation, because the number moved. `audits/2026-Q3/quarterly-whitespace-analysis.md` reports this lane at $30,845.69 and 2,580 leads at $11.96. That figure used `B1 - Copy 7`'s single-ad row. My pull grouped by name and picked up all five of its variants, which is the fuller read. Both are honest; the name-group figures are the ones to carry forward, and they make the lane bigger and slightly cheaper than the audit had it.

**Three things about those numbers.**

Against the brand's own scoreboard, where under $15 is "fantastic" (`stated`, brand context, confirmed at intake), $11.79 is not just inside the top band, it is 21% below its ceiling. The account has been in the "meh" band for six straight months.

**19.04% leads per link click against video's 8.28% is a 2.30x gap**, and it is on the metric this brain has just finished proving is the trustworthy one. This is the strongest efficiency evidence in the account and until today nobody had computed it.

And the CPM is $15.89 and $15.05, the cheapest impressions in the whole library. This lane was not buying scraps. It was buying cheap attention that converted.

### What cannot be said, and why the call is provisional

**There is no ceiling, so nothing here can be called profitable.** No revenue per lead, no gross margin, no lifetime value, no payback window, no maximum tolerable cost per acquisition was ever captured. (`stated` as unanswered in `running-notes/brand-rules.md`.) So "cheapest" means cheapest against this account's own history, which is a real bar but not a business one.

**And the revenue model itself is unknown, which is the fork that decides everything.** If the brand is paid per lead delivered, this is a volume business and cost per lead really is close to the whole game, which is how the team has it set up. If it is paid per policy written, or on renewals, then lead quality is not a second gate at all, it is the first one, and the entire ranking of winners in this brain could invert. (`inferred` from the account shape and the absence of any revenue metric; `list_custom_metrics` returned four auto-detected pixel events and **zero formulas** and no revenue metric of any kind, re-verified live 2026-09-04.) **Brand-routed.**

**One live observation about gate two that nobody in this brain has made.** The four pixel events include `offsite_conversion.fb_pixel_custom.invitee_meeting_scheduled`. The word "invitee" is booking-tool language, so somewhere in this funnel there is or was a step where a mother schedules a call. It has returned no data at all. Either that booking step is dead, or the pixel sits on a page nobody reaches. (`verified` that the event exists and returns nothing; `inferred` on what it implies.) That matters here because it is the one gate-two instrument the brand already owns and it is not reporting. Turning it back on is a product decision, and it is cheaper than any conversation with a partner agency.

## Why — the journey

**The lead product is a starting point in a sequence, so read where the buyer enters and where the line stalls.** `personas/lifecycle-journey-maps.md` had to abandon the standard five-stage lens for this business and built a six-stage variation, and the reason is the whole strategic picture: **the brand can see stages one through four and stages five and six are completely dark.** Stage five is the agent's phone call. Stage six is whether she enrolled. Both happen at another company.

Three things in that journey decide this call.

**One. The employer-plan mother's blocker is a belief, and beliefs are the cheapest blockers to fix.** Every other buyer in this account is stopped by something the brand cannot move: a state list, an underwriting screen, a price nobody has named. She is stopped by not knowing a rule. The proof of that is who currently teaches her. Not the brand. A stranger in the replies, on 2026-05-05 under `MOMS38 - 1 - V2`: *"if it's an employer insurance, you don't have to sign up with that employer insurance you can decline the coverage and go out and find your own insurance carrier."* (`verified` verbatim, comment corpus.)

She says the blocker herself, flatly, over and over. *"nope. My job picks the plan that they offer,"* 2026-03-30 on `MOMS38 - 1 - V3`. *"Mine is $6k per person too but since it's thru my job I don't really have a choice,"* 2026-03-17 on `MOMS39 - 2 - V2`. *"The hospital I work for only provides the option to use their insurance company. Last year it was over 18k,"* 2026-03-28 on `MOMS38 - 1 - V3`. *"Mine is $9,200/individual, $17,500/family and that's the only plan my employer offers 😬,"* 2026-03-27 on `MOMS38 - 1 - V2`. (`verified` verbatims, carried from the whitespace analysis on the 1,322 denominator.)

Read against `killer-performance-ads.md`, that is a solution-aware buyer being sold at with a product-aware promise. She does not need the problem built. She has been carrying a five-figure deductible for years. She needs one fact she does not have.

**Two. She is the buyer most likely to survive the gate, and this is the part of the call that reaches into gate two.** Stack the screens this product is known to apply: a qualifying state, medically healthy, not pregnant or planning to be, and possibly above an income floor. Now hold the employer-plan mother against them. She is employed, so she clears an income floor by construction. She is on a group plan she can quote to the dollar, which is not the profile of a woman in acute medical crisis. She is not the pregnancy buyer and she is not the chronic-condition family, and those are the two groups the corpus shows getting turned away most.

**This is the heart of the call and I want to be exact about its status.** It is `inferred`, not verified, and it rests on the shape of who employer coverage selects for rather than on any enrollment data. Nobody can check it, because gate two is dark. But it is the one place in this whole account where gate one and gate two plausibly point the same way instead of opposite ways, and that is worth a great deal. Every other efficiency finding in this brain carries the worry that the cheapest lead might be the least qualifiable one. This one does not carry that worry as hard.

**Three. The journey has no second act, so there is no expansion path to protect.** There is no repeat purchase, no subscription, no second product and no returning buyer anywhere in this account. Lifetime, most-aware creative carries 0.1% of spend and unaware carries 0.0%. (`verified`, lifetime awareness cut.) That zero at the bottom is correct and should not be flagged as a hole, because there is nobody to retain. What it means for this call is that **every dollar is acquisition, so every product mismatch is an acquisition mismatch and there is no lifecycle story that rescues a wrong lead choice.**

## Why — the demand

**The swing often shows up in demand before anywhere else, so read where the pull already exists.** Three readings, and the third one is new to this brain.

**One. She recurs, unprompted, across ads and months.** The employer-plan comments above sit on at least five separate ad-name groups. That spread matters more than the raw count, because 60.1% of this corpus sits on one creative family and 64.0% falls in two months, so anything that appears across many ads is the durable signal. (`verified`, two independent counts in the whitespace analysis.)

**Two. The brand already knows employer coverage is its real rival and has never built for it.** The brand's own context document calls employer coverage *"the most common 'competitor' — the default option families already have."* (`stated`, brand context.) So the brand named the competitor, proved it could beat it for $11.79 a lead, and then stopped running the ads that did it.

**Three, and this is new evidence no prior doc in this brain has seen.** `search_chat_history` had not been run since the build; I ran it today. On 2026-09-04 the operator wrote in Slack, while setting up the TikTok inspiration library:

> *"I already deleted some like pregnant, and cant afford health insurance because we dont want broke people."*

(`stated`, Parker Slack thread `1788538777.074209`, 2026-09-04. The team's word, not a verified fact about the carrier's rules.)

**That single sentence resolves something ten documents in this brain had left open.** The income floor has been carried everywhere as thin evidence, two commenters independently naming $30,000, marked "route to the brand." The team has now effectively answered it, and it has also confirmed that pregnancy is a deliberate exclusion rather than an accident of targeting.

And it creates a sharper finding than the one it closes. **The brand has decided who it does not want, and the account has never told her.** No ad in this account's lifetime names a price, an income, or an eligibility rule before the click. In the comment corpus, **207 of 1,342 records mention "deductible" and 42 mention "qualify"** (`verified`, two live substring counts 2026-09-04), and in every one read the money on the table is the plan she already has. There is no record anywhere objecting to what Health For Moms costs, because nothing ever tells her.

So the demand read points one way. The buyer the brand says it wants is employed and not broke. The buyer with the cheapest verified leads in the account's history is a woman with a job and a group plan. **Those are the same woman, and nobody had put those two facts next to each other until now.**

**What the demand read also says, and it is a caution rather than an opportunity.** The two largest pools of demand in this category are the ones the product turns away. Pregnancy runs **38 of 1,342 comments** containing "pregnan" and pre-existing conditions **38** containing "existing" (`verified`, live counts 2026-09-04, both unchanged from the 1,322 reading, which means the twenty newest comments added none). Pregnancy is also 63.2% of the category's organic feed. Both carry the highest like counts in the corpus. Neither is a lead opportunity. Per the personas pass they are a **named recruitment cost**: the brand is paying to reach people it cannot sell to, and they go back to the comment section and say so under the ads that are working hardest. That is treated as a road not taken below, not as a swing.

## The size of it

**Size before you recommend.** A vector that is real but small is not the swing, so here is the arithmetic on both halves of the call, plus what it would take to actually reach it.

### The static lane

**The proven ceiling is $168,907.73 and 13,735 leads.** That is what statics have already delivered on this account, at 22.7% of lifetime spend and **34.7% of lifetime leads**. (`verified`.) So the modality is not a niche. At its own historical rate it was buying more than a third of this business's leads on less than a quarter of its money.

Size it against today's run rate rather than history. The account is running about **$17,698.33 a week** on the trailing seven days, at a blended **$25.58 cost per lead** across 77 delivering ad-name groups. (`verified`, live pull 2026-09-04.) If the static lane's own lifetime rate held, the same $17,698 would buy roughly **1,438 leads a week at $12.30** against roughly **692 at $25.58**. That is the shape of the prize and it is deliberately stated as a shape, not a forecast. It assumes a five-month-old rate holds in a more expensive auction, which is exactly the assumption a real test exists to break.

The honest discount on that number is the auction. Autumn 2025, when the statics ran, was a $14 to $18 CPM world; today's account runs $22.82 to $23.46. (`verified`, thirteen monthly pulls plus today's cuts.) So expect the gap to narrow. It does not need to hold fully to be the largest lever available: at even half the historical advantage this is the cheapest leads the account can buy before November.

### The employer-plan lane specifically

**$44,972.40 and 3,815 leads at $11.79, on two ads, both dark.** (`verified`.) Against lifetime spend that lane is 6.1% of the money and 9.6% of the leads. It is small as a share and it is the best unit economics in the file, which is the definition of an under-invested vector rather than a niche one.

### What it would take to reach it, which is the part that makes this the right swing

Read through `creative-strategy-by-brand-size.md`, this account has lived in two spend bands inside a year and sits in the lower one now, roughly $42,700 a month against an April peak of $156,716. That band's priorities are volume of output as a real lever, reaching genuinely new audiences rather than sweeping existing demand, and checking what the brand believes about its own customer. All three land here.

The brand's stated production capacity is **one to five net-new concepts a month**, with casting named as its top bottleneck. (`stated`, brand context.) **A headline static needs no creator, no shoot, no script and no casting call. It is a sentence and a photograph.** Before a 2026-11-01 Open Enrollment window that the brand plans two months ahead for, and whose planning deadline of 2026-09-01 has already passed, that is the difference between five swings and twenty.

And it is the strongest signal available to Meta. Per the differentiation hierarchy in `andromeda-v2.md`, **format sits at Tier 1, the highest-impact change there is**, above vehicle, hook, persona and messaging. A video-to-static move is the single biggest entity-level differentiation this brand can make. That matters unusually much in an account whose own diagnosis is severe concentration: four ads sharing one text hook carried 60.5% of the quarter, and under entity grouping that is very likely fewer distinct things than the count suggests. This account has iterated its most-used text hook at least four times without once changing the format, which is the exact behaviour `andromeda-v2.md` says now gets penalised. The fix is difference, and format is the biggest difference on the menu.

### The destination decision, sized

This one is small in dollars and it is urgent, so it belongs here rather than in a footnote.

The `go.healthformoms.co/save/` subdomain holds **40 ads, $8,918.29, 5,392 link clicks and 272 leads at a $32.79 blended cost per lead.** (`verified`, live ad-level pull 2026-09-04.) The validation established that this splits in two and only one half is broken. The March cohort in `Internal - ABO - TEST` converts at 8.69% leads per link click, indistinguishable from `www.`'s 9.50% to 10.63%. The August cohort in `USHA - CBO - OTP` converts at 0.82%.

**Four of those August ads are still ACTIVE as of this pull.** `Moms Nahuel WV#1 - V9 - Copy`, `moms-63 2b - Copy`, `moms-63 3e - Copy` and `moms-53 3 - Copy` together hold **$3,474.43, 2,188 link clicks and 18 leads**, which is 0.82% leads per link click and a $193.02 blended cost per lead. One of them, `moms-53 3 - Copy`, has taken **511 link clicks and produced zero leads**. (`verified`, live pull 2026-09-04.) The roll-up routed this to the operational owner marked urgent earlier the same day. It is still running.

The verdict was inconclusive on **cause**, because campaign, date and destination are perfectly collinear and no cut of this account separates them. It is not inconclusive on **what to do**. Whatever the cause, those four ads are duplicates of creative that works fine on `www.`, so switching them off costs the brand nothing it is not already getting. **Do not overclaim this in either direction:** the subdomain is not proven broken, the March cohort worked on it, and the four ads are the actionable subset rather than the whole domain.

**And `quiz.healthformoms.com` is unmeasured, not leaking.** Today it holds **30 ads, $138.27 lifetime, 57 link clicks, 25 landing page views and 2 leads.** (`verified`, live ad-level pull 2026-09-04.) That is up from the 26 ads the vault recorded yesterday, and there is now a second path, `quiz.healthformoms.com/2`, running in a new campaign called `USHA - CBO - Custom` under an ad set named `Moms-67 -lp2`, with four ads created 2026-09-03. **The quiz test is expanding right now, while this doc is being written.** One detail worth carrying: those `/2` ads report click-quality scores of 88.89 and 100, the normal range, which means the landing-page-view counter fires correctly on the quiz in a way it does not on `go.` (`verified` arithmetically from the raw counts.) So the quiz is instrumented. It simply has not spent enough to say anything. Treat it as unmeasured, keep it small, and do not let it take real November money before it has a lead volume worth reading.

## Alternatives considered and why not

Five directions were live going into this. Each was sized against the others before the call was made.

**1. Keep leading with the savings hook. Rejected as the lead, kept running.** The POV husband line carries roughly two thirds of current spend and its best expression, `moms-63 2b`, runs a $13.26 cost per lead in the brand's "fantastic" band. (`verified`, 90-day pull.) This is a real winner and per `seasonality.md` the evergreen proven work stays on while new work layers in, never swapped out wholesale. What it cannot be is the growth call, for two reasons. Its own compliance exposure is live: the on-screen claim *"saved $400 a month, AND the deductible is zero"* is a flat number and a flat promise against the brand's own non-negotiable rule to always say "up to 30%" and "$0 deductible option." (`verified` from creative fields against `stated` brand rules.) And it names no buyer. Per the whitespace read the account "switched from talking to somebody specific to talking to nobody in particular, and it paid 44.7% more per lead to do it."

**2. Put the Approved State List in the first frame across the account. The runner-up, and here is what demoted it.** `moms-53 3` is a genuinely strong ad. It holds the account's best click-through rate at **3.15% to 3.17%** and its cheapest link click at **$0.96 to $1.01**, both best in the file, and the brand names the state angle as its proven lever. (`verified`, live pulls; `stated`, brand context.) But run it on the trustworthy ratio and something shows up that nobody had checked. Over the 90 days it took **2,127 link clicks and produced 127 leads, which is 5.97% leads per link click**, against `moms-63 2b`'s **12.25%** and `moms-63 3e`'s **9.68%** in the same window. (`verified`, computed by hand from today's efficiency pull.) **The state list buys the cheapest clicks in the account and converts them worse than anything else at scale.** The likely reading is that a full-screen list of states makes people stop and hunt, and a good share of the hunters do not find their state, so the ad buys a cheap click from someone it then turns away. That is `inferred` and it fits the comments exactly: *"Why is this being shown in IL if it's not on the list???😭🤦🏼‍♀️"* and *"Ofc Georgia ain't on there 🤣"* (`verified` verbatims). It stays the runner-up because qualifying early is still right and its cost per lead is still good-band. It is not the lead because the mechanism it uses has a measurable leak in it.

**3. Lead into pregnancy and new-baby demand. Rejected, and it is not close.** On demand alone this would be first: 38 of 1,342 comments, fourteen months, the highest like counts in the corpus, 63.2% of the category's organic feed, and a lifetime keyword search for "pregnant" across every ad field returning zero. In a normal audit that is the definition of whitespace. It is not whitespace here, because the product screens her out and **the team confirmed on 2026-09-04 that it deliberately removed pregnancy from its own inspiration set.** (`stated`, Slack.) Leading here would send more women into a funnel that tells them no, in public, under an ad the brand paid for, using the brand's own name as the punchline. This is a recruitment cost to reduce, not a swing to take.

**4. Lead into the chronic-condition family. Rejected for the same reason, with more force.** The most emotionally intense identity in the corpus, and medical underwriting screens her out. Reaching her harder makes the problem worse.

**5. Push the quiz funnel as the new destination. Rejected for now, on evidence rather than on principle.** $138.27 and 2 leads decides nothing. It is being expanded anyway. The position is not "kill it," it is "keep it under a hundred dollars a week until it has a lead count worth reading, and do not let it near the November budget on the strength of a hunch."

## Confidence and what would raise it

**Overall confidence: mixed, and the call is provisional.** Here is the honest split, because the four decisions inside it do not carry the same weight of evidence.

| Decision | Confidence | What it rests on |
|---|---|---|
| Switch the four live `go.` ads off | **strong** | Duplicates of creative that works on `www.`; nothing is lost by stopping. `verified` live today. |
| Restart statics as the format | **strong** on the economics, **mixed** on whether the rate holds | 13,735 leads and 82,871 link clicks is a large denominator on two independent ratios. The auction has changed since. |
| Lead with the employer-plan switch | **mixed** | Gate one is `verified` at real scale. The gate-two argument is `inferred` and uncheckable. |
| Move the gate into the creative | **mixed** | The team's own words, `stated` 2026-09-04, against an account that has never said it. |

**What is genuinely strong here.** Two independent ratios point the same way on the static lane: a cost per lead 44.7% below video, and a leads-per-link-click rate exactly double it. The second one is the important one, because it is computed on the metric this brain has just proved is trustworthy and because the direction of the CTR rules out the easy objection. If statics simply bought cheaper junk, their click-through rate would be higher and their conversion lower. It is the reverse.

**What is genuinely weak, and it is the same weakness that limits every call in this brain.** Per the evidence ladder in `persona-research-and-creative-strategy-process.md`, post-purchase data is the gold standard and public comments sit near the bottom, and this brand holds only the bottom rung and only one source of it. Reviews are verified empty, surveys are verified empty, Reddit is unreachable, no competitor is tracked. So every persona here stays capped at **mixed** and the honest sentence is always "commenters under the brand's paid ads said."

**The three numbers that would settle this, in order of how much they would move it.**

**One. Revenue per lead, and whether it is paid per lead or per enrolled policy.** This is the fork that decides whether the whole account is optimising on the right number. If it is per lead, this call is right and probably understated. If it is per policy, then cost per lead has been the wrong north star for twenty-one months and the ranking of every winner in this brain could invert. **Brand-routed.**

**Two. The share of leads that reach a real conversation, split by ad or even just by week.** One number coming back from the partner agencies would close the largest measurement gap in this business. It costs nothing but a conversation, and it is the only thing that can test the gate-two inference this call leans on. **Brand-routed.** The cheaper first move the brand fully controls: find out why `invitee_meeting_scheduled` returns no data, because that instrument already exists.

**Three. What made the team stop making statics around March.** If it was a staffing or agency change, the lane comes straight back and this call ships this week. If something was learned, a lead-quality problem from static form fills or a platform issue, that reason is a hard constraint nobody has written down and it would overturn the largest piece of this recommendation. **Brand-routed, and it is the single question that most directly gates this call.**

**What would overturn the call outright.** Any one of: the partner agencies reporting that static-sourced leads enroll materially worse than video-sourced ones; a revenue model that pays per policy with a large enough gap between lanes to swamp a 2x lead-rate advantage; or a written reason the statics were killed that names a problem this doc cannot see. Absent those three, the evidence points one way.

## Open loops

**1. The brand has decided who it does not want, and its ads have never said so.**

On 2026-09-04 the operator wrote in Slack that he removed search terms about not affording insurance *"because we dont want broke people,"* and removed pregnancy too. Meanwhile no ad in this account's lifetime names a price, an income, or an eligibility rule before the click, and 42 of 1,342 comments contain "qualify," most of them describing a rejection after the fact.

*Pull: Tension.* It fired because the team's own account of who this offer is for and the account's total silence about money cannot both be a fair description of who these ads are inviting.

*Question:* How do mothers respond to an ad that says out loud who the offer is not for?

*Why it is a loop:* Every gate this product applies is currently discovered after the click, which means the brand pays for the click and then produces a public complaint. If naming the gate early costs less volume than it saves in wasted clicks, the fix is a line of copy rather than a media plan.

*Territory: Product.*

**2. A static's click turns into a lead twice as often as a video's, and nobody knows what she is doing differently.**

Statics converted 13,735 leads out of 82,871 link clicks, 16.57%. Video converted 25,834 out of 312,052, 8.28%. In the same comparison video buys 30% more clicks per impression, so the static is winning at the far end of the funnel rather than the near end.

*Pull: Surprise.* It fired because the format that buys fewer clicks converts twice as many of them, which is the opposite of what a cheaper-click story would predict.

*Question:* What is different about how a mom arrives at the form from a static?

*Why it is a loop:* If the answer is that a headline pre-qualifies her before she clicks, then qualification is the real lever in this account and it applies to video too. If it is something about the landing experience, the answer sits on the page rather than in the creative, and the whole production plan points somewhere else.

*Territory: Product.*

**3. Nobody knows whether this offer can actually beat an employer plan on price.**

The lane with the cheapest verified leads in the account's history speaks to a mother whose premium comes out of payroll before tax, often with an employer contribution on top. Nothing in this brain records what a private plan actually costs her by comparison, and the one complete outcome anyone has reported in 1,342 comments is a woman quoted $400 a month who said the offer saved her nothing.

*Pull: Curiosity.* It fired because the recommendation with the best numbers behind it also aims at the buyer whose existing deal is the hardest one in the category to beat, and no document in this brain has ever priced that comparison.

*Question:* How much does a mom on an employer plan actually save by moving to one of these plans?

*Why it is a loop:* It decides whether the cheapest lead in this account is also its most closeable one or its least. **Brand-routed**, because only the partner agencies hold the quoted numbers.

*Territory: Product.*

**4. A second funnel is being built out before anyone has measured the first thing about it.**

`quiz.healthformoms.com` went from 26 ads to 30 in a day, grew a second path at `/2`, and picked up a new campaign and ad set created 2026-09-03. Lifetime it holds $138.27, 57 link clicks and 2 leads. Its landing-page-view counter reports normal scores of 88.89 and 100, unlike the `go.` subdomain.

*Pull: Curiosity.* It fired because somebody is clearly building toward something specific here, and nothing in this brain says what it is or what it is meant to do better.

*Question:* What is the quiz page built to do that `/save/` does not?

*Why it is a loop:* The funnel destination is the highest-leverage product decision this brand makes and it is 58 days from its biggest season. Knowing the intent decides whether this gets protected budget as a real test or held at a trickle until it can be read.

*Territory: Product.*

## Appendix - Parker media links

Links and paths preserved exactly as returned by the Parker MCP on 2026-09-04. Ad account `HealthForMoms`, act `484897827497337`. Brand `aed0ff06-555d-4f4f-9bf8-31178e2fb977`.

### The lead call — the employer-plan statics, both dark

**`B1 - Copy 7`** — 5 variants, $30,339.32 lifetime, 11,845 link clicks, 2,584 leads, $11.74 CPL, 21.82% leads per link click, $15.89 CPM. Headline: *"Left my big insurance company for a mom-focused one. 24% cheaper and I choose my own doctor 😌"*. Created 2025-02-26. `CAMPAIGN_PAUSED`.
Facebook ad id: 120216241083030519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120216241083030519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/7e3133fccf8b205622146f7297669b76296123fb46177e5262ee89f0040ca8ba.jpg
Landing page: https://www.healthformoms.co/save/

**`B1 samar- Copy 1`** — $14,633.08 lifetime, 8,193 link clicks, 1,231 leads, $11.89 CPL, 15.03% leads per link click, $15.05 CPM. Headline: *"Didn't know I could ditch my job's health plan… until I did."* Created 2025-07-17. `ADSET_PAUSED`.
Facebook ad id: 120227092759640519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120227092759640519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b219b0aa7f7e7ed8d83fa471803f4b6c96ad98b2de118b2a8e68038439e759a9.jpg
Landing page: https://www.healthformoms.co/save/

### The rest of the dormant static library

**`B1 samar- Copy`** — the largest static ad-name group in the account's history. 39 variants, $54,224.86 lifetime, 26,614 link clicks, 4,441 leads, $12.21 CPL, 16.69% leads per link click, $16.18 CPM. Created 2025-07-17. `ADSET_PAUSED`.
Facebook ad id: 120228910482200519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120228910482200519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/59bf52c09c6081e3dfc63e0b17e649c989b490ad5b03079e469d1dc258e2cc0f.jpg

**`B2 - 10TH JUNE - Copy 16`** — 2 variants, $18,409.73 lifetime, 7,489 link clicks, 1,181 leads, $15.59 CPL. Headline: *"Moms...."*. Created 2025-06-10. `ADSET_PAUSED`.
Facebook ad id: 120224684049380519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120224684049380519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/2196cede33edbb670d810d017aa0c57568dc50db2e8c71b7b7a608410b0c0aae.jpg

**`OMC-Health for Moms-[B3-C11-V7]`** — $10,947.56 lifetime, 6,580 link clicks, 675 leads, $16.22 CPL, a 4.44% CTR and an $86.14 click-quality score. Created 2025-10-24, the last Open Enrollment ramp. `CAMPAIGN_PAUSED`.
Facebook ad id: 120232855500240519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120232855500240519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

**`B2 - 10TH JUNE - Copy 1`** — the self-employed static, $1,877.94 lifetime, 112 leads, $16.77 CPL, 54.4% of its spend on women over 45. Carried from the whitespace analysis; not re-pulled this run.
Facebook ad id: 120224684049440519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120224684049440519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/45c5cbc54f430c3c07a32a71077cdc97e1329a6f91856c6fbce9fef811164548.jpg

### The incumbent savings hook — keep running, do not lead with

**`Moms43 - 4 - V3`** — $57,506.21 lifetime, 2,668 leads, $21.55 CPL, 45.84% hook rate, 3.81% hold rate. Last 7 days $3,544.33 for 109 leads at $32.51 on a $27.33 CPM. Text hook *"POV: Telling your husband you found better health insurance, saved $400 a month, AND the deductible is zero. Wife of the year energy. 💕"* over a mother and baby on white bedding, no spoken words, music only. Created 2026-04-06. `ACTIVE`.
Facebook ad id: 120241073380060519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4

**`moms-63 2b`** — the account's cheapest lead at scale over the window. $5,529.74 for 417 leads at $13.26, 3,404 link clicks, 12.25% leads per link click, $21.33 CPM. Same text hook, different picture: a well-dressed mom and her young son walking out of a house. Created 2026-08-14. `ACTIVE`.
Facebook ad id: 120247093361410519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093361410519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399.mp4

**`moms-63 3e`** — the current top spender. $5,449.11 over the window for 353 leads at $15.44, 3,648 link clicks, 9.68% leads per link click, on the cheapest impressions of any real spender at $18.75. Created 2026-08-14. `ACTIVE`.
Facebook ad id: 120247093478820519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093478820519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6a45457e776af311dfb45d100c093bab9d3f90c7575195dfd86b6260763f1670.mp4

### The runner-up — the state list in the first frame

**`moms-53 3`** — $2,041.42 over the window for 127 leads at $16.07, with the account's best CTR at 3.15% and cheapest link click at $0.96, and its worst leads-per-link-click among the real spenders at 5.97%. Text hook *"Approved State List ✔️"*, verbal hook *"I'm so thankful for the mom that told me about this."* Created 2026-08-25. `ACTIVE`.
Facebook ad id: 120247254787160519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254787160519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e6225ca24b359ea0ab06bbeafe453b45496c1310c5a736ba3ea560045c6bd093.mp4

### The four live `go.` ads to switch off today

All four `ACTIVE` as of the pull on 2026-09-04, all in campaign `USHA - CBO - OTP`, ad set `Moms CBO OTP`. Together $3,474.43, 2,188 link clicks, 18 leads.

- **`Moms Nahuel WV#1 - V9 - Copy`** — $1,639.35, 690 link clicks, 63 landing page views, 6 leads, $273.23 CPL, click quality 9.13. Created 2026-08-17.
  Facebook ad id: 120247145872230519
  Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247145872230519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/645496c411d82a546a3e2deada69459c716615ad09f635ca0b978625c2778b37.mp4
  Landing page: https://go.healthformoms.co/save/
- **`moms-63 2b - Copy`** — $835.50, 656 link clicks, 54 landing page views, 5 leads, $167.10 CPL, click quality 8.23. Created 2026-08-31.
  Facebook ad id: 120247339552100519
  Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247339552100519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  Landing page: https://go.healthformoms.co/save/
- **`moms-63 3e - Copy`** — $504.01, 331 link clicks, 30 landing page views, 7 leads, $72.00 CPL, click quality 9.06. Created 2026-08-31.
  Facebook ad id: 120247339547070519
  Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247339547070519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  Landing page: https://go.healthformoms.co/save/
- **`moms-53 3 - Copy`** — $495.57, **511 link clicks, 9 landing page views, zero leads**, click quality 1.76. Created 2026-08-31.
  Facebook ad id: 120247339531520519
  Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247339531520519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  Landing page: https://go.healthformoms.co/save/

### The healthy March `go.` cohort — the reason the subdomain is not condemned outright

All in campaign `Internal - ABO - TEST`, all paused, all created 2026-03-13. Together they took 2,574 link clicks and produced 234 leads, 9.09%, on the same subdomain. They also hold the best hold rates in the account at 12.55% to 15.47%.

- **`Yeti State Angle - 1  - V3`** — $1,175.84, 800 link clicks, 80 leads, $14.70 CPL, 13.41% hold rate. Text hook *"Health Insurance is a scam 😉"*.
  Facebook ad id: 120239524792950519
  Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239524792950519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/5d1bf2bc2f7261b0bc786763c21a68540eece7aba5acd69edc42292cf26932bd.mp4
- **`Yeti State Angle - 1 - V1`** — $719.34, 439 link clicks, 50 leads, $14.39 CPL, 13.38% hold rate.
  Facebook ad id: 120239524792970519
  Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239524792970519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- **`Yeti State Angle - 1 - V2`** — $769.85, 544 link clicks, 39 leads, $19.74 CPL, 13.40% hold rate.
  Facebook ad id: 120239524792940519
  Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239524792940519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- **`Yeti State Angle - 2 - V1`** — $826.09, 353 link clicks, 31 leads, $26.65 CPL, 12.55% hold rate. Text hook *"What!? 😳 i owe a $20,000 bill for anesthesiology??"*.
  Facebook ad id: 120239524721230519
  Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239524721230519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- **`Yeti State Angle - 3  - V3`** — $417.33, 278 link clicks, 15 leads, $27.82 CPL, 55.12% hook rate and 15.47% hold rate, the best paired attention numbers in this cohort. Verbal hook *"Just got off a two hour call fighting for them to cover my newborn son's hospital stay."*
  Facebook ad id: 120239524801690519
  Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239524801690519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- **`Yeti State Angle - 2 - V3`** — $400.05, 160 link clicks, 19 leads, $21.06 CPL, 15.42% hold rate.
  Facebook ad id: 120239524786180519
  Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239524786180519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

### The quiz destination — unmeasured, and expanding

30 ads, $138.27 lifetime, 57 link clicks, 25 landing page views, 2 leads. Two paths now live.

- **`moms-67 4#`** — the largest quiz ad, $66.04, 27 link clicks, 24 landing page views, click quality 88.89. Campaign `USHA - CBO - Custom`, ad set `Moms-67 -lp2`. Created 2026-09-03. `ACTIVE`.
  Facebook ad id: 120247380940680519
  Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247380940680519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/50ac45c62c1386238854a24b156f56f119620062459f1314a7fb3611355040ff.mp4
  Landing page: https://quiz.healthformoms.com/2
- **`moms-63 3e - Copy`** on the quiz — $26.04, 10 link clicks, 1 lead. Created 2026-09-02.
  Facebook ad id: 120247367204690519
  Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247367204690519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  Landing page: https://quiz.healthformoms.com/#/indvfam
- **`moms-63 2b - Copy`** on the quiz — $25.84, 13 link clicks, 1 lead. Created 2026-09-02.
  Facebook ad id: 120247373812970519
  Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247373812970519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  Landing page: https://quiz.healthformoms.com/#/indvfam

### Funnel destinations observed

- https://www.healthformoms.co/save/ — the workhorse, and the destination this call points at
- https://go.healthformoms.co/save/ — four ads still live on it as of 2026-09-04
- https://quiz.healthformoms.com/#/indvfam — unmeasured
- https://quiz.healthformoms.com/2 — new as of 2026-09-03, unmeasured
- https://healthformoms.co/save-cw — a variant path seen on two older ads, not re-pulled this run

### Non-media sources

**Parker chat history** — retrieved through Parker MCP `search_chat_history` on 2026-09-04. Slack thread `1788538777.074209` (the TikTok inspiration set, source of the *"we dont want broke people"* statement) and Slack thread `1788529081.275569` (landing page H1s, evidence the destination is being worked on right now). Channel `C0BUQEFF70V`, team `T02N4RQ62DR`. No public link; reproduced by that call.

**Custom metric definitions** — retrieved through Parker MCP `list_custom_metrics` for brand `aed0ff06-555d-4f4f-9bf8-31178e2fb977` on 2026-09-04. Four auto-detected pixel events including `offsite_conversion.fb_pixel_custom.invitee_meeting_scheduled`, zero formulas, no revenue metric. No public link; reproduced by that call.

**Ad comment corpus** — 1,342 comments lifetime, read through Parker MCP `search_facebook_ad_comments_sql`. Four substring counts run 2026-09-04: "pregnan" 38, "existing" 38, "qualify" 42, "deductible" 207. No dashboard link exists for a comment pull; reproduced by querying the brand id.

**Brand site pages, never opened in any build session** — https://healthformoms.co/ and https://quiz.healthformoms.com/ , both refused by network egress policy.

---

This is everything I know about Andromeda v2.

This is everything I know about static ad design.

This is everything I know about seasonality in creative.

This is everything I know about tailoring creative strategy to brand size.
