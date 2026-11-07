# Company brain

Your company's second brain, in your own repo. Operators decide how the company sells here. Ownable shows your team and their agents what you choose to share.

Markdown is the source of truth and git is the history.

## Get started

Paste this into your agent:

```
Clone https://github.com/NousC/company-brain into a temporary folder, read GET-STARTED.md and follow it.
```

Your agent researches your company, upgrades the repo you have or creates a private one, and drafts your doctrine, strategy and playbooks. Then it connects Ownable, shares what you approve with your team, and sets up your first automations. It asks only what it can't find.

## How it works

| Part | Holds | Who uses it |
|---|---|---|
| **This repo** | Doctrine, strategy, playbooks, initiatives, decisions, skills | Operators |
| **Ownable** | Customer truth from calls, email and CRM, plus the documents you push | Everyone, in the app and over MCP |
| **Their agents** | Where the work happens: Claude, Grok Bot, ChatGPT | Everyone |

Nothing syncs between this repo and Ownable. When something is ready for the team, an operator pushes it into **Documents** with `/push-document` and chooses who can see it: only them, operators or everyone. People read it in the sidebar, and their agents read it through the `search` tool. To send a new version, change it here and push again.

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
