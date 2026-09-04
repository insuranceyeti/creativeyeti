# Build log — Health For Moms cold start, 2026-09-03

Permanent provenance for the build. One entry per prompt run: the prompt, the source pulled,
the output path, and its review verdict. `BUILD-STATUS.md` is the live view; this log accumulates.

**Method version:** parker-brain `v15`
**Run id:** `e5c1cbe7-0bba-4a1e-8b7e-9bdc075777e1`
**Repo posture:** self-managed (see `running-notes/standard-sync.md`)

---

## Phase 0 — Repo & Scaffold

**Completed 2026-09-03.** Flat layout scaffolded; `parker-system/` mounted read-only as a
submodule pinned to v15; 26 skills, 2 review-gate agents, 2 checker scripts and the Parker
voice layer shipped into `.claude/`; `BUILD-STATUS.md` and `parker_config.json` written.

**Surface operability test** — every surface pulled, not merely pinged:

| Surface | Result |
|---|---|
| `get_brand_persona` | live, ~50KB brand context document |
| `search_facebook_ads_sql` | live — 136 ads, $98,276.68 / 90d, 4,336 leads, $22.67 CPL |
| `search_facebook_ad_comments_sql` | live, current through 2026-09-03 |
| `search_tiktok_videos` | live — 23 relevancy-scored videos |
| `search_chat_history` | live — 4 threads (1 web, 3 Slack) |
| `search_customer_reviews_sql` | **0 rows** — dark |
| `semantic_search_post_purchase_survey` | **0 rows** — dark |
| `search_competitor_facebook_ads` | **0 tracked brands** — dark, branch deferred |
| Northbeam | not connected |

**Known deviation from the runner.** The managed Parker repo
(`parker-brain/insuranceyeti-health-for-moms`) was provisioned but could not be reached from
the build session — the egress proxy injects git credentials only for repositories in the
session's authorized set, and `add_repo` refused it as a cross-tier add. The brain is therefore
self-managed in `insuranceyeti/creativeyeti`. Recorded in `running-notes/standard-sync.md`.
Parker Desktop guidance in the method docs does not apply to this brain.

**Brand intake.** Captured partially, after the scaffold rather than before the method mount.
Answers landed in `running-notes/success-definition.md` and `running-notes/brand-rules.md`;
unanswered items logged in `running-notes/missing-context.md`. The intake is never a gate.

---

## Phase 1 — Audit

### `audits-quarterly/90-day-performance-audit` → `audits/2026-Q3/90-day-performance-audit.md`

- **Sources:** two matched 90-day windows, six monthly windows for trajectory, created-time
  filtered pulls for net-new vs carryover, brand context document, chat history.
- **Methods loaded:** `ad-account-analysis`, `ad-metrics-glossary`, `killer-performance-ads`,
  `andromeda-v2` (per `expertise-routing.md`).
- **Findings:** spend down 73.5% QoQ ($374,508 → $99,267) at flat CPL ($22.65 → $22.64);
  one ad holds 43.3% of spend, four ads sharing one text hook hold 60.5%; hold rate collapsed
  11.09% → 3.83% spend-weighted while hook rate rose to 43.40%; in-window creative cheaper
  ($20.26 CPL) than carryover ($23.65).
- **Data limitations:** placement-level (Feed/Reels/Stories) not exposed by the tool, verified
  twice; reach and frequency not returned; ROAS refused as meaningless on a lead-gen account.
- **Review verdict: PASS.** All eight sections in fixed order, 25 claim labels, denominators
  held throughout, seven canonically-formed open loops, dates stamped, required Andromeda v2
  sign-off present. Two minor non-blocking notes: the exec summary omits a placement-movement
  line (defensible — only platform-level stability was available), and section six runs five
  analysis paragraphs against a two-to-three guideline.

### `personas/ad-account` → `source-pulls/ad-account.md`

- **Sources:** 90-day window (117 ad-name groups), lifetime cuts across 1,593 video and 529
  static ads, per-ad delivery breakdowns, full media analysis on 13 ads (transcript, AI
  creative analysis, creator demographic), four semantic sweeps hunting absences.
- **Findings:** top 13 of 117 groups take 92.7% of spend; POV hook family is 67.8% of spend and
  72.0% of leads at $21.37 CPL; static $12.30 CPL vs video $22.23; the state list is the
  qualifier at 0:33, not the variable — identical hook and state list span $13.29 to $30.43 CPL
  on the opening ten seconds; aspirational openers deliver 7-12% of spend to 45+ while grievance
  openers deliver 30-38%; ~100 tail groups averaged under $72 each in three months, including
  every non-white creator at $287 combined lifetime and four of five stated ICPs.
- **Critical finding:** `invitee_meeting_scheduled` returned zero data and only 42 `Call` events
  fired against 4,336 leads. Every CPL in this brain is the cost of a phone number, not a
  customer. Routed to the brand as open loop 8.
- **Review verdict:** pending.

### `personas/ad-comments` → `source-pulls/ad-comments.md`

- **Sources:** full comment corpus, 1,322 comments across 112 ad IDs and 79 ad names,
  2025-01-08 to 2026-09-03 (1,023 top-level, 299 replies), paginated in three pages of 500,
  plus six themed semantic passes and full creative on the 20 ads carrying 997 of the comments.
- **Note:** this is the brand's primary voice-of-customer source, since reviews and surveys are
  both empty. The substitution is recorded in `missing-context.md`.
- **Review verdict:** pending.

### `audits-quarterly/90-day-creative-strategy-audit` → `audits/2026-Q3/90-day-creative-strategy-audit.md`

**The Phase 1 anchor.** 14,357 words, eight sections plus open loops and a 24-entry media appendix.

- **Sources:** full 90-day set (136 ads, $98,276.81, 4,336 leads), full media analysis on nine of
  the top ten ads, a fresh `analyze_video_from_url` on the tenth because no stored analysis
  existed, all 92 in-window ad comments, brand context, chat history.
- **Methods loaded:** `killer-performance-ads`, `ad-account-analysis`, `hooks`, `ad-formats/`,
  `iterations`, `persona-research-and-creative-strategy-process`, `creative-strategy-fundamentals`,
  `emotional-delivery-and-timing`.
- **Note on method:** no prior audit exists, so rather than write a snapshot the agent pulled the
  preceding 90-day window directly to build trajectory. That produced the audit's largest finding.
- **Findings:** spend fell 73.8% from $375,185.71; ad count fell 460 → 136; CPL moved 0.04%.
  Anger went from 55.2% of spend to 2.6% — the five "Health Insurance is a scam" ads that carried
  $120,386.57 at 14-17% hold rates now have zero spend. One ad is 43.5% of spend, the top ten are
  88%. All 136 ads are video; zero statics. POV holds 69.8% of spend. Not one top-ten ad clears an
  8% hold rate against the craft floor of 12%. 66 of 92 comments sit on the single top ad, and 50
  of 92 are a bare "Help" — a qualification wall the creative never mentions.
- **Review verdict: PASS.** All eight sections in fixed order with exact output-spec headings;
  exactly ten deep dives each inside the 2-4 analysis-paragraph band; the media trap cleanly
  avoided (ad 4 had no stored analysis, so the agent ran a fresh `analyze_video_from_url` and
  marked it verified rather than reasoning from the ad name); zero tables, zero parentheses in
  the body; four canonical open loops across all four territories; arithmetic held on every
  spot-check. Sign-offs: the reviewer grepped all six routed docs and found none mandates one,
  so zero required and zero present is correct rather than a gap. Two soft spots noted, neither
  fail-level: labelling sits at claim-cluster rather than per-sentence level, and one
  interpretive clause arrives in section two which is specified as purely descriptive.

### `personas/ad-comments` — full findings

