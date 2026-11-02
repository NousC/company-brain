---
name: rollout
description: Give a skill or pinned instruction to a person, a role or everyone, with a preview and a record. Use when an operator says "roll this out", "give the SDRs this skill", "pin this for the team".
---


# Rollout

Anything an agent reads from `assign` it will act on, so people decide what goes out.

1. **Confirm who's running this.** Call `whoami`. Only owners and admins can assign.
2. **Sort the rule.** Who needs it, and when?
   - Everyone, always: it belongs in `Doctrine/`.
   - Always, for one person or role: a pin.
   - One recurring job: a skill.
   - Just this once: tell the person.
3. **Write it** to the bar in `Skills/README.md`, grounded in their real work. Never include strategy notes or notes about the person.
4. **Check what's there.** Call `assign` with no arguments, or `user` for one person, so you update instead of duplicating.
5. **Preview.** Show the full text, who gets it, and what it replaces. Wait for a yes. Never skip this, even for small changes.
6. **Apply** with `assign`.
7. **Record it.** Write `Rollouts/YYYY-MM-DD Title.md` (proposed, approved, applied) and add a line to `CHANGELOG.md`.

To undo something, read `changes` and roll that change back.
