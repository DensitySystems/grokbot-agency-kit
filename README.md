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
| RULES.md | The short, binding rule set. Start here. |
| ORG-STRUCTURE.md | A lean org shape: owner, lead, managers, workers, rooms. |
| HANDOFF.md | How to replace or archive a seat without losing state. |
| CREDIT-SAVING.md | The method for running agents cheaply. |
| seat-templates/ | Profile templates: manager, worker, customer service, QA, generic. |
| routines/ | Example prompts: quiet watcher, keep-alive, webhook inbound with dedupe wait. |

## Quick start
1. Read RULES.md and CREDIT-SAVING.md (10 minutes).
2. Create a rules file in your workspace from RULES.md. Edit it into your own words. Only rules the owner actually states should bind.
3. Create a lead agent and one manager per domain you actually need (see ORG-STRUCTURE.md). Start with two or three, not nine.
4. Use seat-templates/ to write each profile. Keep profiles short.
5. Add routines one at a time, quiet by default (see routines/).
6. When a seat gets long or changes phase, follow HANDOFF.md.

## Principles in one paragraph
Each request goes down the chain once and the result comes back up once, like a breath cycle. Research, then plan, then execute, and do not re-decide the plan during execution. One check per job, done by its owner. Managers delegate and do not do the work. Workers are created per task and archived three days after the task closes. Routines post only when something changed. Use the smallest tool that does the job.

## Related
- [densityrouter](https://github.com/DensitySystems/densityrouter): a small, standard-library Python router that picks which AI coding CLI runs a job file. Useful once your org has more than one coding tool.

## License
MIT, see LICENSE. Use and adapt freely. No warranty. Review everything before relying on it, and keep a human owner responsible for secrets, spending, outside messages, deployments and deletions.
