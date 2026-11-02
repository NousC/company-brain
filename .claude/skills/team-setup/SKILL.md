---
name: team-setup
description: Set up the company brain once, for the whole company. Use when an operator says "set up our brain", "set up the team", or has just connected OpenNous. GET-STARTED.md calls it for new repos and upgrades.
---


# Team setup

Run once, by an owner or admin. It shapes what they already have. It doesn't make them start over. It has two parts: **Build** needs only this repo, and **Share** needs OpenNous.

If you ran Build earlier, go straight to **Share**.

## Build

1. **Read before you ask.** Read this repo, any second brain they point to, and the company's website and public sources. If OpenNous is connected, read `insights` and recent calls through `activity`.
2. **Map it.** If they have content already, show how it fits `README.md` (`BRAIN.md` on an upgrade): what's there, what's missing, what to move. Move nothing without a yes. Doctrine and `CHANGELOG.md` are the only must-haves.
3. **Draft everything you can.** Write `Doctrine/Doctrine.md`, `Strategy/Strategy.md` and the playbooks: ICP, positioning, pricing, objections and a page per competitor. `Playbooks/ICP.md` in the template is the shape for the ICP. If they already have an ICP, keep that file and add the scoring sections at the end of it. Put new pages where `OVERVIEW.md` says playbooks live.
4. **Label each claim** as public, from their files, from calls, inferred or confirmed. Say where it came from and how sure you are. If you found little, say so and leave a line blank rather than invent it.
5. **Ask at most three things, in one message,** and only what you can't find. Usually: this period's goals, who's on the team, and what must never happen. Show the drafts first, so they correct rather than start from nothing.
6. **Write it down.** Fill `People/Seats.md` and start one initiative in `Initiatives/` with yes-or-no success criteria. Add confirmed calls to `DECISIONS.md` with the name of who confirmed them, from `whoami` or git. Put anything no one named has confirmed under **Needs attention** in `OVERVIEW.md`, and update the rest of that page.

## Share

1. **Check who's running this.** Call `whoami`. Stop unless they're an owner or admin.
2. **Check the workspace is theirs.** If its accounts don't match this company, say so before you change anything in it.
3. **Set the ICP.** Pass their filled-in ICP file, never a blank one, to `set_icp`, and say what came back. If no scoring model was built, tell them why. `whoami` shows whether an ICP is set.
4. **Choose what the team sees.** Propose which documents to push and who sees each, then run `push-document` for each one they approve.
5. **Give the team a start.** Propose the skills in `Skills/starter/` and any pins, then run `rollout` (`company-rollout` if they already had one).

Finish by saying what's done and the single next step. If history is still syncing, say to run `brain-health` once it's in, to check the drafts against real calls.