- **Dominant identity is not the one the creative addresses.** The creative speaks to an uninsured
  shopper; the commenter is a mom who already has insurance and is still broke. 160 comments across
  17 ads post their own deductible figure and treat the ad's $6,000 as an opening bid to beat.
  Most-liked comment in the corpus (47 likes) ends "I want the 1990's back."
- **The brand's own name is the setup for the joke.** 42 comments across 15 ads over 14 months say
  Health For Moms will not cover a pregnant woman. **This objection appears nowhere on the brand's
  stated objection list** in its context document, and it kills the stated ICP "Nicole," described
  there as a 41-year-old with a seven-month-old.
- **The top ad's central claim is publicly corrected as wrong.** 103 comments across 13 ads,
  including self-identified brokers and medical billers, say the ad describes an out-of-pocket
  maximum, not a deductible.
- **Rival agents farm the comments.** 39 comments across 10 ads are competing agents pitching under
  the brand's own creative; 17 of them on the single highest-spend ad.
- **Recognition is rare and misfunded.** ~12 recognition moments in 1,322 comments, nearly all on
  one skit format that has spent ~$3,400, while the deductible-vent family that earns argument has
  spent over $94,000.
- **Limits:** `author_name` is null on all 1,322 rows, so no claim is about people, only comments.
  Nothing can be checked against a confirmed buyer. All identities capped thin-to-mixed, never
  verified.

### Note on a small cross-doc variance

The performance audit reports the spend contraction as 73.5% ($374,508 → $99,267); the creative
strategy audit reports 73.8% (from $375,185.71). The two used slightly different window and
grouping definitions. Both agree on magnitude and direction; neither is wrong. Flagged here so a
later reader does not treat it as a contradiction.

### `brand-profile/brand-identity-analysis` → `sub-context-docs/brand-identity-analysis.md`

- **Findings:** the brand's non-negotiable claim rule ("always 'up to 30%', never drop the
  'up to'") is broken across **69.0% of lifetime static spend** — nine of the ten highest-spending
  statics carry a flat "saving you 20% or more" ($116,622.92), and a "24% cheaper" testimonial
  headline runs on three more ads worth $29,814.72, **two of which Meta has marked DISAPPROVED**.
  Currently-scaling video transcripts hold the qualifiers correctly, so this is legacy copy
  propagating rather than a live drafting problem.
- **Self-echo found:** the canonical ICP "Jen" is word-for-word the "Bucket 2 — Protective
  Planner" text Parker wrote in Slack on 2026-09-03, minus its opening demographic line, and is
  the only ICP with no trigger attached. Routed to `brand-self-echo-detection` for independent
  verification rather than accepted.
- **Team instruction overrides written guidelines:** *"honestly single moms are fine just as long
  as we also use lingo about them not being broke"* contradicts the guidelines' "married or
  partnered" ICP criterion. The typed instruction is the more recent signal.

### `brand-profile/website-and-product-audit` → `sub-context-docs/website-and-product-audit.md`

- **Environment limitation, material to the foundation.** `healthformoms.com`, `healthformoms.co`
  and `quiz.healthformoms.com` are all blocked by this environment's network egress proxy,
  confirmed by both WebFetch and curl. Every website-derived fact is therefore secondhand through
  the brand context document and marked `stated`, never `verified`; the site's visual register is
  a named blank. Re-running this doc from an environment that can reach the site would close the
  gap — it is the single biggest environment-caused weakness in this build.

### In flight

`90-day-diversity-audit`, `monthly-hook-audit`, `brand-identity-analysis`,
`customer-journey-and-persona-discovery`, `website-and-product-audit`, `voc-corpus-profile`.

---

## Correction — quiz destination figures, 2026-09-04

`sub-context-docs/website-and-product-audit.md` reported the `quiz.healthformoms.com` destination
as 903 link clicks against 234 landing page views at a $75.72 CPL. **That was wrong.** The
monthly performance report independently reached a different conclusion, which prompted a direct
verification pull.

**Verified 2026-09-04** via `search_facebook_ads_sql` filtering `landing_url contains "quiz."`,
lifetime, no date window: **26 ads, $138.27 lifetime spend, 72 clicks, 57 link clicks, 25 landing
page views, 2 leads, $69.14 CPL.** All 26 created 2026-09-02 or 2026-09-03.

The quiz destination is a brand-new test with negligible spend, not an established leak. Its CPL
rests on 2 leads and cannot be judged. A correction block has been inserted at the top of the
affected document so the wrong figure cannot propagate into Phase 2.

**The `go.healthformoms.co` finding is unaffected and independently confirmed twice** — by the
monthly hook audit (690 link clicks, 63 landing page views, $273.15 CPL) and the monthly
performance report (August: 11 ads, $2,046.40, 6 leads, $341.07 CPL, 1,103 link clicks to 77
landing page views, 7.0% landing rate against 84.6% account-wide, same video file at $19.22 on
the working destination and $271.90 on the broken one).

**Process note.** This is exactly the failure the per-output review pass exists to catch, and the
website-and-product audit had not yet been reviewed when its figure was relayed. Downstream
syntheses must not consume an unreviewed document. Tightening that ordering is the lesson.

---

## Correction — Open Enrollment history, 2026-09-04

`audits/2026-Q3/90-day-performance-audit.md` stated the account begins in early 2026 with no prior
Open Enrollment in the data. **Both halves were wrong.** `marketing-calendar-and-campaigns.md`
established from 23 live pulls that ads exist from 2024-12-05 and month-level metrics are readable
from 2025-09-01, covering the full 2025-11-01 OE window. That audit's open loop 7 is answered
rather than open. A correction block sits at the top of the affected document.

This is the second cross-document correction of the build, and both were caught by a later prompt
reading a live source, not by the review pass. That is the review backlog showing its cost. The
backlog is now the gate before any Phase 1 synthesis or Phase 2 work.

## Documents completed before the rate-limit pause

- `brand-profile/marketing-calendar-and-campaigns` → `sub-context-docs/marketing-calendar-and-campaigns.md`
  November is real but roughly efficiency-neutral; **December is the unplanned risk** — the most
  expensive CPM of thirteen months at $29.34, CPL up 39.8%, landing-page-view-to-lead down
  18.7% to 14.2% on largely unchanged creative, reading as Marketplace traffic under the
  December 15 deadline hitting a private-plan funnel that cannot qualify it. November 2025 took
  5.4% of thirteen-month spend; March to May 2026 took 58.9%, April alone 4.6x November, and March
  scaled to 3.9x February **while CPL improved**. Across all 2,122 lifetime ads, "deadline" appears
  in zero, "mother's day" in zero, "subsidy" in three totalling $379.92. 58 days to OE with 125 ads
  built since August 1, all on the same POV savings hook — a volume ramp, not a seasonal one.
- `audits-quarterly/quarterly-whitespace-analysis` → `audits/2026-Q3/quarterly-whitespace-analysis.md`
- `personas/customer-reviews` → `source-pulls/customer-reviews.md` (honest named blank)
- `personas/post-purchase-surveys` → `source-pulls/post-purchase-surveys.md` (honest named blank)
- `personas/brand-reputation` → `source-pulls/brand-reputation.md`

All five: review verdict pending.

---

## Correction 3 — the quiz figures resolved by direct pull, 2026-09-04

The earlier correction said the "903 link clicks / 234 landing page views / $75.72 CPL" figures
were wrong. A direct pull has now established **exactly what they are**, and the answer is more
useful than "wrong":

They are **two destinations summed together** on `Moms Nahuel WV#1 - V9 - Copy`:

| Variant destination | Spend | Link clicks | Landing page views | Landing rate | Leads | CPL |
|---|---|---|---|---|---|---|
| `go.healthformoms.co/save/` | $1,639.35 | 690 | 63 | 9.1% | 6 | $273.23 |
| `www.healthformoms.co/save/` | $404.23 | 213 | 171 | 80.3% | 21 | $19.25 |
| **summed (the wrong figure)** | $2,043.58 | **903** | **234** | 25.9% | 27 | **$75.69** |

