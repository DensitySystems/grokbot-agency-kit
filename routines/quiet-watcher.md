# Routine: Quiet watcher (posts only on change)

Schedule: every <INTERVAL, e.g. hourly>.

Prompt:
You watch <SOURCE: mailbox, feed, folder, status page>. Keep the last-seen state in <STATE FILE>.
1. Read the source with the cheapest available method. Compare to the state file.
2. If nothing changed, update nothing, post nothing, and end silently.
3. If something changed, write one short summary (what changed, where, whether action is needed) and post it once to <ROOM>. Update the state file.
4. If an item needs the Owner's yes, add it to the single batched approval thread instead of messaging the Owner directly.
5. Never print credentials. Never send outside messages.
End.
