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
