---
brand: health-for-moms
doc: website-and-product-audit
generated_on: 2026-09-03
refresh_by: 2026-11-01
sources_read:
  - Parker MCP `get_brand_persona` brand context document, brand aed0ff06-555d-4f4f-9bf8-31178e2fb977, pulled 2026-09-03 (~50KB, 14 sections, includes the brand's own uploaded guidelines PDF summary)
  - Parker MCP `search_facebook_ads_sql`, act 484897827497337 `HealthForMoms`, last 90 days (2026-06-05 to 2026-09-02), grouped by ad name and by ad, plus a lifetime cut (page 2) and a static-only cut
  - Parker MCP `search_facebook_ad_comments_sql` and `search_facebook_ad_comments_semantic`, brand comment corpus of 1,322 comments spanning 2025-01-13 to 2026-09-03
  - `running-notes/missing-context.md`, `running-notes/brand-rules.md`, `running-notes/success-definition.md` (Phase 0 intake and surface test, 2026-09-03)
  - Public web search, 2026-09-03: the HealthForMoms terms page naming the operating entity
  - NOT read, blocked: healthformoms.co and quiz.healthformoms.com. See "What could not be seen" below.
---

# Website and product audit — Health For Moms

> **CORRECTION, 2026-09-04, verified by direct pull.** The figures "903 link clicks against 234
> landing page views" and a "$75.72 CPL" on the `Moms Nahuel WV#1` group are **not the quiz
> destination.** They are an aggregate of two different destinations summed together, and the
> attribution to `quiz.healthformoms.com` is wrong.
>
> Ground truth, `Moms Nahuel WV#1 - V9 - Copy`, two variants of the same creative:
>
> | Variant destination | Spend | Link clicks | Landing page views | Landing rate | Leads | CPL |
> |---|---|---|---|---|---|---|
> | `go.healthformoms.co/save/` | $1,639.35 | 690 | **63** | **9.1%** | 6 | **$273.23** |
> | `www.healthformoms.co/save/` | $404.23 | 213 | 171 | 80.3% | 21 | $19.25 |
> | **summed (the wrong figure)** | $2,043.58 | **903** | **234** | 25.9% | 27 | **$75.69** |
>
> So 903 = 690 + 213, 234 = 63 + 171, and $75.72 is the blend of a broken destination and a
> working one. The parent `Moms Nahuel WV#1 - V9` on `www.` is healthy: $17,723.91, 7,196 link
> clicks, 6,198 landing page views (86.1%), 635 leads, $27.91 CPL.
>
> **The real finding survives and is sharper:** the collapse is entirely on `go.healthformoms.co`,
> not the quiz, and the same creative on `www.` converts normally. `quiz.healthformoms.com` is a
> separate, brand-new test — 26 ads, $138.27 lifetime, 57 link clicks, 25 landing page views,
> 2 leads, every ad created 2026-09-02 or 09-03. Treat the quiz as **unmeasured**, never as a leak.


> **CORRECTION, added 2026-09-04 by the build orchestrator.**
>
> This document reports the `quiz.healthformoms.com` destination as having bought **903 link
> clicks against 234 landing page views at a $75.72 CPL**. That is wrong and must not be carried
> into any downstream synthesis.
>
> A direct verification pull on 2026-09-04, filtering `landing_url contains "quiz."` across
> lifetime with no date window, returns the true figures: **26 ads, $138.27 total lifetime spend,
> 72 clicks, 57 link clicks, 25 landing page views, 2 leads, $69.14 CPL.** Every one of those ads
> was created on 2026-09-02 or 2026-09-03. The quiz destination is a **brand-new test that has
> barely spent**, not an established leak.
>
> The $69.14 CPL is real but rests on 2 leads and $138 of spend, which is far too little to
> judge. The 43.9% landing rate (25 of 57) is likewise unstable at this volume. Treat the whole
> quiz destination as **unmeasured**, not as underperforming.
>
> **The `go.healthformoms.co` finding in this document is unaffected and independently
> confirmed** — the monthly performance report reproduced it separately (August: 11 ads,
> $2,046.40, 6 leads, $341.07 CPL, 1,103 link clicks to 77 landing page views, a 7.0% landing
> rate against 84.6% for the rest of the account, with the same video file running to both
> destinations at $19.22 and $271.90). That one is a genuine, live, costly break.



## What could not be seen, and why it matters here

This doc has a hole in the exact place a product audit usually starts, so read the whole thing with that in mind.

**The brand's own site could not be opened during this run.** Both `healthformoms.co` and `quiz.healthformoms.com` were refused by this session's network egress policy, not by the sites themselves. The refusal was an `EGRESS_BLOCKED` policy denial on the domain, which the environment's own guidance says to report rather than route around. So there is no first-hand read of the homepage, the `/save/` funnel, the `/save-cw` variant, the quiz on the `.com` domain, the form fields, the qualifying questions, the state list, the consent and TCPA language, or the footer disclaimers. (`verified` that the block occurred, this run, 2026-09-03.)

That gap is not fatal, because for this brand the ad account and the ad comments turn out to be a stronger read of the actual product than the site copy would have been. Real moms in the comments describe what the funnel asked them and what it told them, which is the product as experienced rather than the product as marketed. But three things stay genuinely unknown until someone opens the pages: the exact wording of the qualification questions, the exact state list, and the exact consent language that governs how a lead is passed on. Those are named as blanks below, not guessed at.

**The rest of the picture is normal for this brand and already logged.** Customer reviews and post-purchase surveys are dark, confirmed empty in the Phase 0 surface test rather than broken, and the team said so directly in Slack on 2026-09-03. No competitors are tracked. Northbeam is not connected, so every number here is Meta-reported. All of that is in `running-notes/missing-context.md`.

## The frame: this is not a catalog, and pretending otherwise would break the doc

The prompt behind this doc is built for a brand with SKUs. Health For Moms does not have any. Forcing a SKU list here would invent a product line that does not exist, so the sections below are answered against what this business actually sells, and where a section has no honest equivalent it says so.

Here is the real shape. Health For Moms is a lead-generation matching service. It is not an insurance carrier and it does not sell a plan. (`stated`, brand context document, Section 1.) A mom sees a video ad, clicks to a landing page, answers a short set of questions, and her contact details are handed to a partner insurance agency, where a licensed agent calls her and tries to enroll her in a private health plan. Health For Moms is paid for the handoff. The mom pays nothing to Health For Moms.

So the business has three product layers, and they are easy to blur:

1. **What the mom experiences as the product.** A free match and a phone consultation with an agent. No cart, no price, no checkout.
2. **What the ads actually sell.** Not the match. The ads sell an outcome on the underlying plan: "save up to 30%," "$0 deductible options," "keep your own doctor." That outcome is delivered by a third party the brand does not control.
3. **What is actually bought at the end.** A private, medically underwritten health plan sold by a partner agency. This is the thing with the real economics, the real exclusions, and the real customer experience, and it is the layer Health For Moms has the least control over and the least visibility into.

The single most important structural fact in this audit is that **layers 2 and 3 do not match as cleanly as the marketing implies**, and the evidence for that gap is strong. That is the "asset becomes liability" problem this doc exists to surface, and it runs through every section below.

For the account's shape, which sets the denominators used throughout: in the last 90 days the account ran 117 distinct ad-name groups against $98,276.81 of spend, produced 4,336 leads at a $22.67 cost per lead, and recorded zero purchases, because there is no purchase event by design. Delivery was 95.2% female, 81.2% aged 25 to 44, 99.5% mobile, and split 60.2% Facebook to 39.2% Instagram. (`verified`, Parker MCP ad pull, 2026-06-05 to 2026-09-02.)

## Full SKU list and product lines

There is no SKU list, and no honest way to write one. What exists instead is a small set of **funnel surfaces** and a partly visible set of **underlying plan types**. Both are mapped here, because between them they are what a strategist actually needs.

### The funnel surfaces, which behave like the real product line

Three distinct landing destinations appear in the ad account. This is the closest thing this brand has to a product range, because choosing which one an ad points at is the highest-leverage product decision anyone here makes.

| Surface | Where it lives | Role in the account | Evidence |
|---|---|---|---|
| `https://www.healthformoms.co/save/` | Main site | The workhorse. Nearly every ad with a recorded destination points here, across both the 90-day window and the lifetime cut. | `verified`, ad pull |
| `https://healthformoms.co/save-cw` | Main site, variant path | A second variant seen on two older ads, one from 2025-10-27 and one from 2026-03-12, both in an "Internal - ABO - TEST" campaign under an ad set literally named "Winner Group." | `verified`, ad pull |
| `https://quiz.healthformoms.com/#/indvfam` | A **different domain**, `.com` not `.co` | A separate quiz funnel on a separate domain. Seen on the ad group "Moms Nahuel WV#1 - V9 - Copy," which ran 2026-08-11 to 2026-09-02. | `verified`, ad pull |

The third one is the finding, though the destination is the `go.healthformoms.co/save/` destination, not the quiz. On the `Moms Nahuel WV#1 - V9 - Copy` creative the `go.` variant converted 690 link clicks into 63 landing page views, a 9.1% landing rate, 6 leads and a $273.23 cost per lead, while the identical video file on `www.healthformoms.co/save/` converted 213 clicks into 171 views, 80.3%, 21 leads and $19.25. `quiz.healthformoms.com` is a separate brand-new test at $138.27 lifetime across 26 ads all created 2026-09-02 or 09-03, and is **unmeasured**, not leaking. *Verified* by ad-level pull, 2026-09-04. See the correction block at the top of this document. Click quality tells the same story: 9.13 on `go.` against 80.28 on `www.`, versus roughly 85 to 90 for the ads pointing at `/save/`. For contrast, the account's biggest spender over the same window, "Moms43 - 4 - V3," bought 21,085 link clicks and recorded 18,413 landing page views, an 87.3% arrival rate, at a $22.21 cost per lead. (`verified`, Parker MCP ad pull, last 90 days.)

Against the brand's own scoreboard, where under $15 is "fantastic," $15 to $20 is "good," $20 to $25 is "meh," and over $25 is "not good" (`stated`, brand context Section 11), the `go.` destination's $273.23 cost per lead is not a soft miss. It is more than ten times the failure line. The ad group is currently in an `ADSET_PAUSED` state, so someone may already have caught it. Whether the leak is a redirect problem, a slow page, a tracking gap, or a genuinely worse quiz is not knowable from the outside, and it is one of the open loops below.

### The underlying plan types, seen only through the gaps

The brand describes the focus as **private health plans, explicitly not government marketplace plans**, sold with premium savings and low or no deductible options. (`stated`, brand context Section 1.) The brand's own compliance rules forbid any reference to the ACA or government programs in creative, and ban the words "policy," "discount," "cheap," "exclusions," and "guaranteed." (`stated`, brand context Section 8.)

What the plans actually are is only visible through what the funnel rejects, and there the evidence is consistent and independent of the brand's framing. **These are medically underwritten plans.** A commenter who reads as an insider put it plainly on 2025-07-01: *"If you are currently pregnant, you dont qualify. Its underwritten, if you have health concerns, be warned."* Another commenter who identifies as a seller of these plans wrote on 2026-05-17: *"these plans apply to anyone who is healthy enough to qualify for them. I sell them all day long and they work as great as they sound."* (`verified` that the comments exist and say this; `inferred` that the plans are underwritten and therefore not ACA-compliant, resting on the underwriting language plus the pattern of health-based denials documented under Known product issues.)

A tiered structure shows up once, thinly. A commenter on 2026-04-07 described *"the plus plan covers unlimited labs up to $100 each. They DO cover emergency care and treatments 💕 at 100%, outside of pre-existing conditions. They cover prescriptions. These plans are not for everyone."* That is a single source who appears to be selling, so treat it as **thin**: it suggests a named "Plus" tier exists above a base tier, and nothing more. One price point appears, equally thin: an apparent agent wrote on 2026-05-17 that she *"just signed up a healthy 39 yr old male and his Premium is just under $350/ month."* One data point from an interested party is not a price list.

**Named blanks.** The plan names, the tier structure, the carriers behind them, the actual premium ranges, the deductible options by tier, and the covered-benefit schedules are all unavailable from any source reachable in this run. These sit with the brand and its partner agencies.

### What the shape of the line says

The line is extremely tight, and getting tighter. One service, one audience, one promise, one dominant landing page. There is no adjacent product, no second vertical, no life or dental or vision extension visible anywhere in the account or the brand document. For a lead-generation business that concentration is a genuine strength, because it is what lets the brand own the "for moms" position that no generic rival holds. (`stated` positioning claim, brand context Section 6; the concentration itself is `verified` from the account.)

One creative-side fact belongs here because it says something about the line rather than the ads: **the account ran zero static ads in the last 90 days.** A static-only cut of the window returned no results at all, against 117 ad groups total. Statics were a real part of the mix historically, and the lifetime cut shows old statics with some of the cheapest costs per lead the account has ever recorded. The brand has said it wants to be video-first with "MAYBE some image ads to find angles." (`stated`, Section 11.) The account has taken that further than the brand said, all the way to none. (`verified`, Parker MCP static-only pull, last 90 days.)

## Top sellers and hero products

With one service there is no best seller. The useful version of this question is: **which creative and which funnel path actually carry the business**, since that is where the acquisition money goes and where a wrong read would hurt most.

**The hero is one video concept, and the concentration is severe.** In the last 90 days the ad group "Moms43 - 4 - V3" spent $42,741.16 of the account's $98,276.81, which is 43.5% of all spend in one place, and returned 1,924 of the 4,336 leads at a $22.21 cost per lead. It is a video of a mother and baby lying in bed on white bedding, looking calmly into the camera, with no spoken hook and music only, carrying the on-screen line *"POV: Telling your husband you found better health insurance, saved $400 a month, AND the deductible is zero. Wife of the year energy. 💕"* (`verified`, Parker MCP ad pull with creative fields, last 90 days.)

That same text hook is doing far more work than one ad. It appears verbatim, down to the emoji swap, on six separate ad groups in the 90-day window: "Moms43 - 4 - V3," "Moms43 - 4 - V1," "Moms43 - 4 - V4," "moms-63 2b," "moms-63 3e," and "moms-65 1a." Together those spent $67,381.71 of the window's $98,276.81, which is 68.6% of everything. **One hook line is carrying more than two thirds of the account.** (`verified`, summed from the ad pull.)

**The efficiency picture disagrees with the spend picture, and the brand's own rule says to report both.** `running-notes/brand-rules.md` records that the team expressed no preference on the spend-versus-efficiency tiebreak, so both readings go here. On spend, "Moms43 - 4 - V3" is the hero and Meta is pouring budget into it. On efficiency, it is only "meh" by the brand's own tiers at $22.21. The genuinely efficient ads in the window are smaller and newer: "moms-63 2b" at a $13.29 cost per lead on $5,527.76 of spend, "moms-63 3e" at $15.14 on $4,632.22, and "moms-53 3" at $16.01 on $1,761. All three clear the brand's "good" line, and the first clears "fantastic." (`verified`, ad pull.)

**Mark this as a candidate, not a winner.** `running-notes/success-definition.md` sets a two-gate bar for this brand: cost per lead first, then lead quality before real scale. Parker can see gate one and cannot see gate two, because lead quality lives with the partner agencies and never enters Meta. So the honest statement is that "moms-63 2b" and "moms-63 3e" have **passed gate one** and are candidates for scale. Whether the leads they produce actually enroll is unknown, and given what the Known product issues section documents about the qualification gate, that is not a small unknown.

**One historical read worth carrying forward, marked as a real puzzle.** The lifetime cut shows several 2025 static ads with costs per lead the current account cannot touch: "IMG 6" at $6.88 and $7.17, "5TH APR - Copy 29" at $9.62, "B1 - Copy 7" at $10.77 and $12.62. But those same ads show a strange funnel shape. "IMG 6" recorded 4,653 link clicks, only 905 landing page views, and yet 666 leads. Leads cannot plausibly exceed 73% of the people who reached the page. Either those campaigns captured leads somewhere other than the website, most likely a Meta on-platform lead form, or the landing-page tracking was not firing then. (`verified` that the numbers are what they are; the explanation is `data-limited`, and it matters, because if on-platform forms really did produce sub-$10 leads that is a live product decision the brand should revisit before the November ramp.)

## Bundles and starter packs

**Not applicable, and the absence is informative rather than a blank.**

There is nothing to bundle. The consumer pays nothing, there is one service, and there is no order value to lift. The concept of a starter pack has no equivalent either, because the first purchase is not a purchase, it is a form fill.

The closest structural analogue is the **short qualification quiz itself**, which does the job a starter pack usually does: it lowers the cost of the first yes. The brand frames the entry as "answer a few simple questions" and "it takes 30 seconds," and positions that low friction as the direct counter to the overwhelm objection. (`stated`, brand context Sections 1 and 5.) A commenter on 2025-08-07 gives the length from the other side: *"So I don't qualify with the 4 questions they asked!"* So the entry gate is roughly four questions long. (`verified` that one commenter says four; the exact question set is a named blank, since the page could not be opened.)

The important thing about that quiz is that it is **not only an easing device. It is also a screen.** A starter pack tries to say yes to as many people as possible. This quiz's job is partly to say no. That double role is the source of most of the friction documented below.

## Product-level differentiators

The brand states five main differentiators. Each is checked against what can actually be verified, because the prompt's warning applies with unusual force here: several of these marketed strengths contain the exact fact customers experience as the problem.

**1. "Save up to 30% on premiums with $0 / low deductible options."** (`stated`, brand context Section 1.) The compliance rule is strict and the brand knows it: always "up to 30%," never drop the "up to," and always "$0 deductible option," never a flat promise. (`stated`, Section 8.) **The ads are not holding that line consistently.** The account's single biggest spender, and the five ad groups sharing its hook, run the on-screen claim *"saved $400 a month, AND the deductible is zero."* That is a specific dollar figure and a flat statement that the deductible is zero, not an "up to" and not an "option." Meanwhile the body copy on those same ads says "saving you 20% or more," which is a different number from the 30% in the brand guidelines and points the opposite way, since "or more" is an open-ended floor rather than a capped ceiling. (`verified`, ad creative fields, last 90 days.) **Flag for legal review before this claim is used again.** Whether the brand may say it is a question only the brand and its compliance counsel can answer, and it is riding on 68.6% of current spend.

**2. "Nationwide coverage, see any doctor, anywhere in the U.S."** (`stated`, Section 1.) This does not survive contact with the comments. Moms report being told there is no coverage in their area, and report the state list excluding them. One on 2026-03-16: *"Why the hell is this ad showing if they dont offer this in Oregon or ANY of the surrounding states??"* Another on 2026-03-18: *"It looks like it's in 37 states 🙄."* Another on 2026-04-10, simply: *"It's not in my state."* (`verified`, comment corpus.) The brand's own document describes a "state-by-state qualification process," which is the honest version. **"Nationwide" and "state-by-state" cannot both be the headline.**

**3. "Freedom to choose your doctor or pediatrician."** (`stated`, Section 1.) Unverifiable from outside, and one comment pushes back hard on the practical side, asking on 2026-04-03: *"Yeah but how many places accept this insurance ???????"* Network breadth is exactly the kind of claim that needs the plan documents to check. **Named blank, route to the brand.**

**4. "Real coverage that actually pays when it matters."** (`stated`, Section 1.) This is the most exposed claim in the set, because it is the direct promise the product's underwriting most visibly breaks for the people it turns away. It is examined in full under Known product issues.

**5. The mom-first position itself.** This one is real and it is the strongest thing the brand owns. No major insurance lead-generation rival speaks only to mothers. The generic platforms serve everyone and speak to no one in particular. (`stated` as positioning in Section 6, but `inferred` as genuinely differentiated, resting on the absence of any mom-specific rival in the brand's own competitor list of EverQuote, QuoteWizard, HealthPlusLife and SmartFinancial, and on the total absence of a tracked competitor set to check it against.) **Confidence: mixed**, because the competitor branch is deferred and nobody has actually looked.

The differentiator that turns out to matter most is one the brand does not market at all: **speed and simplicity of the first step**. Four questions and thirty seconds is a genuine advantage over the marketplace experience these moms describe, and it is the one promise the brand fully controls, because it happens before the handoff.

## Patents, proprietary materials, and manufacturing edges

**One claimed proprietary asset exists, and it is a name rather than a mechanism.**

The brand markets the **MomSmart Coverage Method™**, described as "new tech that scans plans and matches each family with the right private health plan based on their needs, doctors, and budget," delivering "nationwide plan access, transparent pricing, and personal advisors" to help moms "save up to 30% while gaining $0 deductible protection and freedom of choice." It is built into the brand's CTA architecture as one of three primary frameworks, the "Mechanism CTA," recommended for warm and solution-aware audiences. (`stated`, brand context Section 7.)

Reading past the framing: what is described as "new tech that scans plans" is, on the evidence available, a roughly four-question form that routes a contact record to a partner agency. There is no evidence in the ad account, the comments, or the brand document of a plan-comparison engine the customer ever sees. Not one comment among 1,322 describes being shown plans, prices, or a comparison. Several describe the opposite, being told they do not qualify without being told why, like the mom on 2025-08-03: *"Well, this mom did not qualify and it didn't tell me why."* (`verified`, comment corpus.)

So the honest read is that **MomSmart Coverage Method™ is a naming and positioning asset, not a technology moat.** That is not worthless. A named mechanism is a real direct-response device and the brand uses it deliberately. But it is not defensible the way a patent is, and a competitor could copy the move in an afternoon.

**Named blanks.** No patent, trademark registration status, proprietary data asset, or exclusive carrier relationship could be verified. The ™ symbol indicates a claim of common-law trademark rather than a registration, and no registration was checked in this run. Whether any exclusive agency relationship exists is unknown.

**One structural note on ownership, marked as inference.** Public search confirms the site is operated by **Insurance Yeti, LLC** and its subsidiaries and affiliates, and that HealthForMoms "provides users the opportunity to obtain quotes from insurance carriers and other service providers by matching users with appropriate offerings," while stating it does not guarantee approval or that carriers will make contact. (`verified` via public web search of the HealthForMoms terms page, 2026-09-03.) Separately, the ad account's campaigns are named `USHA - ABO - SCALE - MOMS` and `USHA - ABO - TEST - MOMS`. A campaign name is an inventory handle and proves nothing about creative, but it does legitimately reveal how the account is organized, and "USHA" is a common abbreviation for USHEALTH Advisors, an agency that sells underwritten individual health plans. That would fit the underwriting evidence exactly. (`inferred`, low confidence, from account organization only. **Route to the brand to confirm who the partner agency actually is**, because the whole gate-two lead-quality question depends on knowing.)

## Known product issues

This is the most evidence-rich section in the doc and the most consequential. The reviews surface is dark for this brand, so per the substitution rule in `running-notes/missing-context.md`, the evidence here comes from the Facebook ad comment corpus, labelled as such. That corpus holds **1,322 comments** spanning 2025-01-13 to 2026-09-03, and every rate below is against that denominator.

Two cautions before the numbers. Comment sections skew negative, because annoyed people type and satisfied people leave. And a comment section on a cold-traffic insurance ad attracts a lot of general political and category venting that has nothing to do with this brand. Both are accounted for below.

### Issue 1: the product excludes pre-existing conditions, and moms find out at the gate

**38 of 1,322 comments, 2.9%, use the phrase "existing."** They are strikingly consistent and they span fourteen months, from 2025-07-05 to 2026-09-02, which makes this a durable pattern rather than a spike. Representative and exact:

- 2026-09-02: *"Preexisting health condition of cancer disqualified me"*
- 2026-08-13, 2 likes: *"It only works if you don't have any preexisting conditions. You gotta be perfectly healthy to qualify it looks like"*
- 2025-08-27, 5 likes: *"They don't cover preexisting conditions. Don't waste your time"*
- 2025-10-24: *"I clicked on the link, but was told that since I have a preexisting condition, there is no coverage in my area."*
- 2025-07-23, from a commenter who identifies as a certified marketplace application counselor: *"they're holding pre-existing conditions against you, which is illegal. Their system automatically bounced me out."*

Specific conditions named as disqualifying across the corpus include cancer, type 1 diabetes, asthma with a heart murmur, and rheumatoid arthritis.

**Read:** this is significant despite the modest 2.9% rate, for three reasons. It recurs steadily over more than a year rather than clustering. The comments describe a first-hand experience of being rejected, not an opinion. And several carry likes, which means other readers recognised it. **Confidence: strong.**

Two commenters assert the exclusion is illegal. It is almost certainly not, because ACA guaranteed-issue rules apply to marketplace plans and the brand explicitly sells outside that market. But the belief itself is a real marketing problem regardless of the law, and one well-informed commenter on 2025-08-28 lays out the correct version for everyone reading: *"If they're providing plans of private insurance companies, they can discriminate against pre-existing conditions (including pregnancy), which is why Obamacare was such an important thing."*

### Issue 2: the product excludes pregnant women, and the brand is called Health For Moms

**38 of 1,322 comments, 2.9%, contain "pregnan," and this is the sharpest wound in the account** because the exclusion collides head-on with the brand name. The comments are not confused, they are pointed, and several carry real engagement:

- 2026-04-01, 7 likes: *"your insurance says im not eligible because im pregnant 😂 huh.. so much for being for Moms 😂"*
- 2026-05-19, 4 likes: *"Says this is for moms….but you can't get a plan if you're pregnant or planning to become pregnant… 🤔"*
- 2026-04-12, 4 likes: *"I like how it's 'insurance that has your back' but apparently there's no plans for someone who's pregnant with type one diabetes. Yeah, totally has my back on the condition that I'm healthy before getting the insurance"*
- 2026-04-08, 4 likes: *"Plans not available for those that don't plan or can't get pregnant anymore bc of an unexpected hysterectomy last year - yet have kids already… (health for moms) makes sense 👍🏼"*
- 2025-11-23: *"Marketing towards mothers while not covering pregnancy is a disgusting tactic."*
- 2026-02-03: *"Health for Moms, but only if your babies are out of the womb. I was denied for being pregnant. Scam."*

The screen is apparently forward-looking as well as current. A commenter on 2026-02-08 describes the question itself: *"One question literally asks if you are pregnant or planning to be pregnant? The answer choices are no and I'm not planning to be or yes I'm pregnant. I'm not pregnant but I'm planning to be. So I picked yes pregnant and it says there are no plans."*

**Read: this is the highest-severity issue in the audit.** The rate is only 2.9%, but rate is the wrong measure here. These comments carry more likes than almost anything else in the corpus, they name the brand's own promise back at it, and they are unanswerable, because the brand cannot argue with a mother who was turned away by a product called Health For Moms. **Confidence: strong.**

There is a real tension worth naming rather than resolving. The brand's own internal guardrail says "no pregnancy-only targeting, focus on moms with kids, not expectant mothers exclusively." (`stated`, Section 8.) That guardrail may well have been written *because* of this exclusion. But the guardrail governs targeting, and the comments show pregnant women arriving anyway, because a broad audience of women aged 25 to 44 will always contain them.

### Issue 3: the lead handoff produces a flood of calls and texts, and it breaks the brand's core promise

The brand's whole emotional position is pressure-free, mom-to-mom, "Mom BFF" guidance. (`stated`, Section 1.) What a meaningful set of commenters describe is the opposite, and they describe it in detail:

- 2026-03-16, **33 likes, the most-liked comment surfaced anywhere in this run**: *"Filled it out and have been getting calls everyday from all sorts of companies which are mostly India based. Also, the harassment from whomever keeps calling me about Medicare (India again). This is the ONLY form I've filled out since getting my new phone number 3 months ago so it came from this site!"*
- 2025-11-28: *"I filled this out because it literally says we won't be contacted by random agents. That's a lie. I immediately received 5 text messages from 5 different agents claiming to be from 5 different companies."*
- 2025-09-17, 6 likes: *"Absolutely do not give them your info. You will receive calls and texts nonstop from an insane amount of reps."*
- 2026-01-28: *"It listed no selling my number to scammers but it's been just a few hours and I've had multiple numbers contact me with different agency type names"*
- 2025-10-03: *"I connected with a rep via text, wasted my time and gave her all my info and then she ghosted me"*
- 2026-05-17, **17 likes**: *"How many calls will I get if I try to see how this works?"*

**Read: severe, and structurally different from issues 1 and 2.** The other two are honest product limits that marketing has to work around. This one describes the brand's stated promise being contradicted, and two separate commenters say the page made an explicit representation about not being contacted by random agents that was then broken. That is the kind of gap that draws regulatory attention in lead generation, and the brand cannot verify or fix it from inside Meta because the behaviour happens downstream at the partner agencies. **Confidence: strong on the pattern, `data-limited` on the cause.** Whether the leads are being sold to multiple buyers, or one agency is over-dialling, or something else, cannot be seen from here. The exact on-page consent language is a named blank, because the page is blocked.

### Issue 4: legitimacy doubt, running at a low but persistent rate

**45 of 1,322 comments, 3.4%, contain "scam."** The important cut is that **most of them are not about this brand.** Reading all 45, roughly 29 are venting about American health insurance generally, which is actually the brand's own villain framing working as intended, and about 16 are aimed at Health For Moms. So brand-directed scam accusations run at roughly **1.2% of the corpus**.

The brand-directed ones cluster on three things: the funnel asking for information before showing anything, the brand being hard to verify by search, and the exclusions. Exact:

- 2025-01-20: *"I tried to look at them through a regular internet browser and nothing comes up...the link only works through Facebook and they want all your information before they show you anything....sounds like a scam to me."*
- 2025-07-24, 1 like: *"A Google search doesn't pull anything about this. Is it legit?"*
- 2026-03-26: *"Ha… 'in these states' proceeds to list all 50 states… scam"*
- The most damaging single comment in the corpus, from 2025-01-13, with **14 likes and 10 replies**, is a long pasted summary of Reddit discussion asserting the plans are "generally considered not legitimate," citing "minimal coverage," "difficulty cancelling policies," and "not ACA compliant," and advising readers to use the marketplace instead.

**Read: mixed confidence, and lower severity than issues 1 through 3.** At around 1.2% brand-directed, this is not a wall. But it is persistent across twenty months, and the brand's own document independently notes people searching "is Health for Moms legit." The last comment matters more than its rate suggests because it is a load-bearing, high-engagement post that hands other readers a ready-made case against the brand.

### Issue 5: an income floor nobody markets

Two comments name a lower income bound, which is the reverse of what most people expect from an affordability pitch. 2026-09-01: *"But if you make under 30k a year you don't qualify smh."* 2026-05-28: *"I make less than 30,000 bc I'm a student in school and don't qualify for this."* And a third, on 2025-08-03, reasons toward it: *"my income doesn't fall into the sweet spot. I don't make very much, just more than medicaid allows."*

**Read: thin, two direct reports out of 1,322.** But it is worth carrying because it is directionally consistent with how underwritten private plans are sold, and because it means the product's real audience is narrower than "moms." **Route to the brand to confirm whether an income floor exists and what it is.**

### What all five issues add up to

The product's genuine addressable buyer is considerably narrower than the brand's advertising suggests. Stacking the gates that are visible: she must live in a qualifying state, she must be medically healthy, she must not be pregnant or planning to be, and she may need to be above an income floor. The brand's own words for the product are "for moms" and "nationwide."

**This is the single most important thing in this audit, and it constrains what the brand can credibly claim.** A gap this wide between the promise in the ad and the answer at the gate does three kinds of damage: it burns spend on clicks that cannot convert, it produces exactly the public comments quoted above under the ads that are working hardest, and it puts the brand's most-used claims in a place where a regulator or a platform reviewer could reasonably ask questions.

One live signal that the platform side is not theoretical: two ad records in the lifetime cut show an `effective_status` of `DISAPPROVED`. (`verified`, ad pull.) The cause is not visible.

### The other side of the ledger, and how thin it is

An honest audit reports the good too. It is very thin. A semantic search for positive service experiences across all 1,322 comments returned **three** results above the similarity threshold, and only one is a genuine account of the service working:

- 2026-04-01, 1 like: *"I was connected to a very helpful agent. They weren't able to find a lower price for our particular situation but he was very kind and helpful and respectful."*

That is a good comment. It also says the agent could not beat her existing price. **The asymmetry between the volume of documented friction and the volume of documented satisfaction is itself a finding**, and it is exactly the gap a first-party review surface would close. The team has confirmed no review corpus exists. Standing one up would be the highest-value data move available to this brand.

## LTV expansion and the upsell cycle

**Almost nothing here can be verified, and the honest answer is that the brand holds all of it.** What follows is reasoning marked clearly as inference, plus a precise list of what to ask for.

**How the money works, as far as it can be reconstructed.** The consumer pays Health For Moms nothing. Revenue is `inferred` to come from the partner agency, either per lead delivered or per policy written, and which of those two it is changes everything downstream. `running-notes/brand-rules.md` records that unit economics were asked for at intake and not captured: no customer value, no gross margin, no lifetime value, no payback window, and no maximum tolerable cost per acquisition. Without a ceiling, "efficient" in this brain currently means "better than the account's own trailing cost per lead," not "profitable." (`stated`, brand rules.)

**Is the lead a one-time event or a recurring one?** This is the question that decides the whole business shape, and it splits cleanly:

- **For Health For Moms, the lead is almost certainly one-time.** A mom is matched once. There is no second match to sell her, no adjacent product in the line, and no visible re-engagement motion. (`inferred`, from the total absence of any second product or returning-customer motion in the account or the brand document.)
- **For the partner agency, the policy is recurring**, since a health plan renews and pays commission year over year. So there is real lifetime value in this system, but it may sit on the other side of the handoff.

**That asymmetry is the strategic centre of the business, and it is unresolved.** If Health For Moms is paid per lead, it is a volume business and cost per lead really is the whole game, exactly as the team has it set up. If it is paid per policy written, or on renewals, then lead *quality* is not a secondary gate at all, it is the primary one, and the account is currently being optimised on the wrong number. `running-notes/success-definition.md` already anticipates half of this by insisting a low cost per lead is only "gate one." The economics would tell the team how much gate two is actually worth. **Route to the brand.**

**The visible expansion paths, all marked as hypotheses.** There is no product line to expand into, so growth has to come from somewhere else:

1. **Widen who can qualify.** The biggest constraint on this business is not creative, it is the qualification gate. A plan option that accepts pregnant women or common managed conditions would convert traffic the brand is already paying for and already annoying. Whether that is possible depends entirely on the partner agency's carrier shelf. (`inferred` from the rejection evidence.)
2. **Add lines the same mom needs.** Dental, vision, life, and accident are the standard neighbours in this category and none appear anywhere in the account. Nothing suggests the brand has tried. (`inferred`.)
3. **Make the season work harder.** Open Enrollment on November 1 is the brand's one named promotional moment, with a two-month planning window, which means creative for it should already be in production as of this doc's date. (`stated`, Section 12.) The seasonal read that matters more, though, is the other one: because these are private plans sold outside the marketplace, **qualifying life events are a year-round entry point** in a way they are not for ACA plans. New baby, divorce, job loss, and going self-employed all appear as triggers in the brand's own persona work. A brand whose product is not actually gated to the November window, but whose marketing behaves as if it is, is leaving eleven months on the table. The brand's own document already names this as a "feast-or-famine" vulnerability. (`inferred`, resting on the private-plan structure plus the brand's stated triggers.)
4. **Fix the leak before adding anything.** The `quiz.healthformoms.com` path loses 74.1% of the clicks it is sent. No expansion play pays as fast as not losing three quarters of paid traffic. (`verified`.)

**Named blanks, all brand-routed:** revenue model per lead or per policy, revenue per lead, lead-to-enrollment rate, maximum tolerable cost per acquisition, whether renewals pay, and whether lead quality is measured anywhere at all.

## Use-case and need-state mapping

There is one service, so this maps need-states to **entry moments and messages**, not products to buyers. Per the persona method, nothing here is a persona claim. These are the intended uses the brand's own framing and funnel signal, not evidence about who actually buys. The real persona work happens in the persona docs, from buyer data, and the join between these moments and real buyers belongs there.

| Need-state | What she is trying to solve | How the product is meant to serve it | Where it holds or breaks |
|---|---|---|---|
| **The deductible is absurd** | Paying a premium every month and still paying everything out of pocket | The "$0 deductible option" is the direct answer | Strongest fit and the dominant conversation. **207 of 1,322 comments, 15.7%, mention "deductible,"** far and away the biggest theme in the corpus |
| **Coverage change forced on her** | Employer benefits shifting, a plan ending, a renewal spike | A fast alternative that does not require becoming an expert | Good fit. Year-round, not tied to November |
| **Life event opens a gap** | New baby, divorce, job loss, going self-employed | Private plans are not gated to the November window | Good fit in principle. **Breaks for the new-baby version**, since currently pregnant women are screened out |
| **Stuck in the middle** | Earning too much for Medicaid, too little for a comfortable marketplace plan | Positioned squarely at this gap | Genuine fit, and the brand runs creative on it. Complicated by the possible income floor |
| **Overwhelm and avoidance** | Has been meaning to deal with it for months | Four questions, thirty seconds, someone else does the work | The brand's cleanest promise, and the part it fully controls |
| **Distrust of big insurance** | Believes the system is rigged | The system-as-villain framing validates her before selling | Works as a doorway. Carries a risk, since a mom primed to distrust insurers who is then screened out or called by five agents has her prior confirmed |

**The emotional read, which the creative already knows.** The account's two winning openers sit in completely different emotional places. The dominant hook is calm and post-relief, a mother and baby on white bedding with "Wife of the year energy." The highest-attention hook is raw distress: "moms54-3" opens on a young woman with a red, tear-stained face saying *"Just got off a two hour call fighting for them to cover my newborn son's hospital stay,"* and it produced a 57.02% hook rate and a 13.66% hold rate, by far the best attention numbers in the window, on $1,283.69 of spend at a $29.85 cost per lead. (`verified`, ad pull.) So the account has proof that both the trigger moment and the resolved moment can stop the scroll. The calm one converts more cheaply at scale. The distressed one holds attention far better and costs more per lead. That is a real, unresolved trade the strategy work downstream should take up.

**Do not read a persona out of this table.** Delivery is 95.2% female and 81.2% aged 25 to 44, which is who Meta found, not who bought. (`verified`, ad pull.)

## Entry-point product hypothesis

**There is only one entry point, so the real question is which promise should open the relationship.** This is a hypothesis, marked as one throughout.

**Hypothesis: the entry point should stay the free match, but the opening promise should shift from the savings number to the qualification answer.**

The reasoning:

The current opener is a savings claim. Five ad groups sharing one hook line about saving $400 a month with a zero deductible carry roughly 68.6% of the account's spend, and the best of them clears the brand's "fantastic" cost-per-lead tier. On gate one, it works. (`verified`.)

But the product's real gate is not price, it is eligibility. Everything in the Known product issues section says the same thing: the moment of friction is not "is this a good deal," it is "am I allowed." Moms are arriving primed for a savings conversation and hitting a health questionnaire. The comments that hurt most are all versions of the same complaint, that the offer was not really for them.

So the tension the prompt asks to be named rather than resolved sits here, and it is sharp. **The easiest first yes and the most profitable first yes may point in opposite directions.** A savings hook maximises clicks and minimises cost per lead, which is the only gate Parker can see, and it is the gate the team currently manages to. A qualification-forward hook would almost certainly raise cost per lead by turning away people who cannot qualify. Whether that trade is good depends entirely on whether the brand is paid per lead or per enrolled policy, which nobody has told Parker. **If the brand is paid per lead, the current approach may be correct and this hypothesis is wrong.** That is exactly why the economics question is routed to the brand rather than answered here.

Two things can be said with more confidence than the main hypothesis:

- **The funnel choice is not a hypothesis, it is arithmetic.** Acquisition should run on `/save/` until someone explains what `quiz.healthformoms.com` is for. A 25.9% arrival rate against 87.3% is not a testing question. (`verified`.)
- **The brand's own guidelines already contain the fix, and the account is not using it.** The "State Angle CTA" is documented as the framework for cold audiences, the brand says it is the best performer, and the guidelines call the "Select States Classic" framing one that "converts WELL!" (`stated`, Sections 7 and 9.) A state gate is a qualification gate wearing a curiosity costume. It pre-qualifies while creating an open loop rather than closing a door. Yet in the current 90-day window the state angle is barely present: one ad group, "moms-53 3," runs an "Approved State List ✔️" opener, and it produced a $16.01 cost per lead in the brand's "good" band on only $1,761 of spend, while the savings hook took 68.6%. (`verified`, ad pull.) **The brand's stated best angle and the account's actual spend do not agree**, and that gap deserves to be put in front of the team before the November ramp.

## Open loops

**1. How many of the leads actually make it through the gate?**

The account bought 4,336 leads in 90 days at $22.67 each. The comment corpus shows a steady stream of moms being turned away at qualification for health, pregnancy, and possibly income, across fourteen months and 1,322 comments. Nobody on the Parker side can see what happens after the handoff.

*Pull: Tension.* Two sources cannot both be right as stated. The ads promise a product for moms and the funnel keeps telling moms it has nothing for them, and only one of those is the real conversion rate.

*Question:* What share of the leads Health For Moms delivers actually qualify and enroll?

*Why it is a loop:* Everything in this brain is currently optimised on cost per lead, because that is all Parker can see. If a large share of leads cannot qualify, then the cheapest ads may be the ones producing the most unusable leads, and the entire ranking of winners flips. **Brand-routed.** This is gate two from `success-definition.md` and only the partner agency has the answer.

*Territory: Product.*

**2. Where do the paid clicks on the second funnel domain go?**

One ad variant in the window pointed at `go.healthformoms.co/save/`, a different subdomain from the main site. It bought 690 link clicks and recorded 63 landing page views, so about nine in ten of the paid clicks never showed up, and its cost per lead was $273.23 against an account average of $22.67.

*Pull: Surprise.* Nothing in the rest of the account behaves this way. The ads pointing at `/save/` land 87% of their clicks, so a 26% arrival rate is a break in the pattern, not a variation on it.

*Question:* What is happening to the paid clicks that never reach the page on that domain?

*Why it is a loop:* If it is a broken redirect or a tracking gap, it is money already being thrown away and the fix is immediate. If the page is real and simply converts far worse, then the brand has been running two funnels of very different quality without a documented reason, and that decision needs an owner before the November ramp.

*Territory: Product.*

**3. Which mom can this product actually serve?**

The brand is called Health For Moms. The plans screen out women who are currently pregnant or planning to be, and screen out common health conditions. 38 of 1,322 comments name a pregnancy denial and 38 name a pre-existing condition denial, and the pregnancy ones carry more likes than almost anything else in the corpus.

*Pull: Tension.* The brand's name claims one audience and the product's underwriting admits a much smaller one, and the customers have noticed out loud.

*Question:* Which stage of motherhood can this product actually cover, and how big is that group?

*Why it is a loop:* Persona work is about to start from ad delivery data showing women aged 25 to 44, but delivery shows who Meta found, not who could qualify. If the product genuinely cannot serve women in or near their childbearing years, then a large share of the audience the brand is paying to reach can never convert, and both the targeting and the brand's own name are pointed at the wrong person.

*Territory: Personas.*

**4. What is the synthetic talent costing a brand whose main problem is trust?**

Several commenters call the creative AI-generated, unprompted, and tie it directly to distrust. One on 2025-07-25 wrote: *"This is the problem with AI online commercials. If you are using a fake person for your testimonial, it unintentionally sends a message to people that no real actual person would say this about your service. I think it's always better to have a real person. Especially with something that is famous for being a scam, like health insurance."* Another on 2025-08-08 simply replied to an ad: *"You don't qualify for Medicaid because you're an AI video.."*

*Pull: Gap.* The brand's documented weakness is legitimacy, its guidelines call for creative that sounds like a friend sharing a secret, and viewers are reading the people in the ads as fake. Nothing in the brand context acknowledges this.

*Question:* How are viewers reading the people in these ads, and what is that doing to whether they believe the offer?

*Why it is a loop:* Trust is the brand's binding constraint, not attention. Its hook rates are healthy. If the on-screen talent is quietly working against belief at the exact moment the viewer decides whether to hand over her phone number, then casting is a bigger lever than any hook rewrite, and it points the creator and production budget somewhere different.

*Territory: Creators and talent.*

## Appendix - Parker media links

All links preserved exactly as returned by Parker MCP.

**Ad account:** `HealthForMoms`, act `484897827497337`, brand `aed0ff06-555d-4f4f-9bf8-31178e2fb977`.

### Hero ad, 43.5% of 90-day spend: "Moms43 - 4 - V3"
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4

### Gate-one candidates, best cost per lead in the window
- "moms-63 2b", $13.29 CPL: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093361410519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399.mp4
- "moms-63 3e", $15.14 CPL: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093478820519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6a45457e776af311dfb45d100c093bab9d3f90c7575195dfd86b6260763f1670.mp4

### The state-angle ad, the brand's stated best mechanism: "moms-53 3"
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254787160519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e6225ca24b359ea0ab06bbeafe453b45496c1310c5a736ba3ea560045c6bd093.mp4

### The leaking funnel destination: "Moms Nahuel WV#1 - V9 - Copy"
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247373812940519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/645496c411d82a546a3e2deada69459c716615ad09f635ca0b978625c2778b37.mp4
- Landing page: https://quiz.healthformoms.com/#/indvfam

### Highest attention in the window: "moms54-3"
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247063711860519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/5a62b11062812d9509cb2cd8c95e89777a15d1a6ac1cdb1f6e9a92eb77f93a9d.mp4

### Historical statics with the unexplained funnel shape
- "IMG 6", $6.88 CPL: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120212962324800519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/14f1fb45d1b0308a5b25ce5cfdb6b2b7f9116c569643058dc4ba2d6965e51a55.jpg
- "5TH APR - Copy 29", $9.62 CPL: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120219260803030519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/45224b0b0e41a9bf1b7f5d5615b382462b10f5e321ab7875df4adcbb3870f17c.jpg
- "B1 - Copy 7", DISAPPROVED: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120216241083360519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/7e3133fccf8b205622146f7297669b76296123fb46177e5262ee89f0040ca8ba.jpg

### The `/save-cw` variant destination
- "OMC-Health for Moms-[B3-C17-V2] - Copy": https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120233032588900519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Landing page: https://healthformoms.co/save-cw

### Public source
- HealthForMoms terms page, naming Insurance Yeti, LLC as operator: https://healthformoms.co/privacy-policy-acn-9365-1408-4908

### Brand site pages that could not be opened this run
- https://healthformoms.co/ (blocked by network egress policy)
- https://www.healthformoms.co/save/ (blocked by network egress policy)
- https://quiz.healthformoms.com/ (blocked by network egress policy)
