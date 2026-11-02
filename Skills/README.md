# Skills

Operator skills live in `.claude/skills/`, where Claude Code loads them. Team skills live in OpenNous: assign one with `/rollout` and each person's agent reads the current version through `my_desk`, with no file to install.

## Operators

| Skill | Job |
|---|---|
| `team-setup` | Sets up the brain once, from what you already have |
| `push-document` | Pushes a document into OpenNous and sets who can see it |
| `rollout` | Previews, applies and records a skill or pin |
| `audit` | Compares the plan with what's really happening |
| `brain-health` | Finds what's gone stale, and only proposes fixes |
| `new-seat` | Gets a new person working |

## Team

`Skills/starter/` has six to adapt and assign to everyone: `my-day`, `meeting-prep`, `after-call`, `follow-up`, `account-plan` and `delegate`. `delegate` finds what a person could hand to an agent, then builds it as a skill or a RevPlay.

## The bar for a skill

- Build it around what the person needs, not around data sources.
- Name the moments it should catch, with an example.
- Set a number: "two to five items", not "a few".
- Say what it must not do.
- Give it permission to say nothing.
- Say what to do when there's little data.

Two different people should get different output. If they wouldn't, it isn't specific enough.
