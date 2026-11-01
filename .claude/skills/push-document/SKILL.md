---
name: push-document
description: Push a document from this repo into Documents in OpenNous, so the team sees it in the sidebar and their agents can read it. Use when an operator says "push this", "share this initiative with the team", or "put the objection handbook in OpenNous".
---

# Push a document

A document reaches the team only when an operator pushes it. Pushing the same title to the same folder sends the next version.

1. **Confirm you're allowed.** Call `whoami`. Only a workspace owner or admin can push. If this person can't, say so and stop.
2. **Read the file** they named, and name the document from its first heading.
3. **Check it's safe to share.** Flag secrets, candid notes about people, and client details that don't belong with this audience. Never push anything from `People/`.
4. **Ask who can see it,** unless they already said:
   - `operators`: owners and admins
   - `everyone`: the whole team and their agents
   - `only_me`: just this person
5. **Choose the folder:** Initiatives, Strategy, Doctrine, Objections, or the name they give.
6. **Show the title, folder and audience,** and wait for a yes.
7. **Push it:** call `documents` with `title`, `folder`, `markdown` and `shared_with`. Send the whole file.
8. **Log it:** add a line to `CHANGELOG.md` as `date · what changed · who it reached`.

The repo stays the source. Nothing syncs back, so to change a document, edit it here and push again.
