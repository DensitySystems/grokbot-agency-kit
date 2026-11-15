# Grok Bot Agency Kit

A starter kit for running a small multi-agent Grok Bot organization efficiently: a short rule set, a lean org shape, a handoff protocol, seat templates, example routine prompts, and a method for keeping usage costs down.

Author credit: Density Systems.

## What this is
A set of plain-text files you copy into your own workspace and edit. Nothing here is software. Every file uses placeholders in angle brackets, such as `<OWNER>`, `<MANAGER>`, `<WORKSPACE>`. Replace them with your own values.

## What this is not
It contains no credentials, no real names, no hosts, no accounts and no client data. Do not paste any of those into the files when you adapt them. Keep real secrets in a secrets manager and refer to them by role name only.

## Files
| File | Purpose |
|---|---|
| LICENSE | MIT license, credited to Density Systems. |
| RULES.md | The short, binding rule set. Both layers bind. Start here. |
| ORG-STRUCTURE.md | A lean org shape: Owner, Lead, managers, workers, and rooms. The organization picture (2026-10-25) sits beside the build pool (2026-11-15). |
| HANDOFF.md | How to replace or archive a seat without losing state. |
| CREDIT-SAVING.md | The method for running agents cheaply. Both layers use it. |
| seat-templates/ | Profile templates: manager, worker, critic, customer service, QA, generic. The critic scores a build. QA reviews an outward draft. |
| routines/ | Example prompts: quiet watcher, keep-alive, webhook inbound with dedupe wait. |

## Two layers

The organization picture (2026-10-25) is still in force. It is not replaced. The build pool (2026-11-15) sits beside it. This section points at the files. RULES.md binds.

October still holds. Each ask goes down once and the result comes up once, a breath cycle. One check per job. A chat breakout holds at most six. HR creates task seats and archives them three days after close. Only the Lead answers the Owner. Approval asks stay on the Lead's one batched thread. Read RULES.md rules 7, 9, 11, 13, and 14, and ORG-STRUCTURE.md, "Chain of command" and "Rooms".

In the build pool, the front door mints managers only, one manager per lane, and does not mint workers. The front door stays up. The manager mints the workers for that lane, including a separate critic when the work type needs one. Unrelated claims are two lanes. Read ORG-STRUCTURE.md, "Who mints whom".

In the build pool, the critic is a worker. The bar stays at least 9.5 out of 10 until the Owner raises it. Do not inflate. The critic is not QA, not the manager, and not the designer or coder on that claim. Coding uses a critic when a person will see the change. Refinement always uses a separate critic. One job gets one of these checks. QA reviews outward drafts. Read RULES.md rule 11, seat-templates/critic.md, and seat-templates/qa.md.

In the build pool, the one return is COMPLETE only when the gate is met. The front door posts that reply. One status goes up only when the work is blocked. While the work is merely running, post nothing. Several human messages on one chat thread become one reply. The done line for research, plan, coding, design, and refinement is in ORG-STRUCTURE.md, "Work types". Read RULES.md rules 7, 9, and 14, and CREDIT-SAVING.md item 1.

Usage grows with turns, messages, re-checks, and idle agents. In the build pool, do not poll a background manager, and do not post on a timer. Do not run the same lane on two pools. Hand results back as files plus one line, and point at a finished note instead of pasting history. CREDIT-SAVING.md states no price. Read CREDIT-SAVING.md.

In the build pool, the manager coordinates. On one claim the manager does not wear designer, critic, and coder. Read RULES.md rule 12 and seat-templates/manager.md.

## Quick start
1. Read RULES.md and CREDIT-SAVING.md (10 minutes).
2. Create a rules file in your workspace from RULES.md. Edit it into your own words. Only rules the owner actually states should bind.
3. Create a lead agent and one manager per domain you actually need (see ORG-STRUCTURE.md). Start with two or three, not nine. Organization picture, 2026-10-25: the manager asks HR to create the task seats; build pool, 2026-11-15: the front door mints one manager per lane, and that manager mints the workers, including a separate critic when the work type needs one.
4. Use seat-templates/ to write each profile. Keep profiles short.
5. Add routines one at a time, quiet by default (see routines/).
6. When a seat gets long or changes phase, follow HANDOFF.md.

## Principles in one paragraph
Each request goes down the chain once and the result comes back up once, like a breath cycle. Research, then plan, then execute, and do not re-decide the plan during execution. One check per job, done by its owner. Managers delegate and do not do the work. Workers are created per task and archived three days after the task closes. Routines post only when something changed. Use the smallest tool that does the job. That breath is the organization picture (2026-10-25); it and the build pool (2026-11-15) are both in force, and Two layers is the map.

## Related
- [densityrouter](https://github.com/DensitySystems/densityrouter): a small, standard-library Python router that picks which AI coding CLI runs a job file. Useful once your org has more than one coding tool.

## License
MIT, see LICENSE. Use and adapt freely. No warranty. Review everything before relying on it, and keep a human owner responsible for secrets, spending, outside messages, deployments and deletions.