903 = 690 + 213. 234 = 63 + 171. $75.72 is the blend of a broken destination and a working one,
presented as the quiz destination's own CPL. The quiz had nothing to do with it — that variant
carried $0.94 lifetime.

The parent `Moms Nahuel WV#1 - V9` on `www.` is healthy: $17,723.91, 7,196 link clicks, 6,198
landing page views (86.1%), 635 leads, $27.91 CPL.

**The real finding survives and sharpens:** the collapse is entirely `go.healthformoms.co`, the
same creative on `www.` converts normally, and `quiz.healthformoms.com` is a separate brand-new
test at $138.27 lifetime that must be treated as unmeasured.

The canonical correction block is now at the top of all four affected documents:
`source-pulls/ad-account.md` (the origin), `sub-context-docs/website-and-product-audit.md`,
`sub-context-docs/customer-journey-and-persona-discovery.md`, and
`sub-context-docs/marketing-calendar-and-campaigns.md`.

**Root cause for the record:** the origin was an aggregation error in `source-pulls/ad-account.md`
that attributed a group-level sum to one destination. Every downstream document inherited it by
citation. The per-output review pass would have caught it at the source had it not been backlogged.

## Review verdicts — first two batches, 2026-09-04

**Audits batch:** `monthly-hook-audit` **PASS**. `quarterly-whitespace-analysis` **PASS**.
`90-day-diversity-audit` **FAIL** — missing proof-of-read sign-off lines for `iterations.md`,
`visuals.md` and `creative-strategy-by-brand-size.md`, all of which it demonstrably used and cited.
`monthly-organic-tiktok-audit` **FAIL** — same shape, missing sign-offs for `adapting-scripts.md`
and `visuals.md`. Every other requirement met in all four.

**Brand foundation batch:** `brand-identity-analysis` **PASS** (two minor defects: `refresh_by`
stamped at 180 days where `refresh-cadence.md` puts it in the annual tier and the prompt itself
says quarterly — a prompt contradiction to reconcile upstream, not a doc fault; and three craft
reads that run past "present, do not judge" without the observation mark).
`competitive-landscape` **PASS**. `marketing-calendar-and-campaigns` **FAIL**,
`customer-journey-and-persona-discovery` **FAIL** — both on the quiz figures, now corrected above.
`category-and-market-research` **FAIL** — missing the `seasonality.md` sign-off, and two open loops
carry a closure path the open-loops core block explicitly bans.

**Method note.** The reviewer established which method docs actually mandate a sign-off by grepping
the doc bodies rather than inferring from the routing table. Only `iterations.md`,
`adapting-scripts.md`, `visuals.md`, `andromeda-v2.md` and `creative-strategy-by-brand-size.md` do.
That check cleared two documents that would otherwise have read as failures.

## Review verdicts — batch 3, source pulls and voice of customer, 2026-09-04

**PASS (8):** `ad-account`, `ad-comments`, `reddit`, `brand-self-echo-detection`, `customer-reviews`,
`post-purchase-surveys`, `voc-objection`, `voc-pain-phrase`.

**FAIL (1):** `voc-corpus-profile` — quote provenance. The prompt requires a row id on every quote;
roughly 30 of ~48 quotes in the Language and creative-asset index carry none, and the doc declared
the shortcut rather than meeting the rule. This is the one guarantee that document exists to give
every downstream pass, so it is a real fail, not a nit.

**Cross-cutting findings from this batch, all worth keeping:**

- **No sign-off was owed anywhere in this set.** The reviewer grepped the whole
  `creative-strategy-context/` tree and established that exactly ten docs carry a sign-off RULE:
  `static-ad-design`, `seasonality`, `advertising-to-older-audiences`, `non-problem-solution-creative`,
  `creator-briefs`, `creative-strategy-by-brand-size`, `legal-ai-ugc`, `ai-static-ad-generation`,
  `selecting-ads-to-iterate-on`, `andromeda-v2`. None is routed to persona source pulls or VoC.
- **The identifier trap was avoided cleanly.** All 48 `review_id` values in voc-objection and all 29
  in voc-pain-phrase are full 36-character SQL `comment_id` UUIDs, no duplicates, no semantic ids.
- **No `strong` mark appears on any VoC snippet**, correctly, since one source type cannot earn it.
- **The three verified-blank documents refuse substitution explicitly.** `customer-reviews` states
  "This doc is not the place for that substitution"; `post-purchase-surveys` states "Padding it with
  comment data would hand the persona synthesis a false top tier." That is the right instinct and it
  protects the persona confidence ceiling downstream.
- **The one-question rubric is broken in five loops** across four documents — stacked questions or
  either/or splits. Routed to repair.
- **Two numbers to reconcile:** a 90-day spend figure differing by $0.13 between two documents
  ($98,276.68 vs $98,276.81 — the API's own `period_summary` total is authoritative at $98,276.68,
  the other is a summing artifact from 117 ad-name groups), and a stale "34 blocks" where there are
  48 in voc-objection.
- **A contested confidence call:** three organic verdicts in `brand-self-echo-detection` are marked
  `strong` while the doc's own limitations say every organic verdict is single-source. The prompt
  defines strong as requiring source independence. Downgraded to `mixed` in repair; the timing
  evidence itself is good and stays.

**Running review tally: 12 pass, 6 fail, across 18 of 24 documents.** Two repair passes are in
flight. Remaining unreviewed: the three documents built after the batches were launched.

## Repair pass 1 complete, and a rule clarified — 2026-09-04

**Repaired:**
- `90-day-diversity-audit` — three verified sign-offs appended for `iterations.md`, `visuals.md`
  and `creative-strategy-by-brand-size.md`, each use checked against the source passage first.
- `monthly-organic-tiktok-audit` — two verified sign-offs appended for `adapting-scripts.md` and
  `visuals.md`; `visuals.md` also added to `knowledge_docs_read`, which had used it without
  declaring it (the mirror image of the Andromeda defect).
- `category-and-market-research` — two banned closure sentences cut from loops 3 and 4.
- `marketing-calendar-and-campaigns` — `andromeda-v2.md` **removed** from `sources_read` rather
  than signed off, because it appears nowhere in the body. Correct call: a sign-off is a
  proof-of-read, so the fix for "declared but unused" is to undeclare, never to stamp.
- `brand-identity-analysis` — three unmarked observations marked in the document's own form.

**Rule clarified — what counts as a required sign-off.** The repair agent flagged an inconsistency
in the instruction it was given, rather than following it into an incoherent result. It was right.

`expertise-routing.md` defines the sign-off as **the terminal line**: *"Many of these docs end with
a required sign-off line ('This is everything I know about X'). That stamp is a proof-of-read."*
It does **not** define it as a `**RULE:**` directive. Under the terminal-line definition both
`seasonality.md` and `creative-strategy-by-brand-size.md` are owed a sign-off; under a strict
`RULE:` grep, neither is. Treating them differently was the incoherence.

**Decision: the terminal-line definition governs, and explicit `RULE:` directives are additional,
not exclusive.** The union of both mechanisms is the correct set. Accordingly the
`creative-strategy-by-brand-size` sign-off stays in the diversity audit, and the missing
`seasonality.md` sign-off has been appended to `category-and-market-research.md`, matching the
precedent already set by `marketing-calendar-and-campaigns.md`.

**Also flagged, not a defect but a gap in auditability:** `90-day-diversity-audit` carries no
`knowledge_docs_read` frontmatter field at all — only `data_sources_read` — so its method-doc use
cannot be audited against a declared list in either direction. Its three uses were verified by
reading the cited passages against the source docs instead. Worth adding the field on a future
refresh so this document is auditable the way its siblings are.

