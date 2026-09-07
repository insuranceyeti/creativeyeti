# Landing page H1 tests — Health For Moms — www.healthformoms.co/save/

**Deliverable:** landing page hero H1 candidates, 5, each a test against the current control.
**The control is a named blank.** `www.healthformoms.co/save/` is blocked by this environment's network policy (EGRESS_BLOCKED, re-tried 2026-09-07; same block recorded 2026-09-03 in `website-and-product-audit.md`). I cannot see the current H1, subhead, button text, or the on-page contact language. Every test below is a challenger against an unseen control. Mike should paste the current H1 so the set can be re-read against it.
**Where to run them.** On `www.` only. The `go.healthformoms.co/save/` destination turned 690 link clicks into 63 landing page views (9.1%) at $273.23 per lead on the same creative that converted at 80.3% and $19.25 on `www.` (`verified`, 2026-09-04 pull recorded in `website-and-product-audit.md`). A headline test on a page that loses 91% of arrivals before the hero renders measures nothing.
**What to read.** Leads per link click, not landing page views and not cost per lead alone. `product-priority.md` line 89: landing page views are an unreliable counter on this account (the `go.` collapse was a proven counting artifact), and leads divided by link clicks is the ratio that survived. If the page-builder's own split tool counts its own views, say so and read leads per its view; if the read is in Meta, use leads per link click by ad, with the challenger and control on separate URLs. Cost per lead is gate one; lead quality lives with the partner agencies and Parker cannot see it. No H1 here gets called a winner on cost per lead.

---

## Brand type, stage, sophistication

Problem/solution. She arrives problem-aware to solution-aware: she clicked a video whose hook was either the flagship `POV: Telling your husband you found better health insurance, saved $400 a month, AND the deductible is zero. Wife of the year energy. 💕` ($43,459.55 of $103,938.70 in the last 90 days, 1,922 leads at $22.61, pulled 2026-09-07) or the deductible-mirror family (`My deductible is $6000. I have to pay $6000 before my insurance even kicks in...`, `MOMS39 - 2 - V2 - Copy`, $18.38 per lead, same pull). High sophistication: she already has insurance ("deductible" in 207 of 1,342 comments, "uninsured" in 2, per `strategic-roadmap.md`), she has tried her employer plan, and her first question on arrival is a trust check, not a benefit check: "Is this legit?" (2026-04-27, `Moms43 - 4 - V1`), "Is this real?" (2026-05-15, `Moms43 - 4 - V4`), "How does it work" (2026-08-11, `Moms43 - 5 - V1`), all re-pulled live 2026-09-07 via `search_facebook_ad_comments_sql` (substring "legit": 4 rows; "is this real": 1 row; "how does": 1 row; the three quotes are rows `7acf4fad`, `667ae414`, `cd63dfcf`). An earlier semantic pull surfaced the same three, but it did not show in the pull log, so the SQL pull is the receipt.

The page's job, per `customer-journey-and-persona-discovery.md`: "The click takes almost no thought and the purchase behind it takes a great deal... What the creative has to do is win a two-second qualification scan and then survive a trust check." The H1 is the two-second qualification scan. The subhead and button carry the rails.

**Held constant across every test.** Subhead, drafted from the rail phrases (not verbatim): "Depending on your state, you may qualify for a private family plan with a $0 deductible option. Some moms save up to 30%. Takes about 30 seconds." Button: "See if you qualify". The rails it is built from are verbatim from the winners' transcripts (`moms-63 3e` 0:28 "you may qualify for a health plan with a $0 deductible", `moms-53 3` "It takes you 30 seconds... fill it out and see if you qualify", closing VO "save up to 30%"; `brand-identity-analysis.md`). **The hero image is not held constant.** `static-ad-design.md` is explicit that message and image move together, and that one image under five different messages is the common failure. Each test below names the in-play shot from `visual-vocabulary.md` it should sit over. The current hero is unseen, so the pairing is a recommendation until Mike pastes what's there.

---

## Baseline studied

**Running corpus, pulled 2026-09-07.** Last 90 days, top 15 spenders by name: 15 of 15 carry the identical `ad_title` "Approved by thousands of Mom's across America" and the identical body copy block with "saving you 20% or more". The headline surface the account actually varies is the `text_hook`, the on-video overlay. Its families:

