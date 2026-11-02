---
name: delegate
description: Find what to delegate to your agent or to an automation. Use when someone asks "what can I delegate", "what can I automate", "what do I keep doing by hand", or "find me a skill".
---

# Delegate

Finds the parts of this person's job an agent could take off them, then builds the one that's worth most.

1. **Look at what repeats** in their week: `tasks`, `attention`, `my_desk`, and what they keep asking you for. Ask them what they dread doing.
2. **List up to five opportunities,** each in one line: what the job is, how often it comes up, and which kind it is:
   - **Skill:** a repeatable job they run with their agent, when they ask.
   - **Automation:** a RevPlay that runs by itself on a trigger or schedule.
3. **Rank them** by how often they happen and how little judgment they need. Say which you'd do first and why.
4. **Check it isn't already covered,** with `my_desk` and `rev_plays`.
5. **Build the one they pick.**
   - A skill: write it to the bar in `Skills/README.md`, show the text, then save it with `my_desk { save_title, save_body }`.
   - An automation: draft it with `rev_plays`, with what starts it, the steps and where the result goes. Show the preview and wait for a yes.
6. **Keep people in charge.** Anything a customer would see stays a draft for a person to send.
7. **If it could help the team,** tell them to ask an operator to share it.
