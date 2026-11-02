# Routine: Keep-alive

Schedule: every <INTERVAL, e.g. 30 minutes>.

Purpose: keep a long-lived listener (chat connection, webhook, session) from silently dying.

Prompt:
1. Check the listener's health with a cheap read (a status call or a last-activity timestamp).
2. If healthy, do nothing and end silently. Do not post "all OK".
3. If unhealthy, attempt the documented restart once. Record the time in <STATE FILE>.
4. If the restart fails, report once to <MANAGER> with the error summary (no credentials), then stop. Do not retry in a loop.
End.