- **POV wife-of-the-year** — `POV: Telling your husband you found better health insurance, saved $400 a month, AND the deductible is zero. Wife of the year energy. 💕` on `Moms43 - 4 - V3` ($43,459.55, $22.61), `moms-63 3e` ($7,433.62, $16.97), `moms-63 2b` ($5,673.86, $13.20), `moms-65 1a`, `Moms43 - 4 - V1`, `Moms43 - 4 - V4`. Carries the spend.
- **Deductible mirror** — `My deductible is $6000. I have to pay $6000 before my insurance even kicks in...` (`MOMS39 - 2 - V2 - Copy`, $18.38), `if you're a mom and your deductible is insane listen to this` (`Moms Nahuel WV#1 - V9 - Copy`), `STOP paying your insurance deductibles before you watch this.,, Seriously.` (`Moms43 - 5 - V4`).
- **State gate** — `Approved State List ✔️` (`moms-53 3`, $2,665.55, 156 leads at $17.09, 3.05% CTR, the highest CTR of the top 15).
- **Calm POV** — `POV: At peace...because my family finally has the best health insurance and I pay less. ❤️` (`MOMS34 - N1 - 3a`, $25.24).
- **Hack / reveal** — `Sharing this 2026 health insurance hack!!` (`Moms43 - 5 - V1`, $10,578.68, $24.10), `Here's why Moms are cancelling their health plans 👇` (`moms55-1`, $23.53).

**Lifetime statics by leads, pulled 2026-09-07, all 12 rows** (the `headline` field is populated here and it is the closest thing the account has to a tested H1):

- `B1 samar- Copy` — 39 variants, $54,224.86, 4,441 leads at $12.21. The group's `headline` field is empty on the parent row; its variants carry "Didn't know I could ditch my job's health plan… until I did. Now I have no deductibles and choose any doctors we want 👏" (`visual-vocabulary.md` shot 14), "Left my work health plan for one that's actually built for moms." (P005), and "I changed our health plan, got $0 deductible options, and picked our doctors with no networks." (`brand-identity-analysis.md` line 616). The largest static family in the account and the employer-switch family. **Headline field only as a reference; the body copy carries "saving you 20% or more."**
- `IMG 6` — "Moms, your health insurance should cover preventative care..." — 1,331 leads at $6.98 (2024-12-10)
- `5TH APR - Copy 8` — "I PAID $1,000 OUT-OF-PICKET FOR A 5-MINUTE ULTRASOUND." — 338 leads at $6.99
- `5TH APR - Copy 29` — "One ER visit could've wiped us out." — 747 leads at $9.62
- `B1 - Copy 7` — "Left my big insurance company for a mom-focused one. 24% cheaper and I choose my own doctor 😌" — 2,584 leads at $11.74. **Off limits as a reference: flat "24% cheaper" breaks the up-to rule and 2 of 5 variants are DISAPPROVED.**
- `B1 samar- Copy 1` — "Didn't know I could ditch my job's health plan… until I did." — 1,231 leads at $11.89
- `B2 - 10TH JUNE - Copy 16` — "Moms...." — 1,181 leads at $15.59
- `B2 - 10TH JUNE - Copy 1` — "If you're self-employed, between jobs, or just tired of paying too much..." — 112 leads at $16.77
- `OMC-Health for Moms-[B1-C3-V3] - Copy` — "I'm a single mom, and I didn't know my insurance was failing us... 😭" — 70 leads at $16.11
- `14TH JUNE - Copy9` — "MOM approved" — 129 leads at $17.28
- `B1 - Copy` — "Do your family's health a favor" — 119 leads at $15.79, DISAPPROVED
- `15` — "Mom hack: Left my big insurance company for a Mom-focused company that understands my values." — 116 leads at $18.32

**Fingerprint.** 6 to 14 words. Sentence case with one all-caps outlier. First person or a "Moms," callout. A specific odd number where there is one ($1,000, 5-minute, $6000). Ellipses and one emoji are normal. The register is a mom telling another mom what happened to her, never the brand describing itself. The one brand-voice title ("Protect Their Health, Protect Yours") is the `ad_title` on every static and is never what varied.

