# Org Structure (generic)

Keep the org lean. Start with the lead plus the managers you need today. Add a domain only when work actually needs it.

Two layers are in force. The organization picture is 2026-10-25. The build pool is 2026-11-15. Where they differ, this file names the layer. Behavior that binds is in RULES.md. This file does not add a check RULES.md does not name.

## Chain of command
Owner > Lead > Chief of staff (optional) > Domain managers > Team leads (optional) > Workers

- **Owner**: the human. Sets goals. Gives the yes on money, outside sends, deploys, merges, deletions and final sign-offs.
- **Lead**: runs the single batched approval thread, briefs the Owner, routes requests to the right manager. Does no desk work. Only the Lead answers the Owner; workers and managers never answer the Owner directly.
- **Chief of staff** (optional): keeps day-to-day work moving across managers. Not a gate on every packet.
- **Managers**: scope, plan, request workers, synthesize results, report up once.
- **Workers**: one task from one packet. Return a result with a one-line PASS or FAIL.
- **HR agent**: creates and archives seats, keeps the roster, logs failures. Independent of the managers it serves. Organization picture, 2026-10-25: HR creates and archives task seats. Build pool, 2026-11-15: the front door mints managers, and the manager mints workers. HR still keeps the roster and the failure log. A failure still does not become a rule.
- **Customer-service (CS) team**: the only seats allowed to contact outside people.
- **Front door** (build pool, 2026-11-15): the seat where a request arrives and where the one chat-thread reply is posted. Mints managers only, one manager per lane. Returns nothing from worker transcripts. Approval asks stay with the Lead. The front door and the Lead may be the same seat.
- **Critic** (build pool): a worker. Scores one result once, at a bar of at least 9.5 out of 10, and names what is left. Does not inflate a score. Is not the designer or the coder on that claim. Is not QA.

## Who mints whom

Use the column for the room you are in. One lane, one manager. Unrelated claims are two lanes.

| | Organization picture, 2026-10-25 | Build pool, 2026-11-15 |
|---|---|---|
| **Front door** | Routes an incoming request to the manager who owns it. | Mints managers only. One manager per lane. Does not mint workers. A fan-out from the front door fills that long-lived session. |
| **Who creates the worker** | When a manager needs help, HR creates a seat for that one job. | The manager mints the workers for that lane, including a separate critic when the work type needs one. |
| **Who speaks to the Owner** | The Lead, on the one batched thread. Workers post in the room, never to the Owner. | Workers return text to the manager. The manager returns text to the front door. The front door posts one chat-thread reply. Approval asks still go through the Lead. |

## Work types

Pick the type before anyone is minted. The done column is the gate for COMPLETE. Rule 10 names that gate. These rows add no extra check.

| Type | Who | Done looks like |
|---|---|---|
| Research | Manager plus research workers | A few easy paths, with sources, and notes on terms of service and rate limits |
| Plan | Manager synthesizes | A plan note with milestones and gates |
| Coding | Manager mints a coder, and a critic when a person will see the change | A proofed change. When a person will see it, the critic has scored it |
| Design | A designer writes a brief, then a coder | Visual direction exists before pixels |
| Refinement | Designer, critic, and coder are separate workers | An honest critic score at or above the bar. One person does not wear all three hats |

Plans live with the job's notes. Critic notes live with the review. When the work is visual, COMPLETE includes where to look, the score, and the proof. The manager waits for the critic, when this table calls for one, before it returns COMPLETE text. Under the bar, the next pass receives the score and what is left.

## Domains (pick what you need)
| Domain | One job |
|---|---|
| Operations | Day-to-day go/hold, the live work log, routing between managers |
| People / HR | Seat creation, archive, roster, failure log |
| Growth | Marketing and sales together (small orgs merge them) |
| Customer service | Inbound messages, replies, support, QA of outward drafts |
| Finance | Books, invoices, expenses, budgets. Records and proposes, never moves money |
| Projects | Builds and deliverables, including research |
| Data | Sources, freshness pulls, metrics |
| Security and compliance | Access, secrets handling, backups, policy |
| Build and IT | Coding work and infrastructure changes |

Small orgs combine functions: sales with marketing, HR inside operations, legal outsourced to humans.

## Growing a domain
A manager runs roughly five to eight direct seats. Past that, or when one stream runs daily, promote a team lead and open a team room. Per-task work gets a task room that closes when the task closes. Retire anything idle for 14 days to a bench.

That span of five to eight is the organization picture. Build-pool parallelism is under Rooms. It does not raise the chat-room cap of six.

