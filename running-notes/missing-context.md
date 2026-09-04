# Missing context — the open questions

What Parker could not observe, could not reach, or was not told. Every entry here is an open
question, never a blocker. Prompts that hit one of these must label the affected claim
`data-limited` and say so plainly rather than filling the gap with a guess.

**Generated:** 2026-09-03 (Phase 0 surface test)

## Dark data surfaces — confirmed empty, not broken

These were tested with real pulls during Phase 0. They returned zero rows.

- **Customer reviews** — zero rows. The team confirmed this directly in Slack on 2026-09-03:
  *"we don't have reviews but you can pull from competitor reviews or health insurance Reddit etc."*
  **Substitution rule for this brand:** wherever a prompt calls for customer-review evidence, use
  Facebook ad comments (live and rich), Reddit, and competitor/category reviews instead, and label
  the source explicitly. Never present substituted evidence as this brand's own review corpus.
- **Post-purchase surveys** — zero responses. No survey platform connected and no CSV uploaded.
- **Competitor ad library** — no external brands tracked in the Parker app. The competitor branch
  and the external audit cuts are **deferred at the user's request** (2026-09-03), not failed.
  Adding rivals in the Parker app backfills this branch without redoing anything else.
- **Northbeam** — not connected. All attribution is Meta-reported. Read performance on Meta
  numbers and say so; do not imply multi-touch attribution.

## Live surfaces — for contrast

Brand context document, Meta ads (`HealthForMoms`, act `484897827497337`), Facebook ad comments,
the TikTok mining library (23 relevancy-scored videos), and Parker chat history (4 threads,
1 web + 3 Slack).

## Account shape — read this before any performance analysis

**This account is lead generation, not ecommerce.** Last 90 days: 136 ads, $98,276.68 spend,
**4,336 leads at $22.67 CPL**, and **zero purchases**. ROAS is 0 across the board because there
is no purchase event, not because the ads fail.

- Judge performance on **CPL, lead volume, CPM, CTR, hook rate and hold rate**. Never on ROAS,
  AOV, or purchase value.
- Audience skew is sharp: **95.2% female**, **81.2% aged 25-44**, **99.5% mobile**,
  60% Facebook / 39% Instagram.
- The business model is a match-and-consult referral to partner insurance agencies, not a
  direct sale, so "conversion" means a qualified lead handed to an agent.

## Brand intake — not yet captured

The Phase 0 brand intake was not run before the build began. These remain open until the team
answers them, and the build proceeds without them.

- Main business objective right now
- Primary campaign objective
- North-star metric and whether hitting its goal is the whole definition of success
- Secondary metrics they still weigh
- Whether higher spend wins when two ads in one ad set diverge
- Where they read performance (in-platform vs a third-party tool)
- Ad naming convention
- Brief template (would be saved verbatim to `briefs/_brief-template.md`)
- Who they consider real competitors, plus aspirational brands
- Unit economics: customer value, gross margin, LTV or payback window, max tolerable CPA

## Operational breaks the brain found but cannot fix — for the team, not for Parker

These are not research questions. Each one is a thing that is wrong right now, on live spend, and it needs an owner outside this brain.

### The quiz destination does not register arrivals — found 2026-09-04, urgent

`moms-53 3 - Copy` (three variants, `ADSET_PAUSED` today) points at **`quiz.healthformoms.com/#/indvfam`** and returned **9 landing page views against 511 link clicks** across 2026-06-06 to 2026-09-03 — a click quality of **1.76%**. Its sibling `moms-53 3` carries the **same creative, same hook, same body copy**, points at `www.healthformoms.co/save/` instead, and returns **76.12%**. `verified live`, `search_facebook_ads_sql`, 2026-09-04, Meta default attribution.

**Two possible causes and the data cannot separate them.** Either almost nobody who clicks actually lands on the quiz, or they land and the pixel does not fire on that domain. The first is lost spend; the second is blind measurement on every quiz-pointed ad this account has ever run. Both are urgent and neither is a creative problem.

