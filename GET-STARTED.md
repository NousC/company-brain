# Get started

Instructions for the agent setting up this company brain. Follow them in order, one step at a time. Keep every message short and plain.

If your tool has a task list, put these seven in it. If it doesn't, start each reply with the step, such as "Step 3 of 7: Your repo".

1. Find the company
2. Find the brain
3. Your repo
4. Build the brain
5. Connect Ownable
6. Share it with the team
7. Start

Open by telling them what this ends with, in these words or close to them:

> You'll end up with a private repo where you decide how the company sells, and Ownable delivers what you choose to your team and their agents. I'll do the research and drafting. You only answer what I can't find.

**Ask as little as you can.** Find it before you ask it. Never send a list of questions. Before step 4 you need one yes, in step 2. After that, ask at most three things, once.

## 1. Find the company

Work it out from what's here: `whoami` if Ownable is connected, the git remote, the folder, their email domain. Then read the company's website and public sources: what it sells, to whom, its pricing, its competitors.

Ask which company only if you still can't tell. If they name a website, use it.

## 2. Find the brain

Look in the current folder, then at the repos you can reach. A brain holds how the company sells and decides. Product code isn't one. Neither is a template whose files are still blank.

Then say what you found and what you'll do, in a few lines:

- **A brain with real content:** upgrade it. Name the repo and say what you'd keep.
- **Nothing real:** create a new private repo. Suggest the name `<company>-brain`.

If their knowledge lives in Notion, Google Docs or elsewhere, create a new repo and read those as sources.

Wait for a yes. Change nothing before it. That's the only approval you need before you start building.

## 3. Your repo

The template you cloned to read this is never where you work. Never push to `NousC/company-brain`: it's public.

**Check you can save first.** Web agents often run in a temporary session that can't create repos or push, and anything left there is lost when it ends. Before you write anything, find out if you can push to the repo you'll use. If you can't, stop and give them these choices:

1. **Run it on their machine (best):** paste the same line into Claude Code or another agent there.
2. **Give this session access:** they create the repo, grant this agent push access, and send you the link. For a new repo, that's **Use this template** on https://github.com/NousC/company-brain, then **Private**.
3. **Carry on anyway:** you build here, and at the end hand them everything as a `git bundle` or a zip. Say plainly that it isn't saved until they download it.

**New repo:**

```
gh repo create <owner>/<company>-brain --private --template NousC/company-brain --clone
```

**Upgrade:** work in their repo, on a new branch called `company-brain-setup`. Clone it first if it isn't in this folder. Their main branch doesn't change until they merge.

The rule is one home for each job. Where a file or folder of theirs already does a job, such as their own ICP file or meetings folder, keep it and skip the template's. Never overwrite anything, and copy file by file, not whole folders.

1. **Copy what's missing:** `CHANGELOG.md`, `DECISIONS.md`, `OVERVIEW.md`, `GET-STARTED.md`, `Doctrine/`, `Strategy/`, `People/`, `Initiatives/`, `Rollouts/`, `Skills/` and `.claude/skills/`. Add `Clients/`, `Partners/` and the other folders only if they'd use them. Add `README.md`, or save it as `BRAIN.md` if they have one.
2. **Playbooks:** if they already keep sales pages in a folder, new pages go there and `Playbooks/` isn't needed. If they don't, copy `Playbooks/`, leaving out any page they already have. Copy a blank page only when you're about to fill it. List where each playbook lives in `OVERVIEW.md`.
3. **Same-name skills:** keep theirs and install ours as `company-<name>`, such as `company-rollout`. Change the `name:` line, update the references in the files you copied, and tell them.
4. **Config:** add the `ownable` server to their `.mcp.json`, and add the template's `.gitignore` lines to theirs.
5. **`CLAUDE.md`:** add the template's whole file at the end of theirs, under `## Company brain`. Where the two disagree, such as spelling or style, theirs wins. Copy the file if they have none.
6. **Fix the map.** In what you copied, point any mention of a folder you skipped, such as `Playbooks/` or `Internal Meetings/`, to the home they use.
7. **Moves:** don't rename anything to match the template. To suggest a move, list it in a table with the reason, and move it only after a yes.

**Either way,** check the repo is private with `gh repo view --json visibility`. If it's public, say so and ask before you write anything about strategy or people. If it has no remote, ask them to create a private one, or carry on locally and tell them it isn't backed up.

## 4. Build the brain

Run `/team-setup`, or follow `.claude/skills/team-setup/SKILL.md` if you can't run it. Do its first part, **Build**. It needs no Ownable account.

Commit and push when it's done. On an upgrade, open a pull request if there's a remote, and tell them it's ready to read.

## 5. Connect Ownable

Call `whoami`. If it works, say which workspace you're connected to and go to step 6.

If it doesn't work, tell them what Ownable adds:

> The brain is what you decided. Ownable is what's really happening: it reads your calls, email and CRM into one record per account, and spots objections, competitors and buying signals. It's also how the brain reaches your team. You push a document from this repo, your team reads it in the sidebar, and their agents read it through `search`. Nothing goes across unless you push it.

Then give them the two steps:

1. **Create an account:** https://app.opennous.cloud/signup. It's free for 14 days with no card. The app walks you through connecting your email, notetaker and CRM. Your history starts syncing on its own.
2. **Connect this agent:** in Claude Code, run `/mcp`, choose `ownable` and sign in as yourself. In any other agent, run `npx -y @opennous/cli@latest init`, or follow the Connect step in the app.

Tell them to say when it's done, then call `whoami` again.

If they don't want Ownable now, stop here. The brain works without it. Add "Connect Ownable" to **Needs attention** in `OVERVIEW.md`, commit it, and tell them to ask you to continue with `GET-STARTED.md` when they're ready.

## 6. Share it with the team

Do the second part of `team-setup`, **Share**.

## 7. Start

Call the `start` tool and follow what it returns. It shows what's connected and what's in the workspace, sets up their automations, and runs one so they can see it work. Don't repeat anything you've already covered.

Finish with what's done, then the single next step. If their history is still syncing, that step is to come back when the app says it's done and run `brain-health`, which checks the drafts against their real calls and deals.
