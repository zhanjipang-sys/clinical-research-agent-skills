# Delegated work guardian

## Write a brief that requires a return report

- End every task brief with a requirement that the executor report back on completion with the deliverable paths, the acceptance points checked, and any blockers met.

- Treat a task with no return report as not delivered even when the work looks finished in a log.

- Name the deliverable files and the check that proves each one exists before you dispatch the work.

- Tell the executor to stop and report when it reaches a limit instead of substituting another executor or quietly continuing.

## Launch through a tracked route

- Start long work through the tracked background route in `muse.exec` so its completion returns to your context automatically.

- Launch long work only from the main chat through that tracked route, never from inside a cron or scheduled worker run.

- Do not start long work with nohup or disown and leave it detached with no return route.

- When a detached start is technically unavoidable, create a one off check with `cron.add` at the same moment so an expiry check still catches the result.

- Treat a `cron.add` check as a monitor only, never as the launch route for the long work itself, because the worker that runs the check ends and cleans up any child it spawned.

- Let a scheduled wake only check state and report back, and let the main chat re-dispatch the work when the wake finds work to resume.

- If a cron run reports the work is not finished after it spawned long work, treat that as this launch failure and re-dispatch from the main chat instead of retrying inside another cron run.

## Set an independent monitor at dispatch

- Create the monitor in the same turn you dispatch the work, never after the executor has already gone quiet.

- Give the monitor a periodic check with `cron.add` that reads the deliverable files and checks that the process is still alive.

- Judge progress by deliverable change such as a new file or a changed file time, never by a log line that only says the work started.

- Report only when the state changes, and stay silent while nothing has changed.

- Remove the monitor with `cron.remove` as soon as the deliverable closes.

## Check a suspected stall

- Treat about 30 minutes of silence with no deliverable change as a suspected stall.

- Check the work yourself at that point and report whether it is running, stalled, or recovered, without waiting for the user to ask.

- Check pending approval cards first, since a task can look idle while it waits for an approval that was never answered.

- Check quota, login state, and process survival next, and name the cause you found before you retry anything.

- Treat about 45 minutes with no deliverable change as possibly dead, and verify by a direct check of the files and the process rather than assuming the work is still running.

## Resume after a restart and close the loop

- After a machine restart, check whether the monitor and the work are still alive and restart the monitor when either one is gone.

- Resume the work from its last saved deliverable instead of starting over when the saved state is still valid.

- Deliver the result to the user as soon as it arrives, and do not wait for the user to ask for it.

- Report completion, failure, or a block in the same message as the evidence for that outcome.

## Available connectors

- Use `muse.connector_search` to find other connectors and `muse.skill_search` to find related skills.

- If nothing here fits, look on the web for a maintained API or MCP server and set it up with [Custom Connectors and MCPs](/opt/muse/skills/custom-connector-setup/SKILL.md), or build a custom connector.

## Alternatives for better results

- Split a long task into smaller deliverables so the monitor can see progress between checks.

- Ask the executor for a short progress note at each natural checkpoint instead of only at the end.