**What it blocks:** no brief may be built on a figure sourced from a `quiz.healthformoms.com` ad until this is settled, because every conversion rate on those ads is currently unreadable.

**Who can answer it:** whoever owns the website and the Meta pixel. Parker cannot see server logs or pixel configuration.

**UPGRADED 2026-09-04 — the account ran the experiment itself, four times, and the result is not subtle.** A pull of every ad-name group created since 2026-08-01 that took $500 or more returned 14 groups. Inside those 14 are **matched pairs running the identical video file** — same `video_storage_url` hash, same text hook, same body copy — split only by landing URL. `verified live`, 2026-09-04, lifetime metrics.

| Ad-name group | Destination | Leads | Cost per lead | Landing page views / link clicks |
|---|---|---|---|---|
| `moms-63 2b` | `www.healthformoms.co/save/` | **417** | **$13.26** | 2,981 / 3,404 = **88%** |
| `moms-63 2b - Copy` | `quiz.healthformoms.com` | **6** | **$144.23** | 54 / 672 = **8%** |
| `moms-63 3e` | `www.healthformoms.co/save/` | **339** | **$15.46** | 3,014 / 3,531 = **85%** |
| `moms-63 3e - Copy` | `quiz.healthformoms.com` | **8** | **$67.15** | 30 / 344 = **9%** |

**Same creative. Same hook. Ten times the cost per lead on one pair, four times on the other.** The landing-page-view ratio is the mechanism: roughly 85 to 88% of link clicks register an arrival on `www./save/`, against 8 to 9% on the quiz. This is the cleanest evidence in the whole brain, because creative is held constant by the file hash and only the destination moves.

Two more quiz-pointed groups in the same cohort agree: `Moms Nahuel WV#1 - V9 - Copy` at **$75.75** a lead (234 landing page views on 903 link clicks) and `Moms36 - 3 - A - 2 - V4c - Copy` at **$20.08**.

**It still does not separate the two causes** — people not arriving versus arrivals not being measured — and that distinction decides whether this is wasted spend or blind measurement. But it does settle that **the quiz destination costs this account real money at real scale**, and it sizes it: on `moms-63 2b` alone, $865.39 bought 6 leads where the same video on `www./save/` was buying them at $13.26.

**All four quiz-pointed groups in this cohort read `effective_status: ADSET_PAUSED` as of 2026-09-04**, so the bleed appears to be stopped for now. That makes this a fix-before-relaunch item rather than an emergency, and it makes the standing rule firmer, not softer: **route new work to `www.healthformoms.co/save/` and do not send traffic to the quiz until someone establishes which of the two causes is real.**

This is the same shape as the `go.healthformoms.co` redirect break the open-loops roll-up routed to the operational owner on 2026-09-04, on a different destination. Two destination problems found independently is a pattern worth a single audit of every landing URL in the account rather than two one-off fixes.

### Fabricated social proof across seven static ad groups — found 2026-09-04, urgent

**What was found.** Seven static ad-name groups, **$35,234.91 lifetime spend, 2,871 leads at $12.27**, are built as mock X (Twitter) posts. Every one of them carries, inside the image itself:

- **A blue verified checkmark on an invented persona.** Three named personas across the set: "Cindie" `@cindie_mama_23`, "Cindy Green" `@thehealthymom34`, and "Grace Skagg" `@Motherooffthree`. None is a real verified account.
- **Fabricated engagement counts, printed as image text.** `B1 - Copy 7` shows *"390 Retweets 7,314 Likes 751 Bookmarks"* and *"333.3k Views"*. Five others show *"503 Retweets 24 Quotes 2.5K Likes"*.
- **A fabricated timestamp.** `B1 - Copy 7` reads *"23:51 • 30/05/2024 from Earth"*.