## Repair pass 2 complete — 2026-09-04

- **`voc-corpus-profile` (the one FAIL) is fixed properly.** 27 quote bullets resolved to real SQL
  rows via live lookup, each given its real `comment_id`, ad name and date. **Zero removed** — every
  un-sourced quote resolved to a genuine row. The truncated id `b7aa4d37` expanded to its full UUID,
  and the declared-shortcut sentence deleted now that the rule is actually met. The index carries 49
  row-id citations and zero un-sourced bullets. Two lookups needed a second pass because the database
  stores curly apostrophes where the document used straight ones.
- **Five stacked open-loop questions split** across `ad-account`, `ad-comments`, `voc-objection` and
  `voc-pain-phrase`, each cut to the half its own justification says drives the decision.
- **`voc-objection` stale count** corrected 34 → 48, verified by a direct block count (48 snippet
  blocks, 48 null identity tags, 48 null behavioural tags).
- **Cross-doc counts reconciled** in `voc-pain-phrase` — a line now records that `voc-objection`'s
  stricter re-derivation returns 36 and 42 because it drops rows describing the commenter's existing
  plan, while the ad spreads (15 and 17) agree exactly. Both numbers stay visible.
- **Three confidence marks downgraded** `strong` → `mixed` in `brand-self-echo-detection`. The timing
  evidence stays exactly as written; the mark cannot, because `strong` requires source independence
  and this brand has one corpus it controls the language environment of.

### Repair 4's premise failed live verification — and that is the finding

The instruction said the authoritative 90-day spend was **$98,276.68**. The agent pulled
`period_summary` twice for 2026-06-05 to 2026-09-02, grouped two different ways, and got
**$98,277.97**. Leads (4,336) and CPL ($22.67) match the documents exactly, so only spend moved — by
**$1.29** — which reads as a **Meta restatement** since the 2026-09-03 pull the documents were built
on. The agent refused to write an unverified number and recorded both readings.

`ad-account.md` is set to $98,276.68, which is the correct as-of-2026-09-03 reported total and
reconciles with `post-purchase-surveys.md`; the $98,276.81 it previously carried was genuinely a
summing artifact. Its `data_limitations` now records both readings, the $0.13 group-rounding gap, the
$1.29 restatement, and the standing rule: **never re-derive spend by summing ad-name groups — read
the reported `period_summary` total.**

**Standing lesson for this brain:** Meta restates historical spend. A figure stamped on one date will
not reproduce exactly on another, and that is not an error in either document. Any figure carried
between documents must carry its as-of date.

### Flagged, deliberately not changed

- A fourth `strong` mark in "Confirmed organic of note" ("peace of mind") rests on the semantics of
  two comments arguing against the ad rather than the timing argument that made the other three
  untenable. Same single-source caveat arguably applies. Flagged, not acted on.
- Six `strong` marks earlier in the same document grade brand-**origin** verdicts sourced from the
  brand's own document — a different evidence class, correctly left alone.
- Composite narrative bullets in the corpus-profile index quote several rows inside one argument;
  they are thread-level reads, not single-quote bullets, and adding inline ids would have meant
  rewriting them.
- Curly-versus-straight apostrophes in some quoted text. Real, minor, and fixing it would mean
  touching verbatim quote text.

## Note on commits — for anyone reading this log later

Build agents are instructed **not** to run git. The orchestrator commits centrally, on its own
cadence, which means an agent's files can move from untracked to committed between its last write
and its report. Several agents flagged this as a possible concurrency problem. It is not — it is the
design. Content was verified byte-identical in each case. No agent ran a git command.

## Corpus denominator moved mid-build

Documents written on 2026-09-03 pin the ad-comment corpus at **1,322**. Documents written on
2026-09-04 re-probed it live and found **1,342** — twenty comments landed late on 09-03. Both are
correct as of their own date. Later documents recompute their own percentages on 1,342 and carry
upstream figures with the 1,322 denominator attached. This is the same as-of-date discipline the
Meta spend restatement forced, and it now applies to the comment corpus too.

## Correction 4 — the format-age-lever figure was window-scoped, 2026-09-04

The orchestrator briefed the personas pass with "Skit reaches 45-54 at 34.7% of its spend, POV at
9.4%" as though it were a stable account fact. It is the **90-day** cut, and it rests on only
**$712.20** of Skit spend. The lifetime cut, on $32,935.04, is **23.9% / 8.6%**.

The direction is solid either way — Skit reaches the older band roughly three times as heavily as
POV — but the sharp number is not, and a recommendation sized off $712 of spend would be
overconfident. Both tables are carried in `personas/personas-profile.md` with the denominators
attached.

**Pattern worth naming.** This is the fourth time a build agent has corrected a figure the
orchestrator handed it as settled: the quiz destination attribution, the Open Enrollment history,
the 90-day spend total, and now this. Each was caught because the agent re-pulled rather than
trusting the brief. The fidelity contract's instruction to pass a pointer and not a retelling is
doing exactly what it was written to do, and the orchestrator should window-scope every figure it
passes downstream.

## Persona judgment calls recorded

- **The employer-plan captive was demoted from persona to behavioral signal**, despite
  `quarterly-whitespace-analysis.md` naming her the highest-value persona. She fails the durability
  test. She is filed as the highest-commercial-value *signal* with the reasoning stated, rather than
  promoted to a persona the creative would then be built around.
- **No persona was made of the pregnancy or chronic-condition groups.** A persona requires a buyer,
  and the product screens both out. They appear instead as a named recruitment cost — the brand is
  paying to reach people it cannot sell to.
- **The lifecycle document discards the standard five-stage lens** for a six-stage variation,
  because a lens assuming purchase, repeat and subscription would be fiction in an account with zero
  purchase events.
- **The Jen contamination is confirmed harder than briefed:** an exact substring match at offset
  4268 against Parker's own Slack text, verified programmatically. Jen is also visibly a different
  shape from the other four ICPs — four sentences with no city, spouse, age or dollar figure, where
  the others run hundreds of words carrying all of them.

---

## The `go.healthformoms.co` conclusion is UNDER INVESTIGATION — 2026-09-04

**Do not treat the "broken destination" conclusion as settled.** Several documents in this build
state that `go.healthformoms.co/save/` is losing roughly nine in ten clicks, and the orchestrator
relayed that to the user three times with confidence. A live pull on reconnection complicated it.

**What is certain:** across **40 active ads** on that subdomain — not 11, as an earlier document
said — landing page views run at **8.7% of link clicks** (5,392 to 468) and click quality sits at
**8-11** against 80-90 on `www.`. That pattern is universal on the subdomain.

**What is now in doubt:** whether clicks are actually being lost. The CPL spread across those same
40 ads is enormous and several perform well — `Yeti State Angle - 1 - V3` produced **80 leads at
$14.70** on 800 link clicks reporting only 92 landing page views. If nine in ten clicks genuinely
evaporated, that ad could not exist.

**The decisive test is leads per link click**, which bypasses the suspect metric entirely. A
hypothesis and validation are running now under `hypotheses/` and `validations/`, following the
open-loops-advance and open-loops-validate skills, including a matched-pair analysis by `media_hash`
across the two destinations and a check on whether the campaign (`Internal - ABO - TEST` versus
`USHA - CBO - OTP`) explains the CPL spread better than the destination does.

**Until that resolves, the honest statement is:** the `go.` subdomain does not report landing page
views correctly, so every ad pointed at it is being judged on broken funnel data — which is why some
look catastrophic and some look excellent. Whether that is only a measurement fault or also a real
funnel loss is unresolved.

**Process note.** This is the second time a confident conclusion about this destination has needed
qualifying — the first was the quiz misattribution. Both came from reading a derived or aggregated
metric as though it were a direct observation. The lesson for this brain: when a metric looks
catastrophic, check what it is actually derived from before acting on it.