**AI-tells to avoid, by contrast with this corpus:** no colon-summary, no "Discover / Unlock", no balanced triad, no "say goodbye to", no marketing abstraction ("coverage that works for you") where the corpus names the thing (the deductible, the ER, the ultrasound, your job's plan). No "not just X, it's Y". The corpus asks one real question at most and never interviews itself.

**Rivals:** none. Competitor tracking deferred at the team's request 2026-09-03; no rival headlines exist in the vault to counter.

---

## The five tests

### Test 1 — Winning-headline adaptation — the employer-plan mom, relief that she has a choice

> **You don't have to keep your job's health plan.**

- **Process:** headline-from-winning-headline. Adapts the `B1 samar- Copy` employer-switch family: the group at 4,441 leads and $12.21 across 39 variants, and its single-variant sibling `B1 samar- Copy 1` at 1,231 leads, $11.89, 15.03% leads per link click (both pulled 2026-09-07). Headlines adapted: "Didn't know I could ditch my job's health plan… until I did." and "Left my work health plan for one that's actually built for moms." Mechanism borrowed: the standing reveal, that leaving the employer plan is allowed. Content swapped from first-person past tense to second-person present, because the H1 speaks to her, not as her. 9 words.
- **Hero it sits over:** the walk out of the house (`visual-vocabulary.md` shot 2, in play, verified; the `moms-63 2b` and `3e` frame, the two cheapest funded leads in the window). She is leaving. Alternative: the dark-mode fake tweet (shot 14) as the proof element under the H1, since it is the exact line's own container.
- **ICP and emotion:** the mom on an employer plan with a deductible she never chose. Relief, then permission. Level 2 (what she can't do: leave the plan she was handed) reaching toward Level 3 (she has no choice, as a state of being).
- **Source:** the headline above, plus the commenter on 2026-05-05 under `MOMS38 - 1 - V2`: *"And if it's an employer insurance, you don't have to sign up with that employer insurance you can decline the coverage and go out and find your own insurance carrier."* And *"Mine is $6k per person too but since it's thru my job I don't really have a choice"* (`MOMS39 - 2 - V2`, 2026-03-17, `voc-pain-phrase.md`). Executes idea-bank entry `2026-09-04-you-can-decline-your-jobs-plan.md` and the roadmap's Priority 2 ("lead with the switch, not the saving"), which is drafted and unapproved.
- **Why:** this is the message the roadmap says the whole account should lead with, and it has never been on the page. The employer family is the most durable signal in the comment corpus (24 comments, March through August, per `strategic-roadmap.md`).

### Test 2 — Rail phrase as H1 — the mom who clicked the $0 deductible hook, message match

> **Moms, you may qualify for a $0 deductible option.**

- **Process:** headline-from-winning-headline, adapting the winners' own closing line rather than an overlay. `moms-63 3e` at 0:28: "you may qualify for a health plan with a $0 deductible"; `moms-53 3`: "fill it out and see if you qualify"; Mechanism: message match. 9 words; "you may qualify for a health plan with a $0 deductible" is verbatim `moms-63 3e` at 0:28, and the "Moms," callout is `IMG 6` ($6.98). The voice gate moved the imperative off the H1 so "see if you qualify" lives once, on the button. She clicked on "the deductible is zero"; the first thing she reads says the same thing in the hedged form.
- **ICP and emotion:** the flagship's clicker, `pays-and-still-owes`. Hope, held in check by "see if you qualify". Level 1 surface, and that is a stated exception to the checklist's Level 2 rule: on a landing page the ad has already done the Level 2 work, and this arm tests whether confirmation alone converts.
- **Hero it sits over:** the silent bed (`visual-vocabulary.md` shot 1, in play, verified), the flagship's own frame, so the page looks like the ad she clicked.
- **Source:** the transcripts above, `brand-identity-analysis.md` "Where the live winners do hold the rule". Compliance: "$0 deductible option" and "see if you qualify" are the brand's exact sanctioned forms.
- **Why:** this is the likeliest current control, or close to it, and it is the safe arm. If it beats the others, the page's job is confirmation and the ad does the selling. **Flag:** if the current H1 already reads like this, drop this test and keep the control.

### Test 3 — The brand's own unfunded line — the skeptic at the trust check

> **Yes, it's real insurance. Not a health share.**

- **Process:** headline-from-comment-response. Answers the arrival doubt in her words. Comments, `search_facebook_ad_comments_sql` 2026-09-07: "Is this legit?" (2026-04-27, `Moms43 - 4 - V1`), "Is this real?" (2026-05-15, `Moms43 - 4 - V4`), "A Google search doesn't pull anything about this. Is it legit?" (2025-07-24, `B1 samar- Copy`, 1 like), "How does it work" (2026-08-11, `Moms43 - 5 - V1`). The vault carries the first and third at `customer-journey-and-persona-discovery.md` line 404 and `website-and-product-audit.md` line 237. And from the vault: *"Is this insurance or something like a Christian health share?"* (2026-08-31, `2026-09-04-yes-its-real-insurance.md`).
- **ICP and emotion:** the skeptic who has been burned by a form before. Relief from a specific doubt. Level 3: she does not want to be the fool who got scammed.
- **Source:** the line is the brand's own, from `MOMS25 - 5TH DEC - Y1 - Copy 3` (created 2025-12-05, $77.86, 4 leads at $19.47): *"And before you ask, yes it's real insurance. Not a health share, not some discount card."* Trimmed: "discount" is a banned word, so the third clause goes. "Real insurance" is the brand's own description of the private plans, `stated`; the plans are medically underwritten private health plans per the brand context Section 1.
- **Why:** the customer-journey doc says the page has to "survive a trust check she runs somewhere the brand does not control." This puts the trust answer where the brand does control it. 8 words.
- **Hero it sits over:** the wall of state names (`visual-vocabulary.md` shot 4, in play, verified), which the state-list idea-bank entry calls "the only genuine document in its whole library." A real document under a line about being real. Not the fake tweet: a mocked-up post under "yes, it's real" undercuts itself. **Compliance note:** naming a health share as what this is not is allowed (no named company, no government reference). Do not extend it to "no calls" or "no random agents"; two commenters say the page already made that promise and it was broken (2025-11-28, `B1 samar- Copy`).

### Test 4 — Problem-naming question — the mom who pays and still owes, in her arithmetic

> **Got insurance but still a bill at the doctor?**

- **Process:** question-engagement. One question, forces an internal yes.
- **ICP and emotion:** `pays-and-still-owes`. Resentment, Level 2 (what she can't do: use the thing she pays for).
- **Source:** *"I still pay full price for everything all year until I pay $6k which has been never. They have never helped me pay for anything, but I give them thousands a year for what?"* (`voc-pain-phrase.md`) and *"Why we have insurance and still have a damn bill when we go to the doctor."* (same slice). Voiced from those two, not lifted; both are longer than 10 words. 9 words.
- **Hero it sits over:** the school pickup line (`visual-vocabulary.md` shot 8, in play, verified; `moms55-1`, "doing the math on how much I pay for health insurance"), a mom in the car doing the arithmetic. Not the crying close-up: the account's calm openers convert at $13.20 to $17.09 and its high-distress ones at $29.85 and up (top-15 pull, 2026-09-07).
- **Why:** this is the experience, not the number. `2026-09-04-mirror-the-experience-not-the-number.md` shows that mirroring a dollar figure produces a bidding war (64 of 76 "mine is" comments name a higher number than the ad's) while mirroring an experience produces recognition. A landing page has no comment box to bid in, but the disqualify reflex is the same: a number she beats reads as unrealistic. So no number in this H1.

### Test 5 — The state gate — the cold clicker, the open loop she has to close

> **Is your state on the approved list?**

- **Process:** question-engagement, one question, adapting the state-gate mechanic. 7 words; the "check in 30 seconds" clause moved to the subhead, which already carries it. `moms-53 3`'s overlay `Approved State List ✔️` and its line "If you're a mom and you live in one of these states... listen up" (`2026-09-04-the-state-list-as-a-single-frame.md`). The brand's own guidelines mark the State Angle CTA "Select States Classic" as one that "converts WELL!" (`stated`, Section 7 via `brand-identity-analysis.md`). Mechanism: the open loop, the reader has to look for her state.
- **ICP and emotion:** the cold clicker. Curiosity, then either relief or a clean no. Level 1, a stated exception: the question is a gate, not a feeling, and a gate is the point of this arm.
- **Hero it sits over:** the wall of state names (`visual-vocabulary.md` shot 4). Required, not optional: the H1 is a question and the list is its answer.
- **Source:** the overlay and transcript above; the "30 seconds" rail from `moms-53 3`. Also the complaint this answers: *"Why is this being shown in IL if it's not on the list???😭🤦🏼‍♀️"* (`moms-53 3`, 2026-09-02) and *"It's not in my state."* (2026-04-10, `website-and-product-audit.md`).
- **Why, and the number against it:** it is the only H1 of the five that is honest about the gate before she types. But the roadmap ran this exact mechanic on the trustworthy ratio: `moms-53 3` took 2,127 link clicks and produced 127 leads, 5.97% leads per link click, against `moms-63 2b`'s 12.25% in the same window (`strategic-roadmap.md`, roads not taken 6). The state list buys the cheapest clicks in the account and converts them worst. Expect this arm to lose on leads per link click, by about half if the ad pattern holds on the page. It earns its slot only if the team can read gate two, because the leads it does produce are pre-screened on the one thing the brand can check without a phone call. Run it last, and only if lead quality feedback from the partner agencies is coming back.

---

## What to test first

Test 1 against the control. It is the roadmap's central message, it has never been on the page, and its source ad is the cheapest compliant lead in the account's static library. Test 3 second: it costs nothing and it answers the exact words she types under the ads. Run one challenger at a time against the control on `www.` only, each on its own URL so leads per link click reads by ad. `Moms43 - 4 - V3` alone sent 21,230 link clicks in 90 days (pull, 2026-09-07), so a week per arm is plenty at current spend.

Not in this set: a savings number. "Save up to 30%" is a rail phrase and belongs in the subhead, but the roadmap's own read is that the saving is the thing the account has led with for twenty-one months, so none of the five leads with it. Also not here: the `already-knows` line ("a mom is a mom whether her kid is four or twenty-four"). It is a segment test, not a page test, and belongs on a page variant she is sent to on purpose.

---

**Brand Context Applied:**

- **What I used:** the running text_hook and lifetime static headline corpus, pulled 2026-09-07; the account's own rail phrases from the winners' transcripts; the employer-plan comment cluster and the 2026-05-05 "you can decline the coverage" comment; the live trust-check comments; the pain phrases in `voc-pain-phrase.md`; the brand's State Angle CTA guidance; the roadmap's Priority 2 (drafted, unapproved); idea-bank entries on the decline line, the real-insurance line, the state list, the experience-over-number read, and one-specific-moment headlines.
- **What I avoided:** every flat savings number (the "24% cheaper" and "saving you 20% or more" surfaces are named as off limits); the words cheap, discount, policy, ACA, exclusions, guaranteed; any government or marketplace reference; any "no calls" promise; a dollar figure in the H1; "Approved by thousands of Mom's across America" as a receipt, since no count behind it exists; the brand-voice body copy register.
- **Why this fits:** the account is video-only by choice right now and pushes about $1,150 a day at one page ($103,938.70 over 90 days, derived, not a pull). The H1 on that page is the cheapest test the brand can run this month, and the page has never carried the message the roadmap says the whole account should lead with. Roadmap is unapproved, so the ranking here is provisional.

This is everything I know about static ad design.
This is based on everything I've learned about writing effective problem/solution headlines

---

## Gate receipts

**Grounding Review (context-grounding-review, 2026-09-07):** first pass bounced on seven items: word counts wrong on four of five (two H1s at ten, one at eleven), a pull receipt the log could not see, the largest static family missing from the baseline, the hero image held constant against `static-ad-design.md`, the wrong counter for the read, the state-list counter-evidence left out, and two labels. All seven fixed; the three trust-check quotes re-pulled by SQL with row ids. Second pass: **grounded**, every claimed pull in the log, counts verified 9 / 9 / 8 / 9 / 7, every hero pairing an in-play verified shot. Two inline edits applied. Trace: `self-improvement/reasoning-traces/2026-09/2026-09-07-headlines-grounding-bounce.md`.

**Voice Review (creative-voice-review, 2026-09-07):**

```
VERDICT: ships
LINT: 0 flags, density 0.00 (before) -> 0 flags, density 0.00 (after)
FLAGS: Test 2 rewritten ("See if you qualify for a $0 deductible option." -> "Moms, you may qualify for a $0 deductible option."), because the H1 and the button were the same sentence and the arm said "qualify" three times in forty words. Four H1s, the subhead and the button: keep.
CONFLICTS: none. Test 3's "real insurance" is the brand's own stated description; left as the brand's claim to own.
RESIDUAL: none on the five H1s.
```