## Rooms
- Department room: managers and leads of a domain.
- Team room: a lead and its workers.
- Task room: one packet, one worker.
- Maximum six members per room. That cap is the chat breakout, organization picture, 2026-10-25. Workers post only in their task or team room, never to the Owner.

### Chat breakout, 2026-10-25

Jobs with several workers run in the manager's breakout room. The room holds at most six. A larger job gets a sub-lead who splits the work and collects the results. Workers post their results in the room, never to the Owner. If a turn has nothing essential to say, it says nothing.

### Build pool, 2026-11-15

A build pool is the set of agent sessions that can run at once. It is a different room from the chat breakout. A manager may run many workers at once, including a large batch, only when their outputs do not overlap. The manager mints those workers. The front door does not. The critic bar stays at least 9.5 out of 10. Parallel workers do not lower it. Two workers on one unsplit problem waste the pool. Split the outputs, then run them side by side. A large batch of pool workers is not a chat room of that size.

## Sessions

| Session | How long it lives | What it holds |
|---|---|---|
| Front door | Long, and thin. Later reads see it again, so it stays small. | The clipped request and the manager's return. It does not hold worker transcripts. |
| Manager | One lane, until the gate. | The packet. It slices work to workers. It does not take the front door's full history. |
| Worker | One slice, then stop. It does not sit idle on the lane. | That slice only: what to read, where the result lives, and the gate. No posting. No minting. |

The three-day archive is the organization picture for task seats. The front door is not archived after one job.

One lane has one manager. Do not run that same lane on two pools at once. Two managers on one lane spend the usage twice.

Use one background manager when the lane will outlive a single turn. A multi-step job and a critic loop qualify. Do not poll it. Do not post on a timer. When it returns, the front door receives COMPLETE, or one blocked line. A background manager is the wrong tool while the lane is waiting on the Owner for a gated yes. Stop, and return the one blocked line.

A handoff to a later session on the same lane is three things: the finished note, where the result lives, and what is still open. Seat replacement still follows HANDOFF.md. The chat thread plus where the result lives is the record. Before the front door is posting, the note kept with the job is the record.

## Standard flow
1. The Owner and the lead research and decide direction together.
2. The lead asks the operations manager for a workflow and skill pattern, then hands a suggestion to the domain manager.
3. Organization picture, 2026-10-25: the manager asks HR to create the task seats, operates the team, synthesizes, and pushes the result up. Build pool, 2026-11-15: the front door mints this one manager; the manager mints the workers, including a separate critic when the work type needs one, and returns text to the front door.
4. Anything needing approval goes into the one batched thread.
5. Organization picture, 2026-10-25: the task closes and HR archives its workers three days later. Build pool, 2026-11-15: each worker stops at the end of its slice. The front door stays up and posts COMPLETE when the gate is met.

## Packets

A packet is the short hand-off from one manager to one worker, for one job. The build pool uses this same packet. Fill it before workers are minted. A dump that arrives anyway is reshaped into one job first. Extra claims wait for their own lane.

1. Objective: one sentence, including what done looks like. Name the lane and the work type: research, plan, coding, design, or refinement.
2. Output: where the result goes, in words. When a finished note already records where it lives and the score, point at that note. Do not paste the note or the history.
3. Tools and boundaries: what is allowed, the short list of files to read, and one line for what is out of scope. Stop and return at any step that needs a yes. Do not say "read the whole workspace."
4. Budget: when it runs out, return partial results instead of looping. For coding a person will see, and for refinement, name the separate critic. The bar is at least 9.5 out of 10. Do not inflate.

The worker hands the result back as a file plus one line: PASS or FAIL. The manager reads it and synthesizes.

The same four lines, shown filled:

```text
1. Objective: <lane>. <work type>. <one claim>. Done: <one sentence>.
2. Output: <where it lives, in words>. Prior finished note: <pointer, or none>.
3. Tools and boundaries: <what is allowed>. Read: <short file list>. Out of scope: <one line>. Stop at a gate.
4. Budget: <when it runs out, return partial work>. Critic: <separate worker when the work type needs one>. Bar at least 9.5 out of 10. Do not inflate.
```

Signs the packet was not shaped:

- A second job added with "while you are in there."
- "Read the whole workspace," with no file list.
- A request for status mixed into the deliverable.
- A new session opened because the last one felt full, while the gate is unchanged.

## Seat law
Each manager keeps a short law file for its team: its one job, its manager, its rooms, its gates, its NEVER lines, and the Owner's rulings quoted verbatim with their message ids and times. Seat law may narrow the org rules but never contradict them. When a team uses the build pool, the seat law names that layer. Seat law may narrow these rules. It may not contradict RULES.md.
