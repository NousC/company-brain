# delegate

_Find what to hand off. Use when someone asks "what can I delegate", "what can I automate", "what do I keep doing by hand", or "find me a skill"._

Look at what repeats in their week: call `tasks`, `priorities` and `my_desk`, and think about what they keep asking you for. Ask what they dread doing.

List up to five opportunities, one line each: the job, how often it comes up, and which kind it is:

- **Skill:** a repeatable job they run with their agent when they ask.
- **Automation:** a RevPlay that runs by itself on a trigger or schedule.
- **Living document:** a RevPlay that keeps a company document current, like new objections feeding the objection playbook or won and lost deals feeding the ICP file.

Check `search` for documents that go stale, or that could be fed by calls, deals or signals. If one should exist and doesn't, say so.

Rank them by how often they happen and how little judgment they need. Say which you'd do first and why. Skip anything `my_desk` or `rev_plays` already covers. If nothing is worth handing off, say so.

Build the one they pick:

- A skill: name the moment it's for and what good output looks like, with a number, like "two to five items". Show the text, then save it with `my_desk { save_title, save_body }`.
- An automation: draft it with `rev_plays`, with what starts it, the steps and where the result goes. Show the preview and wait for a yes.
- A living document: the same, with a trigger such as `call_ended`, `deal_closed_won`, `deal_closed_lost` or `account_signal`, an agent step, then a `document` step with the document's id. Only an admin can share this RevPlay, so if this person isn't one, write it up for an operator. If the document doesn't exist yet, an operator has to push it first.

Anything a customer would see stays a draft for a person to send. If it could help the team, tell them to ask an operator to share it.
