# Health For Moms — the brand brain

This is Health For Moms' brain. It's a set of plain text files that hold everything Parker knows about this brand: who the customer is and the exact words she uses, what the ad account is actually doing, what the strategy should be, and the ideas that come out of it. Parker reads these files every time you ask it something, so its answers come from real evidence about this brand instead of general marketing advice.

**You never have to open a file to use this.** Just talk to Parker and ask for what you want. Everything below is here so you can look under the hood when you want to.

New here, or just cloned this? Run **`/get-started`** and Parker will walk you through it at whatever level you're at.

---

## What's in here

**The strategy — start here if you read nothing else.**

- [`strategy/strategic-roadmap.md`](strategy/strategic-roadmap.md) — the diagnosis and the three priorities in order. **Still awaiting approval.** Everything in the idea bank was graded against it, so approving or changing it re-sorts what comes next.
- [`strategy/`](strategy/) — the four reads the roadmap was built from: who to talk to, what to sell, what to say, and who should say it.

**The evidence underneath it.**

- [`sub-context-docs/`](sub-context-docs/) — the fourteen foundation reads. Brand identity, the website and product, the category and market, the competitive picture, the customer journey, community, reputation, organic channels, performance targets, the marketing calendar, operations and team, the ad-account read, and the visual shot library. [`brand-profile-narrative.md`](sub-context-docs/brand-profile-narrative.md) is the summary of all of it.
- [`personas/`](personas/) — who actually buys, plus [`voice-of-customer/`](personas/voice-of-customer/), the exact language pulled from 1,342 comments under the brand's own ads.
- [`source-pulls/`](source-pulls/) — the raw evidence the personas were built from. Some of these are honest blanks; open the file rather than judging by the name.
- [`audits/`](audits/) — the recurring reads by month and quarter. Hook audits, performance reports, the organic read, whitespace, and the 90-day audits. **The newest one is what's true right now.**

**The questions and the ideas.**

- [`open-loops/`](open-loops/) — the graded list of what nobody knows yet that would change the strategy if answered. 57 questions, 14 at the top of the list.
- [`hypotheses/`](hypotheses/), [`validations/`](validations/), [`re-validations/`](re-validations/) — the research pipeline that turns those questions into answers.
- [`idea-bank/`](idea-bank/) — 45 captured ideas plus [`evaluation-2026-09-04.md`](idea-bank/evaluation-2026-09-04.md), the ranked read on them.

**The live notes.**

- [`running-notes/`](running-notes/) — what winning means here, the brand's standing rules, what the brand hasn't told us yet, when every document is due for a refresh, and the log of what the brain did on its own.
- [`brand-lens.md`](brand-lens.md) — this brand's own tribal knowledge. Voice rules, what's worked, what's failed, what's off limits. It sits on top of everything else, and where it disagrees with a general rule, it wins.
- [`expert-insights/`](expert-insights/) — where outside expert knowledge lands when you feed Parker a source. Empty until you do.

**The machinery.**

- [`CLAUDE.md`](CLAUDE.md) — Parker's operating instructions for this brand. The hard rules live at the top.
- `.claude/skills/` — the 26 playbooks Parker runs. Scriptwriting, hooks, headlines, iterations, ad-account analysis, AI ad generation, the research pipeline, and the routines below. You don't call these by name; just ask for what you want.
- `parker-system/` — the method itself, pinned to release `v15`. Read-only. It updates through `/update-brain`, never by hand.
- [`schedules/`](schedules/) — the six routines that run on their own.

## What runs on its own

Six routines keep this brain current without anyone asking:

| Routine | When | What it does |
|---|---|---|
| Dreaming | Daily, 05:00 | Reads the day's conversations and proposes what to change |
| Idea hunt | Weekly | Finds and grades new creative ideas against the strategy |
| Research | Weekly | Turns open questions into tests, runs them, folds the answers back in |
| Refresh | Weekly | Re-runs anything that's gone stale |
| Self-improvement | Weekly | Decides which proposals get promoted, with you in the loop |
| Standard check | Weekly | Offers anything new from the Parker method. Offers only, never overrides |

Run `/setup-routines` to change a cadence or turn one off. On a brain cloned to a new machine these arrive switched off, since schedules can't travel in the files themselves.

## Things to know before you trust a number

- **This is lead generation, not ecommerce.** Zero purchase events by design. Every read runs on cost per lead and lead volume. ROAS, AOV and purchase value are meaningless here and never get reported.
- **A cheap lead is not a winner.** The team's bar has two gates: cost per lead, then lead quality. Parker sees the first and cannot see the second, because lead quality lives with the partner agencies. Every recommendation in here clears gate one only, and says so.
- **The only first-party customer language is ad comments.** Customer reviews and post-purchase surveys are confirmed empty. So Parker says "commenters under the brand's paid ads said," never "customers said."
- **All numbers are Meta-reported.** Northbeam isn't connected, so nothing here is multi-touch.
- **No competitor tracking yet.** Deferred by the team. Adding rivals in the Parker app fills that whole branch in without redoing anything else.

## Working with this

**Save your work.** This lives in the team's own GitHub at `insuranceyeti/creativeyeti`. Parker commits and pushes every change as it makes it, so you don't have to ask.

**Bring teammates in.** Anyone you add to the repository on GitHub can clone it and work off the same brain. Their conversations can propose updates, and nothing lands until it's reviewed.

**Grow it.** Correct Parker when it's wrong, tell it what it doesn't know, connect more of your tools. It keeps its own notes current as you go, and the more you put in, the sharper it gets.
