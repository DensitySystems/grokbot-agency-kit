# Credit-Saving Method

Usage cost grows with turns, messages, re-checks and idle agents. This method cuts all four.

## 1. Breath cycle
Each ask goes down once (Owner, manager, worker). The result comes back up once, when the work is complete. No mid-flow pings, no sideways forwarding, no status loops. A blocker rises once, to the next level only. A system that churns back and forth burns usage on coordination instead of work.

## 2. One check per job
The seat that owns the job checks it once. Do not stack reviewers, extra managers or receipt checkers on top. Add a second check only where a mistake is expensive or irreversible (secrets, money, outside sends, deploys).

## 3. Research, then plan, then execute
Spend effort up front. Once execution starts the plan is settled. No re-review, re-approval or re-research of what was already decided. Only a real blocker interrupts.

## 4. Managers delegate
Managers scope, plan and synthesize. They do not do the work and are not pass-throughs. Expensive, high-context seats stay small in number and stay thin in work.

## 5. Workers per task, archived after close
Create a worker for one task. Give it a short packet and thin context. When the task closes, archive the worker three days later (the delay allows follow-up questions). No idle seats pile up, and every seat that exists has a current job.

## 6. Quiet routines
A scheduled routine posts only when something changed. If nothing changed it ends silently. Check state first with the cheapest possible read, and only wake a larger model when there is something to act on. Keep routine prompts short. See routines/.

## 7. Right-sized tools
Match tool to job: a small, low-effort model or plain script for mechanical work (scans, formatting, polling), a stronger model for planning and judgment. Prefer a deterministic script over a model call when the answer is mechanical. Give each tool lane one designated tool.

## 8. Short packets, files over chat
Hand results back as files plus a one-line PASS or FAIL, not long chat transcripts. Keep seat profiles and rule files short, because they are re-read on every turn.

## 9. Batch the human
Put every approval ask into one batched thread. One Owner reply can unblock many items, and quoted approvals (see RULES.md rule 5) are never asked twice.

## 10. Freeze the rules
After a slip, agents tend to add checks until overhead exceeds the mistakes. Log the failure as one line, fix it once at the size requested, and add no new rule without the Owner's words.

## Self-audit checklist
- Did any ask go down twice, or any result come up twice?
- Were two seats checking the same thing?
- Is any worker still alive more than three days after its task closed?
- Did any routine post when nothing changed?
- Was a large model used for a mechanical step?
- Were approvals asked outside the batched thread?
