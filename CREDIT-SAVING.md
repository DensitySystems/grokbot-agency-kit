# Credit-Saving Method

Usage cost grows with turns, messages, re-checks and idle agents. This method cuts all four.

The organization picture (2026-10-25) and the build pool (2026-11-15) both use this method. Where a numbered item names both, both apply.

## 1. Breath cycle
Each ask goes down once (Owner, manager, worker). The result comes back up once, when the work is complete. No mid-flow pings, no sideways forwarding, no status loops. A blocker rises once, to the next level only. A system that churns back and forth burns usage on coordination instead of work.

Organization picture, 2026-10-25: that is the cycle. Build pool, 2026-11-15: the result that comes up is COMPLETE, and only when the gate is met. One status goes up only when the work is blocked. While the work is merely running, post nothing. This is the same breath. A play-by-play status spends the next read on noise. A missing COMPLETE spends the next session too, because that session cannot tell the job finished.

## 2. One check per job
The seat that owns the job checks it once. Do not stack reviewers, extra managers or receipt checkers on top. Add a second check only where a mistake is expensive or irreversible (secrets, money, outside sends, deploys).

Organization picture, 2026-10-25: that is the check, and QA of an outward draft is that one check. Build pool, 2026-11-15: when the work type is coding and a person will see the change, and when the work type is refinement, the one check is a separate critic worker. The bar stays at least 9.5 out of 10 until the Owner raises it. Do not inflate a score. The critic is that one check. A critic plus another reviewer on the same job is the stack this item forbids. Parallel workers do not lower the bar. A second check is still only for a mistake that is expensive or irreversible.

## 3. Research, then plan, then execute
Spend effort up front. Once execution starts the plan is settled. No re-review, re-approval or re-research of what was already decided. Only a real blocker interrupts.

## 4. Managers delegate
Managers scope, plan and synthesize. They do not do the work and are not pass-throughs. Expensive, high-context seats stay small in number and stay thin in work.

Build pool, 2026-11-15: the manager does not wear designer, critic, and coder on the same claim. Use one background manager when the lane will outlive a single turn. Do not poll it. Do not post on a timer. A background manager is the wrong tool while the lane waits on the Owner for a gated yes.

## 5. Workers per task, archived after close
Create a worker for one task. Give it a short packet and thin context. When the task closes, archive the worker three days later (the delay allows follow-up questions). No idle seats pile up, and every seat that exists has a current job.

Organization picture, 2026-10-25: HR creates that seat and archives it three days after close. Build pool, 2026-11-15: the worker does one slice, then stops. The manager lasts for one lane, until the gate. The front door is long and thin and stays up after the job. Do not archive the front door under the three-day rule.

## 6. Quiet routines
A scheduled routine posts only when something changed. If nothing changed it ends silently. Check state first with the cheapest possible read, and only wake a larger model when there is something to act on. Keep routine prompts short. See routines/.

## 7. Right-sized tools
Match tool to job: a small, low-effort model or plain script for mechanical work (scans, formatting, polling), a stronger model for planning and judgment. Prefer a deterministic script over a model call when the answer is mechanical. Give each tool lane one designated tool.

## 8. Short packets, files over chat
Hand results back as files plus a one-line PASS or FAIL, not long chat transcripts. Keep seat profiles and rule files short, because they are re-read on every turn.

When a finished note already records where the result lives and the score, extend that result. Do not open a session to rediscover a path and a score already recorded. Point the packet at the note. Do not paste it.

## 9. Batch the human
Put every approval ask into one batched thread. One Owner reply can unblock many items, and quoted approvals (see RULES.md rule 5) are never asked twice.

## 10. Freeze the rules
After a slip, agents tend to add checks until overhead exceeds the mistakes. Log the failure as one line, fix it once at the size requested, and add no new rule without the Owner's words.

## Capacity

A build pool is the set of agent sessions that can run at once. Each session spends usage. Usage goes up when a session carries context it does not need, and when a later session repeats a read. This file states no price. Parallel workers spend usage side by side. They save clock time only when their outputs differ. The same lane on two pools spends the usage twice.

## Self-audit checklist
- Did any ask go down twice, or any result come up twice?
- Were two seats checking the same thing?
- Is any worker still alive more than three days after its task closed?
- Did any routine post when nothing changed?
- Was a large model used for a mechanical step?
- Were approvals asked outside the batched thread?
- Did anyone post while the work was merely running, or post COMPLETE before the gate was met?
- Did a later session rediscover a path or a score that a finished note already recorded?
- Was the same lane running on two pools?