## RESOLVED — the `go.` subdomain, 2026-09-04. Verdict: INCONCLUSIVE, and that is the right answer.

The premise that the 40 `go.` ads are one population is **wrong**, and that is what broke every
earlier reading. They are two cohorts with zero overlap: **24 created 2026-03-06 to 03-13** (almost
all `Internal - ABO - TEST`) and **16 created 2026-08-17 to 08-31** (all `USHA - CBO - OTP`).

**Leads per link click** — the ratio that bypasses the suspect metric. Note Parker's own
`click_to_leads` field divides by *all* clicks rather than link clicks, so it is not this number and
had to be computed by hand:

| Cohort | Link clicks | Leads | Leads / link click |
|---|---|---|---|
| `go.` March (Internal - ABO - TEST) | 2,854 | 248 | **8.69%** |
| `go.` August (USHA - CBO - OTP) | 2,196 | 18 | **0.82%** |
| `www./save/` lifetime | 288,916 | 30,702 | **10.63%** |
| `www./save/` created on or after 2026-08-01 | 12,551 | 1,192 | **9.50%** |

**Matched pairs by `media_hash`** — four video files that ran to both destinations: `www.` converts
1,510 leads on 16,186 link clicks (**9.33%**); `go.` converts 18 on 2,188 (**0.82%**). An **11.3x
gap on identical creative**. `moms-53 3` took 511 link clicks to **zero** leads on `go.` while
converting at 5.79% on `www.`

**The number that splits the cohort is leads per landing page view.** The account's normal is 8-14%.
March `go.` returns **82.9%** (248 leads from 299 recorded views), which is impossible — the counter
is missing arrivals. August `go.` returns **11.5%** (18 from 156), which is dead normal — there the
view counter behaves truthfully.

**So it is both, and it differs by cohort:** a long-standing page-view counting fault that has
always been harmless, plus a real lead collapse confined to the August cluster.

**`click_quality` is NOT independent evidence.** It is exactly `100 × landing page views ÷ link
clicks`, reproduced to two decimals on seven ads (63/690 = 9.13, 92/800 = 11.50, 2981/3404 = 87.57,
6198/7196 = 86.13). **Five documents in this build cite it alongside the landing-page-view ratio as
a corroborating second witness. It is the same witness.** Those citations must be corrected — this
is a build-wide defect, not a single-document one.

**Why the verdict is inconclusive rather than confirmed:** campaign, creation date and destination
are perfectly collinear in the failing cell. `USHA - CBO - OTP` holds 2,209 link clicks and 2,196 of
them are the `go.` ads, so the campaign's number *is* the destination's number. Exactly one of four
cells fails — `go.`x August. `go.`x March worked and `www.`x August worked, so it is neither the
domain alone nor the date alone, and nothing in this account separates them.

The archived "leaks" verdict is **refuted as a general claim about the subdomain** and is
**better supported for the August ads specifically** than it ever was.

## Phase 1 fully closed — 2026-09-04. And a live change to record.

`audits/2026-Q3/gaps-opportunities-inspo.md` completes Phase 1 at **51 documents**.

**A live pull contradicted every upstream document, and the agent recorded the conflict rather than
smoothing it.** `search_competitor_facebook_ads` mode `brands` now returns **`totalCount: 1` —
Ethos**, 2,090 ads with 2,073 analysed. Every document written earlier the same day states the
tracked set is empty, and each verified that live at the time. So the set changed during the build.

The agent treated Ethos on what its library actually shows — a creative competitor one product over,
not a market rival — and noted that the relationship-type filter returns it under both `competitor`
and `inspo`, so the team's own tag cannot be read from that surface. That is the right handling:
neither ignoring the new data nor overreading one brand into a competitive set.

**Implication for the deferred branch:** the competitor branch and the six external audit cuts remain
deferred by the user's decision, but the blocker has partially lifted. One tracked brand is not a
competitive set, and Ethos sells life insurance rather than health, so it does not answer the
competitive question. Worth raising with the user rather than silently reopening the branch.

**The synthesis's diagnosis, worth carrying into Phase 2:** the field is not rival advertisers, it is
the alternatives mothers name themselves, and the category's attention sits on the one buyer
underwriting screens out. So the leverage is **restarting what the account already proved**, not
inventing what nobody has run. Its sharpest structural read: the organic field mirrors the problem
and never resolves it, the paid field resolves it and never mirrors it, **and the join is empty.**

## Correction 5 — "format is the age lever" does not survive opening the tag, 2026-09-04

Three documents, and the orchestrator three times, reported that **format** acts as an unintended age
lever — Skit reaching women 45+ far more heavily than POV. The number was corrected once already
(34.7% was the 90-day cut on $712; lifetime is 23.9%). The Phase 2 persona pass has now overturned
the **causal reading** as well.

Two ads both tagged `Skit` deliver **40.9%** and **12.4%** of spend to women 45+. The format tag does
not predict the age skew. The `Moms36` confession pair carries **56.9% of all Skit spend** and
nearly all of the age lift. **The lever is a woman talking straight to camera about her own bill —
a creative device — not the skit format.** Filed as an open loop.

This matters for what gets recommended. "Fund more Skits" would have been the wrong instruction and
would have spent against a tag rather than against the thing that works.

**Second correction from the same pass:** the $11.96 employer-plan statics sent **83.4%** of their
money to women 25-44, so that message belongs to the flagship persona, not to both as the vault
files it.

**Third:** the vault's "$34.21 older-woman ad" is one of two files totalling $144.07. The unnamed
sibling put **53.4%** of its spend on 45+, the highest share in the account.

**Standing lesson for this brain, now on its fifth instance:** an AI format tag is a label applied to
creative, not a property of it. Open the tag and look at the ads before spending against it.

## Phase 2 — the WHO call

`strategy/persona-strategy-input.md`. **Position: lead against `pays-and-still-owes`, and change the
premise rather than the audience.** The account already puts **77.0% of lifetime money on women
25-44** — it simply talks to her as though she has no insurance. Her real message, *you are allowed
to decline your job's plan*, bought **2,580 leads at $11.96** across $30,845.69 and is **switched
off**. A sentence change inside an audience already reached is the cheapest high-leverage move
available.

**The 45+ woman is a funded, sized bet, not the lead.** She is the most attentive audience the
account has and has never had an ad built for her, but she is about a fifth of delivery and falling,
and reaching her costs **41.5% more per lead** on the only gate anyone can see. Under the team's own
efficiency-first sequence a bet is defensible; a lead call is not.

**Deprioritize the peaceful-outcome montage:** $110,205.90 lifetime, **3.28% hold against a 12%
floor**, and "wife of the year" returns 0 of 1,342.

**What would invert the call:** if the partner agencies report the older woman's leads close better,
the cost premium becomes a discount and the lead call flips. That is gate two, and it is exactly the
measurement the brand cannot currently see.

## Escalation, verified by the orchestrator's own pull — 2026-09-04

The flat savings claim was reported in Phase 1 as "69% of lifetime static spend." That understated it
badly. A live keyword sweep in the messaging pass, **independently re-run and confirmed by the
orchestrator**, returns:

**`saving you 20% or more` — 127 ad-name groups, $100,066.79 of $100,067.42 in the trailing 90 days.
Essentially 100% of spend, video included.**

The claim sits in the shared body-copy block that appears on every ad in the account. The brand's own
guidelines mark "always 'up to 30%' — never drop the 'up to'" as non-negotiable, and two ads carrying
the related "24% cheaper" headline are already Meta-DISAPPROVED.

The second unsupported claim rides the same block: **`Approved by thousands of Mom's across America`
is the `ad_title` on all eight of the eight top-spending ad names — $83,918.11, 83.9% of the 90-day
window** — against zero reviews, zero press and no BBB profile for the operating entity.
`category-and-market-research.md` documents six verified enforcement actions aimed at exactly this
industry layer, including FTC warning letters to 21 health-plan marketers and lead generators.

