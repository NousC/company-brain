# Company brain

Your company's second brain, in your own repo. Operators decide how the company sells here. OpenNous shows your team and their agents what you choose to share.

Markdown is the source of truth and git is the history.

## How it works

| Part | Holds | Who uses it |
|---|---|---|
| **This repo** | Doctrine, strategy, playbooks, initiatives, decisions, skills | Operators |
| **OpenNous** | Customer truth from calls, email and CRM, plus the documents you push | Everyone, in the app and over MCP |
| **Their agents** | Where the work happens: Claude, Grok Bot, ChatGPT | Everyone |

Nothing syncs on its own. When something is ready for the team, an operator pushes it into **Documents** in OpenNous and chooses who can see it: only them, operators or everyone. People read it in the sidebar, and their agents read it through the `documents` tool. Change it here and push again to send the next version.

## What goes where

| Path | What goes there |
|---|---|
| `OVERVIEW.md` | Where things stand right now. Read first. |
| `DECISIONS.md` | What you decided and why, newest first. |
| `CHANGELOG.md` | What went out to people and their agents. |
| `Doctrine/` | Rules everyone follows. Rarely changes. |
| `Strategy/` | This period's goals, motions, bets and what you won't do. |
| `Playbooks/` | How you sell: ICP, positioning, pricing, objections, competitors. |
| `Initiatives/` | Owned, dated work with yes-or-no success criteria. |
| `People/` | Seats and what each person owns. Stays here. |
| `Skills/` | Which skills operators and the team use. |
| `Rollouts/` | Each change that reaches people: proposed, approved, applied. |
| `Internal Meetings/` | Your own calls. |
| `Working Documents/` | Drafts. |
| `Clients/`, `Partners/` | One folder each. Copy `_Template/`. |

## Set it up

1. Click **Use this template** and keep your copy private. It will hold strategy and candid notes.
2. Open it in Claude Code and approve the `opennous` server, signing in as yourself.
3. Fill in `Doctrine/Doctrine.md` and `Strategy/Strategy.md`.
4. Run `/push-document` on the first file your team should see.
