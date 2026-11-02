---
name: brain-health
description: Find what's gone stale in the brain. Use weekly, or when an operator says "what's out of date" or "check the brain".
---


# Brain health

This skill proposes. It never applies a change.

1. **List what the brain depends on:** people named as owners, skills assigned, documents pushed, playbook claims.
2. **Compare with what's true now:**
   - Owners who left or changed role, from `People/Seats.md` and Settings → Team.
   - Skills or pins that mention people, stages or pages that no longer exist, from `assign`.
   - Pushed documents older than their source in this repo, from `documents` and git history.
   - Playbook claims that `read_intelligence` or recent calls now contradict.
3. **Default to no change.** Propose one only for something broken, something that drifted, or a real change in how the business works.
4. **Report** each proposal with what changed, the evidence and where to fix it. Repo fixes wait for the operator's yes; anything agents read goes through `rollout`.