**Why this is the cheapest fix on the list:** both claims live in one shared copy block. Editing that
block once changes essentially every ad in the account. No creative needs remaking.

## Phase 2 — the messaging call

`strategy/messaging-strategy-input.md`. **Position: stop leading with savings, lead with standing.**
She has more say over her own coverage than she believes, and the sharpest version is that she is
allowed to leave the plan she thinks she is stuck in. Three parts, all changing:

- **Territory — standing, not savings.** Every dollar of live spend leads with a number she can beat,
  and 82 of 1,322 comments beat it, 64 naming a higher figure. Underneath sits the luck belief: the
  four highest-engagement metaphor rows treat another woman's coverage as a lottery win. Savings copy
  assumes she can choose; she does not think she can.
- **Register — calm permission.** The account already learned this. Calm openers delivered
  $13.29-$24.45 per lead; distress openers $29.85-$38.09, blending to $33.23 — while the distress ads
  posted the *higher* hook rates. **Intensity buys the stop, calm buys the lead.**
- **Proof — one real named licensed human** using the audience's vocabulary correctly.

**What it costs, stated in the document:** it gives up a phrase with a 45.76% hook rate and no decay;
its best supporting ad is compromised (two of five variants Meta-DISAPPROVED, headline breaks the
brand's own hard rule); it points at a woman the underwriting may reject; the income-gap version is
compliance-blocked because Medicaid and the Marketplace cannot be named; and every figure clears gate
one only.

**Maternity is explicitly ruled OUT as a messaging lane** and routed to product and claims instead:
no hook fixes a name that promises around an exclusion.

## Phase 2 — the casting call, and two more corrections

`strategy/creator-talent-strategy-input.md`. **Position: lead with the woman who reads 45-55, and
put her in the first three seconds instead of the fourteenth.** She is not a hire — she already
delivers the pitch in both of the account's two biggest ads ever, and has never once opened one.

**The spine is a comparison nothing in the vault had made:**

| Ad | Spend | Leads | CPL | Hold | She arrives |
|---|---|---|---|---|---|
| `Moms43 - 4 - V3` | $57,506.21 | 2,668 | $21.55 | **3.81%** | 0:18 |
| `MOMS38 - 1 - V1` | $54,173.20 | 2,689 | $20.15 | **17.12%** | 0:14 |

Near-identical size, near-identical lead count. **Four seconds of difference buys four and a half
times the watch time.** Second half of the call: put a second person in frame, proven four ways in
this account, every one clearing or nearing the 12% hold floor.

**Correction — the phone call is not an expensive format.** `MOMS38 - 2 - V4` and `V1` land at
**$22.87 and $22.50**, at or below the window CPL, on **27.31% and 25.36% hold**. The $30.91 figure
carried through three documents is the third-best build, not the format.

**Correction — the "$287 of non-white creator spend" is imprecise.** The two ads Parker reads as
Black or Asian-American led carry **$252.91** combined. Separately, the account's best click
economics — **$16.43 CPL, 3.15% CTR, $0.95 CPC** — belong to `moms-53 3`, fronted by a creator read
as mixed race or Hispanic, on $1,955.60.

**A live find no vault document held:** `MOMS25 BLAST - X1 - Copy 2`, two women talking to each other
in a podcast studio, **$3,483.03 for 175 leads at $19.90 CPL and 10.29% hold**. `visual-vocabulary.md`
concluded the brand's podcast format is "a podcast setting without a podcast, only ever one person in
it" — true of the two ads it read, false of the account.

**The lab coat rules itself out on its own evidence:** $7,407.34 at a $19.44 CPL but **2.44% hold**,
and it delivered **52.7% of spend to women 25-34**. The clinical setting skews young, the opposite of
what authority is supposed to do here. Authority survives only as the gated runner-up, via a licensed
partner advisor.

**What the call costs, named in the document:** the CPL edge is only $1.40 (6.5%) and the real case
rests on hold rate, which this account has not shown predicts lead cost; the woman recommended is the
one a viewer called "Creepy AI blonde lady" on a live flagship, so the casting change must ship
alongside a production-method change; and gate two is invisible, so if she brings leads the partner
agencies cannot enrol, the call is wrong in a way Parker cannot detect.

## Phase 2 convergence — worth stating before the roadmap

Four inputs, four independent evidence paths, one direction. **Persona** says lead against the woman
who pays and still owes, changing the premise not the audience. **Product** says lead with the switch
as a static on `www./save/`. **Messaging** says lead with standing rather than savings — *you are
allowed to leave*. **Casting** says the woman who already carries both flagship ads should open them.

None of these was told what the others concluded. They agree.

---

## Phase 3 — Ideation, 2026-09-04

### `ideas-and-briefs/brand-idea-bank` → `idea-bank/` — **fail, repair pass running**

**Run.** Backfill mode on the built brain. 20 entries in `idea-bank/entries/`, plus `README.md` and `index.md`. Roughly 23,400 words. Nine marked `worth testing`, eleven `raw idea`.

**Source-surface spread.** Customer language (commenters under the brand's own paid ads) 8 · organic video from the 23-video mining library 7 · the team's own conversations with Parker 2 · Parker's cold pass 2 · old print ads 1 (data-limited) · competitor paid ads 0. Hunt lanes: customer language 8, format 7, cold pass 2, far transfer 1, historian 1, affinity paid 1.

**Five live Parker pulls rather than carrying the vault forward:** `search_chat_history` (17 threads, 3 read in full), `search_facebook_ad_comments_sql` top-30 by likes plus two keyword sweeps, and `search_tiktok_videos` twice across all 23 rows. Two things surfaced that the vault did not have: a 10-like paycheck-stub comment that pairs with an organic video nobody had connected to it, and real viewable URLs for every organic entry.

**Four lanes recorded as gaps rather than papered over.**

1. **The historian lane is nearly empty, and it is a tooling gap, not a judgment one.** `parker-system/creative-strategy-context/old-ads/entries/` holds zero files, and all three live-archive fallbacks the corpus README names — `repository.duke.edu`, `www.ebay.de`, `adretro.com` — are blocked by the network egress proxy. One entry was logged from a 1954 Blue Shield headline recovered from an archive listing title, marked `data-limited` with no visual reconstruction, plus two retrieval leads. Biggest hole in the bank.
2. **No trend lane.** The mining library is a fixed scrape from 2026-09-03 and no fresh TikTok keyword search runs from this environment, so there is no "what moved this week" capture.
3. **No competitor lane.** Nothing tracked. Ethos sells term life, so it is logged as an affinity reference and never as a category read.
4. **Far transfer ran one client-supplied lane** rather than the method's two or three rotated categories, and the entry says so.

**Fidelity review verdict: FAIL** — narrowly, on one named hard rule plus two labeling gaps. Reviewed by an independent agent against the prompt, not by the agent that wrote it.

What the review verified as correct, by check rather than by assumption: all 18 schema fields present in all 20 entries with none thinned; the prompt's literal fallback string for missing media present verbatim in the 5 entries lacking it; the evidence picture in all 20; the index table carrying exactly the six columns the prompt names; `generated_on` / `refresh_by` stamped, with the `refresh_by: none` claim confirmed correct against `parker-system/system/refresh-cadence.md:65`; the craft-doc sign-off block stamping exactly the five docs that carry required sign-off lines, naming the ones read that carry none, and explaining why `creator-briefs.md` was read but deliberately not stamped; the open-loops tail in canonical four-part form even though this prompt embeds no open-loops block; zero "customers said"; zero ROAS/AOV/purchase-value reads; and zero reproductions of either banned claim string, with four entries actively flagging the flat savings claim for stripping. Six numbers spot-checked against the vault matched to the digit.

The three gaps:

1. **Hard-rule breach — the fail.** `entries/2026-09-04-the-flat-confession.md:62` calls an ad "this account's biggest winner" with no basis stated and gate two unnamed. That breaks `brand-lens.md:72` and `CLAUDE.md:47`, and it contradicts the bank's own claims at `README.md:48` and `index.md:36` that nothing in it is called a winner. The phrase was inherited from `audits/2026-Q3/gaps-opportunities-inspo.md:275`, but that doc carries the gate framing at line 283 and the entry does not.
2. **Step seven half-honored.** The prompt calls stage of awareness and audience fit inferences and requires the uncertainty be marked. Nine entries do it. Eleven carry no claim label on `persona_or_audience_fit` and no uncertainty note; on `you-did-everything-right` both fields are unlabeled.
3. **Three comment counts without denominators.** `CLAUDE.md:126` requires them, and the bank declares the 1,342 / 1,322 corpus split at `index.md:10` and honors it in 17 other places — but not in three claims about the 42 pregnancy and 55 pre-existing-condition objection comments.

**Disposition:** the method's single automatic re-run, scoped to the three named gaps, with everything the review verified as correct explicitly preserved.

**Repair outcome.** 13 entry files changed; `index.md` and `README.md` untouched. The repair closed all three gaps **and found three more of the same kind that the review had missed**, which is the useful part of the record:

- The winner breach appeared **twice more wearing the word "best"** — `a-hill-i-will-die-on.md:47` and `the-second-task-that-frees-the-eye.md:59` both called the same ad "the account's best paid ad," which is the identical claim with a shorter word. The review had searched for the word it already found. All three now name the ad by what it is — the highest-spending one, `Moms43 - 4 - V3` at $42,741.16 across the 90 days to 2026-09-02, 43.5% of everything spent — and state that biggest by spend is not best, that it buys leads at $22.21 inside the brand's own "meh" band so it clears gate one and no better, and that gate two sits with the partner agencies.
- A **fourth missing denominator** in `the-pinned-comment-answered-out-loud.md:57`, the identical breach in an entry nobody had checked.
- Eleven persona fits labelled, plus the twelfth field flagged. Not blanket-labelled: seven got split labels because the persona is reasoned while what she wants is not evidenced at all, and the thin-base ones read `data-limited` rather than `inferred`.

**Re-review verdict: PASS.** All three gaps closed, nothing that previously passed regressed, both fold-ins landed. The reviewer swept independently for every word the superlative could wear — winner, best, top performer, star, hero, champion, workhorse, breakout, control, strongest, number one — and confirmed every remaining hit legitimate: commenters' own verbatim, a craft rule being quoted, an organic TikTok rather than an ad in this account, or a metric-scoped fact the same sentence qualifies. It also confirmed the 1,322 denominator reasoning holds and that the bank is consistent in both directions — live-pulled counts on 1,342, doc-carried counts on 1,322, each saying which.

Two residuals it flagged as pre-existing rather than regressions were closed rather than left: three persona fits whose `verified` mark attached to a supporting fact left the fit read looking settled, and two roadmap citations missing the drafted-and-unapproved label.

### `ideas-and-briefs/idea-evaluation` → `idea-bank/evaluation-2026-09-04.md` — **done**

615 lines. All 20 ideas placed and banded, nothing sampled. Priority draw: **P1 = 2, P2 = 9, P3 = 6, serving no priority = 3**. **Zero hard cuts**, six soft pulls each named with the road it grazes, four folds so the next round does not brief the same thing twice. The ranked call is marked **provisional** throughout, against a roadmap that is drafted and unapproved.

**The finding that changed the roadmap.** The evaluation's live pulls showed the two statics behind Priority 2 are **fabricated social proof**. The orchestrator re-pulled it independently rather than let it travel on one agent's read, and it verified wider than reported: **seven static ad-name groups, $35,234.91 lifetime, 2,871 leads at $12.27**, all mock X posts with a blue verified checkmark on an invented persona (`@cindie_mama_23`, `@thehealthymom34`, `@Motherooffthree`) and printed engagement counts. Against the brand's own non-negotiable **"No fabricated statistics."** `B1 - Copy 7` is one of the two statics Priority 2 wanted to restart, so **Priority 2 is a rebuild, not a switch-flip**, and the $11.79 must never be carried as a forecast. Two carry a second breach each: `B1 - Copy 7` runs the flat "24% cheaper", and `B2 - 10TH JUNE - Copy 1` runs "no government red tape" against the brand's no-government-references rule — a third distinct live breach nothing in the vault had recorded.

**Delivery question resolved the same day.** All seven read `effective_status: CAMPAIGN_PAUSED` and returned zero spend across the last 30 days; across 365 days the set spent $699.78 for 32 leads. So this is an asset-library and compliance problem, not live burn. Full record: `running-notes/missing-context.md`, `brand-lens.md`.

### `ideas-and-briefs/sprint-plan` → `sprints/2026-09-04-lead-with-the-switch/sprint-plan.md` — **done**

540 lines. **8 concepts, 20 assets, two waves.** Sized from live pulls: trailing 30 days $48,381.47 / 2,171 leads / $22.29 CPL, and a real net-new evergreen cadence of ~1.4 concepts a week once duplicates and variants-of-one-concept are stripped from the raw 95 groups since 2026-08-01. Split P1 = 2, P2 = 4, P3 = 2 — deliberately not mirroring the bank's shape. Personas: `pays-and-still-owes` 5, `already-knows` 3, `built-it-herself` 0 and dropped on purpose with the reasoning written out. Three of eight concepts need nobody on camera, which walks around the brand's stated number-one bottleneck.

**Two findings, both re-verified independently by the orchestrator before briefs were built on them:**

1. **Zero statics created since 2026-06-01.** A static-filtered lifetime pull with `created_time >= 2026-06-01` returns **zero rows** — three months, not one static — in an account where statics convert link clicks to leads at 16.57% against video's 8.28%.
2. **Only 14 of 95 ad-name groups created since 2026-08-01 took $500 or more**, and those 14 carry **$24,804.82** of the cohort's $25,908.79 — **95.7%**. Eighty-one never got read. That is why the round launches in two waves rather than being dumped.

### The quiz destination, upgraded by the same pull — the account ran the experiment itself

Inside those 14 funded groups sit **matched pairs on the identical video file** — same storage hash, same text hook, same body copy — split only by landing URL. `verified live`, 2026-09-04:

| Group | Destination | Leads | Cost per lead | Landing page views / link clicks |
|---|---|---|---|---|
| `moms-63 2b` | `www./save/` | 417 | $13.26 | 2,981 / 3,404 = 88% |
| `moms-63 2b - Copy` | quiz | 6 | $144.23 | 54 / 672 = 8% |
| `moms-63 3e` | `www./save/` | 339 | $15.46 | 3,014 / 3,531 = 85% |
| `moms-63 3e - Copy` | quiz | 8 | $67.15 | 30 / 344 = 9% |

Creative held constant by the file hash, only the destination moving. It still does not separate "nobody arrives" from "arrivals are not measured," but it settles that the quiz costs real money at scale and sizes it. All four quiz-pointed groups read `ADSET_PAUSED` today.

### `ideas-and-briefs/brief-creation` → `sprints/2026-09-04-lead-with-the-switch/briefs/` — **done**

**Eight briefs, J001 through J008, ~52,000 words.** All 11 required sections present in all eight, plus the three validations, the execution routing table, the open-loops tail, the Parker media appendix, and sign-off stamps for every doc that carries one and was read.

**No brief carries customer-facing copy**, which is what the prompt itself demands. Each names per variation which execution skill produces the copy and which docs it must load, and states that every line ships with both gate receipts before anything is designed or filmed. Existing ad copy appears only as evidence of what already ran; J003 explicitly forbids pasting those strings.

Three briefs build on `B2 - 10TH JUNE - Copy 16` as the clean frame. The orchestrator re-pulled it: the carried figure was **stale** ($15,660.83 / 1,040 leads / $15.06) and the ad is still `ACTIVE`, now **$18,409.73 / 1,181 leads / $15.59**. Re-pinned in all three. It also verified **clean on inspection** — solid black, white serif hook, white sans body, one emoji, no profile, no handle, no verification badge, no printed engagement counts, and "Save up to 30%" with the qualifier intact. And it delivers **31.6% of spend to women 45 and over against the account's lifetime 21.2%**, plus 69.1% Instagram — independent support for the older-spokesperson thread in J002 and J006, recorded as an observation rather than proof, since Meta's optimiser chose that audience.

Three briefs carry honest blockers rather than pretending: **J007 is hard-gated** pending a written answer on the licensed-advisor question, **J008** has an unresolved compliance question about what any comparison figure is measured against, and **J006** flags that both its source ads sit inside the 127-group set carrying the banned copy block, so a re-cut would silently republish it.

Two things the brief pass could not execute, both recorded rather than worked around: `creative-consumption-analysis.md` is named as the casting method for J002 and J006 but cannot run, because the mining library is a frozen 23-video scrape and no live keyword search runs from this environment; and no fresh Parker pulls were made in that pass, so every figure is carried with its original mark and denominator, which each brief states in its appendix rather than implying fresh calls.

### Conflict resolved by live pull — cost per link click on `moms-53 3`, 2026-09-04

The bank flagged three docs giving three different costs per link click for one ad: $0.69 (`sub-context-docs/brand-profile-narrative.md`), $0.96 (`strategy/strategic-roadmap.md`, twice), $0.67 (`audits/2026-09/monthly-hook-audit.md`).

**Not a data error. Two metrics wearing one label.** `verified live`, `search_facebook_ads_sql`, ad `120247254787160519`, window 2026-06-06 to 2026-09-03, Meta default attribution. Over that window the ad spent **$2,041.42** and bought **2,962 clicks but only 2,127 link clicks**. Cost per click across all clicks is **$0.69**, matching the narrative exactly; cost per *link* click is **$0.9598**, matching the roadmap exactly in both places; lifetime cost per click today is **$0.68**, which is almost certainly what the hook audit read as $0.67 pulling one day earlier.

All three docs were right and none was talking about the same thing. No correction is needed — each should state which metric it means. **Standing rule: use cost per link click when the question is what it costs to get someone to the site, because 28% of this ad's clicks are engagement the brand cannot convert.**

### New operational break found by the same pull — the quiz destination, 2026-09-04

`moms-53 3 - Copy` (three variants, $497.42 across the window, `ADSET_PAUSED` today) carries the **same creative, same hook and same body copy** as `moms-53 3`, but points at `quiz.healthformoms.com/#/indvfam` instead of `www.healthformoms.co/save/`. It returned **9 landing page views against 511 link clicks** — click quality **1.76%** against the sibling's **76.12%**. `verified live`, 2026-09-04.

**Two possible causes and the data cannot separate them:** either almost nobody who clicks lands, or they land and the pixel does not fire on that domain. The first is lost spend; the second means every quiz-pointed ad in this account has unreadable conversion numbers. Both are urgent, neither is a creative problem.

Routed to the team in `running-notes/missing-context.md` as a fix rather than filed as a research loop, the same call the roll-up made on the `go.healthformoms.co` break. **Two destination breaks found independently now, which makes a single audit of every landing URL in the account the right response rather than two one-off patches.** No brief may be built on a figure sourced from a quiz-pointed ad until this is settled.

---

## Build-completion verification — 2026-09-04

Run by an independent subagent against the runner's "Verify the build" checklist. Structural completeness only, not document quality. **First verdict: FAIL — 2 blocking gaps, 2 secondary, 7 of 9 items passing.** All four fixed in the same pass; none was a rebuild.

### What passed, by check rather than by assumption

- **The method is mounted and pinned.** Submodule clean at `b55c441`, carrying `prompts/`, `creative-strategy-context/`, `system/`. The v14-versus-v15 question was re-confirmed independently: `git tag --points-at HEAD` returns **both**, so `git submodule status` printing `(v14)` while the config says `v15` is two tags on one commit, not drift. Deny rules present in all four path forms.
- **Skills cross-checked by name and count.** All **21** factory skills present, plus the 5 routine-bundle additions = **26**, every one carrying a real `SKILL.md`, no empty directories, **exactly one `dream`**.
- **Both review-gate checkers execute in the brain.** `voice-lint.py` flagged a throwaway line and exited 1; `grounding-check.py` printed usage and exited 2.
- **The brain is self-running, and verified against the account rather than the docs.** `list_triggers` returned all six routines registered and enabled, with cadences and next-run times matching every schedule doc exactly. The MCP-connector limitation is real — every trigger returns `"mcp_connections":[]` — and it is documented in `schedules/README.md`, on all six status lines individually, and in the status file, with each doc naming whether that routine actually needs it.
- **The freshness ledger is real.** All 56 standing docs aggregated; eight spot-checked against actual frontmatter and all eight matched to the day. The one doc with no `refresh_by` is flagged by the schedule itself in bold rather than hidden.
- **Provenance holds under adversarial check.** The banned savings string returns 26 hits outside the method mount and **every one is the string being quoted as prohibited** in a compliance checklist — zero reproductions in copy. ROAS appears in 8 audit files and **every instance is a refusal**. The idea-bank hard-rule breach is gone.

### The four gaps, and what was done

1. **BLOCKING — a dangling path in the operating contract, five times.** `CLAUDE.md` lines 60, 83, 89, 108 and 179 pointed at a root-level `brand-profile.md` that does not exist; line 60 is the "**Read it first on every question**" instruction and line 89 makes it the retrieval floor for every creative answer. Carried through verbatim from `parker-system/templates/brand-brain-CLAUDE-template.md` lines 19, 42 and 48. The real doc is `sub-context-docs/brand-profile-narrative.md`, which `CLAUDE.md:222` already named correctly. **Fixed: all five repointed.** This is the highest-cost gap on the list — the contract was instructing every session to open a file that could not resolve, on every question.
2. **BLOCKING — the status file.** `BUILD-STATUS.md` still reported Phase 3 as running at 0 of 4 against a Phase 3 that was finished and committed, and it had not been moved out of the repo root. **Fixed: reconciled and archived here.**
3. **Secondary — the run log stopped mid-Phase-3.** It recorded the idea bank as "fail, repair pass running" and never recorded the repair outcome, the re-review, or the three prompts after it. **Fixed: the whole Phase 3 record is written above.**
4. **Secondary — `expert-insights/` did not exist** while `CLAUDE.md` described it as present with three subfolders. **Fixed: scaffolded with its `inbox/`, `curation/`, `context-update-candidates/` and a README saying plainly it is empty by design and fills on the first `/expert-signal-intake` run.**

### Also recorded, none of them gaps

- **This repo has no `main` branch.** All work sits on `claude/parker-brain-health-for-moms-x0vbs5`, tracked by [PR #1](https://github.com/insuranceyeti/creativeyeti/pull/1). Documented in `running-notes/standard-sync.md`, including that the session-start hook's `fatal: couldn't find remote ref main` is benign and that merging the pull request is the team's call, not Parker's. Until then `/save-brain`'s "everything lands on `main`" rule cannot be followed literally, and a teammate cloning the repo lands on a default branch that may not exist.
- **`users/` does not exist**, so the brain has no stored read on the person using it yet. Expected on a fresh brain; it fills as they work.
- The save is healthy: working tree clean, nothing ahead of upstream, nothing unsaved.

**Verdict after fixes: pass.** Logged per the runner's requirement that every verdict lands here.
