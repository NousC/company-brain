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
5. **The folder is where the file lives.** `Playbooks/objection-playbook.md` goes in Playbooks, and the folder is made if it's new. Never choose one or ask. A file at the repo's root goes in `General`.
6. **Show the title, folder and audience,** and wait for a yes.
7. **Fold in what RevPlays added.** If the document is already in OpenNous, open it with `search`. If it has a `New from RevPlays` section, merge those points into the file here, then push with `updates_folded: true`.
8. **Push it:** call `search` with `path`, `title`, `markdown` and `shared_with`. Send the whole file. Pass `folder` only for a file at the root.
9. **Log it:** add a line to `CHANGELOG.md` as `date · what changed · who it reached`.

The repo stays the source. To change a document, edit it here and push again.
