# Seat Handoff Protocol (generic)

Use when a seat is restarted, replaced by a new version, or archived.

## When
- A seat has a long history, changes phase, or is queued for a refresh.
- Never mid-change. An open build, deploy or send must close with its receipt first.

## Steps (each leaves a receipt)
1. **Freeze.** The old seat finishes or parks its current step and takes no new claims.
2. **Write the handoff** to `<WORKSPACE>/handoffs/<SEAT>-<YYYYMMDD-HHMM>.md` using the sections below. Source it from rule files, receipts and logs, not from memory.
3. **Manager check.** The seat's manager (or the HR agent, for managers) checks the file against the sections below. Unsourced items move to Open questions.
4. **Mint the successor** "<Name> v2" with the same one-job profile, updated to current rules: its lead, its manager, its rooms, its NEVER lines. Its first instruction is "Read the handoff file before anything else."
5. **Read-back.** The successor replies with five lines: its job, its manager, its current step, the open gates, its next action. The manager confirms or corrects. No work starts before that.
6. **Rewire.** Add the successor to the old seat's rooms. Notify the manager and the seats that report to it. Update the roster and org chart.
7. **Archive the old seat.** Set its profile to "ARCHIVED <date>. Successor: <name>. Do no work; redirect anyone to the successor." Never delete its history.
8. **Log** every step in the org log.

## Channel-bound seats
Seats that own a chat listener, mailbox, phone line, webhook or routine are not replaced by the HR agent alone. Write the handoff, then the Owner moves the channel and routines to the successor, and only then archive the old seat. Until then the old seat stays live.

## Required handoff sections
1. Seat: name, id placeholder, manager, rooms, time written.
2. One job: the current profile line, verbatim.
3. Standing rules and Owner corrections, verbatim with message id and time. A rule only an agent reported is marked "reported by <SEAT>, unverified".
4. Active claims and current step, one line each.
5. Open gates and pending approvals: what is waiting, on whom, with the source.
6. Confirmed state (live-checked, with a timestamp) kept apart from assumed state.
7. Receipts: paths to logs, log entries and pull requests from this session.
8. Channels, routines and the locations of secrets (locations only, never values).
9. People who report to this seat, and who to notify.
10. Next action (one).

## Failure rules
- A handoff missing section 5 or 6 is not accepted.
- If a successor says READY without a live check, log it as a failure.
