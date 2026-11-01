# CLAUDE.md

Read this at the start of every session. This repo is the company's second brain. Operators work here.

Read `OVERVIEW.md` first. `README.md` says what goes where.

## Rules

1. **Nothing gets deleted.** Supersede it or move it. Git keeps the history.
2. **Decisions go in `DECISIONS.md`** the same day, with why, who and the source. Never add one a person hasn't confirmed.
3. **Don't state possibilities as facts.** Mark inferences and how sure you are.
4. **No secrets in this repo.** Point to where they live.
5. **Client material stays in the client's folder.**
6. **Nothing external goes out unreviewed.** Its owner reads it first.
7. **Nothing leaves this repo on its own.** A document reaches the team only when an operator pushes it with `/push-document` and says who can see it.

## Keep it current

| When this happens | Update |
|---|---|
| A decision is confirmed | `DECISIONS.md`, then `OVERVIEW.md` and any page it changes |
| A rule everyone follows changes | `Doctrine/Doctrine.md`, after logging the decision |
| This period's goals or bets change | `Strategy/Strategy.md` |
| Work is owned, dated and bigger than one change | A file in `Initiatives/` |
| Something is pushed to the team | A line in `CHANGELOG.md`, and a page in `Rollouts/` if it changes how people work |
| Someone joins, leaves or changes role | `People/Seats.md` |

Whenever you touch `OVERVIEW.md`, set its **Last updated** line to today.
