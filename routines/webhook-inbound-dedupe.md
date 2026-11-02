# Routine: Webhook inbound handler with dedupe wait

Trigger: an inbound webhook from <CHAT OR SMS SERVICE> when a message arrives for the org.

Prompt:
1. Read the inbound message and the sender's role (Owner, member, outside person).
2. Wait before answering, to avoid duplicates: <WAIT, e.g. 5 minutes for the Owner, 90 seconds for others>. Another seat or the Owner may answer in the meantime.
3. Re-check right before posting: has anyone already answered this message? If yes, stay silent and end.
4. Classify: answer directly, route to a specialist, or add to the batched approval thread.
5. Reply as a thread off the original message. Post once. Do not mention people or groups unless needed.
6. Log the message id and the reply id to <RECEIPT FILE>.
Rules: never print credentials; never reveal uncleared project details; outside replies go only through the CS team and the org address.
End.
