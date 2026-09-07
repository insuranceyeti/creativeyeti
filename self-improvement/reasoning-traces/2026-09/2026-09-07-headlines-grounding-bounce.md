---
date: 2026-09-07
skill: headlines
trigger: context-grounding-review bounce, first pass
task_shape: landing page hero H1 test set, 5 candidates, control unseen (site blocked by egress policy)
status: captured, not yet promoted
---

# Headlines grounding bounce — landing page H1 tests

**What the gate caught, in order of cost.**

1. **Word counts were wrong on 4 of 5 candidates and the errors hid a hard-rule breach.** Two H1s at ten words, one at eleven, all labeled under ten. Candidate rule: print the count from a script, never from the writer's head, before the gate runs.
2. **A pull receipt named the wrong tool.** The draft attributed three live comment quotes to `search_facebook_ad_comments_semantic`. The call ran in this session's context and the quotes were real, but it did not appear in the Parker pull log, so the gate could not see it and read the receipt as false. Whether the log drops semantic calls or the call was logged elsewhere is unresolved; the fix is the same either way. Candidate rule: when a comment quote has to carry a live receipt, run `search_facebook_ad_comments_sql` (substring) as the citable pull; use semantic to find, SQL to cite.
3. **The baseline dropped the largest static family.** Pull 3 returned 12 rows and the draft listed 8, and the one it dropped first was `B1 samar- Copy` (4,441 leads, $12.21), the account's biggest employer-switch family and the direct parent of Test 1's reference. Candidate rule: the Baseline Studied block carries every row the pull returned, or says which were cut and why.
4. **"Only the H1 moves" contradicted `static-ad-design.md`.** The method says message and image move together and names one image under many headlines as the common failure. Candidate rule: a landing page hero test names the visual per arm from `visual-vocabulary.md` in-play shots, same as a static.
5. **The measurement plan used a counter the strategy layer had already written off.** `product-priority.md` line 89: landing page views are unreliable on this account; leads per link click is the ratio that survived. The draft cited the `go.` collapse as evidence and then proposed reading the test on the collapsed counter. Candidate rule: any "what to read" line on this brand checks `product-priority.md` first.
6. **A cited idea-bank entry's own counter-evidence was left out.** The state-list entry and roadmap road-not-taken 6 both carry 5.97% vs 12.25% leads per link click against the exact mechanic Test 5 proposes. Candidate rule: when a candidate cites an entry, carry the entry's strongest number against itself.

**What held:** compliance sweep, the roadmap-unapproved caveat, the www-only instruction, the AI-tells read, every static headline verbatim, the MOMS25 "real insurance" line, the 2026-05-05 decline comment.

**Cross-reference:** `2026-09-05-scriptwriting-grounding-bounce.md` (same family: loads claimed, not made). Two bounces in three days on receipts and counts, not on concept. The fix is mechanical: a pre-gate script that prints word counts and lists the rows every pull returned.