`verified live`, `search_facebook_ads_sql`, `adType: static`, `metricsMode: lifetime_only`, keyword sweep, pulled 2026-09-04. The account's own AI creative analysis describes them in exactly these terms without prompting — *"simulated engagement metrics," "artificial social proof," "a 'verified' persona adds a layer of simulated authenticity."*

The seven, by lifetime spend: `B1 - Copy 7` ($30,339.32), `15` ($2,125.47), `B2 - 10TH JUNE - Copy 1` ($1,877.94), `30th may moms 9 - Copy 6` ($615.52), `5TH APR - Copy 25` ($170.54), `30th may moms 9` ($53.91), `B2 - 10TH JUNE - Copy 2` ($52.21).

**Why this is a hard-rule problem and not a taste one.** The brand's own guidelines, in the section it heads "THIS SECTION IS NON-NEGOTIABLE," say **"No fabricated statistics."** Printed retweet counts, like counts, bookmark counts and view counts are statistics, and they are invented. The verification badge is a further claim — it asserts platform verification of a person who does not exist.

**Two of the seven carry a second breach each, on top of the fabrication.**

- `B1 - Copy 7` also carries the flat savings claim **"24% cheaper"** with no "up to," against the rule *"Savings claims: always 'up to 30%' — never drop the 'up to'."* Two of its five variants already carry a Meta status of DISAPPROVED, recorded earlier in the build.
- `B2 - 10TH JUNE - Copy 1` carries **"no gimmicks, no government red tape,"** against the rule *"No government/ACA references,"* which the brand explains as positioning itself in the private market and avoiding any association with government programs. **This is a third distinct live rule breach that nothing in the vault had recorded before today.**

**What it changes, and this is the strategic half.** `strategy/strategic-roadmap.md` Priority 2 is to restart the employer-plan switch message on the strength of the two statics that returned **3,817 leads at $11.79**. `B1 - Copy 7` is one of those two. **So Priority 2 is a rebuild, not a switch-flip.** The message is still proven and the direction still holds — what cannot be reused is the execution that carried it. Any brief serving Priority 2 must rebuild the creative without the fake platform frame, and must not treat the old cost per lead as a forecast, because the fabricated social proof is plausibly part of why it converted.

**RESOLVED 2026-09-04 — they are NOT delivering, and that lowers the urgency without changing the finding.** The open question was whether the `ACTIVE` ad-level status meant live spend. It does not. A `groupBy: ad` pull returns **`effective_status: CAMPAIGN_PAUSED` on every one of them**, and a 30-day window returns **zero rows — no spend, no impressions**. Across the trailing 365 days the whole set spent **$699.78 and bought 32 leads at $21.87**, so the $35,234.91 is almost entirely older money. `verified live`, 2026-09-04.

**So this is not money burning today. It is an asset library that must not be switched back on as it stands** — which is exactly the decision roadmap Priority 2 was about to make. The urgency is a creative-rebuild urgency and a compliance-record urgency, not a stop-the-spend urgency.

**One more thing the same pull turned up, and it is the useful half.** The `B1 samar- Copy` statics in this set carry headlines nothing else in the account does, and they speak the language the comment corpus actually uses:

- *"Finally found a health plan that doesn't make me Google "is a $7000 deductible normal?" at midnight."*
- *"I can handle tantrums. Insurance hold music? Not so much."*
- *"Switched to a mom-focused health plan and finally relaxed / saved on premiums."*

The first one is deductible-anxiety in the customer's own register, and "deductible" appears in **207 of 1,342** comments against "uninsured" in **2**. **The headlines are worth keeping; the fake platform frame around them is what has to go.** All four of these ads also carry the banned shared body copy ("saving you 20% or more" / "savings of 20% or more") and one carries the approval claim as its `ad_title`, so a rebuild strips the frame AND the block, and keeps the headline.

**Who needs this:** whoever signs off on creative and whoever owns compliance. Parker can see the ads and the brand's own rules; it cannot judge legal exposure and is not doing so here.
