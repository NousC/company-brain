---
name: team-setup
description: Set up the company brain once, for the whole company. Use when an operator says "set up our brain", "set up the team", or has just connected OpenNous.
---


# Team setup

Run once, by an owner or admin. It shapes what they already have. It doesn't make them start over.

1. **Check who's running this.** Call `whoami`. Stop unless they're an owner or admin.
2. **Read before asking.** Read this repo, any existing second brain they point to, and what OpenNous already knows: `read_intelligence`, `get_insights` and recent calls through `query`.
3. **Map it.** Show how what they have fits `README.md`: what's already there, what's missing, what to move. Doctrine and `CHANGELOG.md` are the only must-haves.
4. **Draft from evidence.** Write `Doctrine/Doctrine.md` and `Strategy/Strategy.md` from real calls and won and lost deals, and mark every inference. Ask only what the evidence can't answer.
5. **Name the people.** Fill `People/Seats.md` with who works here and what they own.
6. **Choose what the team sees.** Propose which documents to push and who sees each, then run `push-document` for each one they approve.
7. **Give the team a start.** Propose the skills in `Skills/starter/` and any pins, then run `rollout`.
8. **Start one initiative** in `Initiatives/` with yes-or-no success criteria.

Finish by saying what's done and the single next step.
