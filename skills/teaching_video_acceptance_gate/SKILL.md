# Teaching video acceptance gate

## Require a second independent literature check

- Treat the first literature check as provisional and never as final proof.

- Ask a checker who did not do the first check to verify every citation against its source.

- Remove every number and claim that has no source instead of softening its wording.

- Record every correction in a correction log kept beside the draft.

- Hold the draft from user review until the second check reports no unresolved citation.

## Reconcile frames before accepting a splice

- Sum the frame counts of every segment before accepting a finished video.

- Compare the delivered frame count with that sum and with the total duration multiplied by the frame rate.

- Reject any finished video whose frame count does not match even when its build tool exited without an error.

- Reencode from segment image sequences when a stream copy splice may carry nonmonotonic timestamps.

- Report the delivered frame count and the expected frame count together in the delivery receipt.

## Prescreen pronunciation before final audio

- Scan the script for characters with known homophone or tone confusion risk before recording final audio.

- Attach a pronunciation dictionary when the chosen voice service supports one.

- Test forced alignment scoring with a standard voice positive and negative control before trusting it on a cloned voice.

- List every character that the dictionary does not rescue as a top listen point for human review.

- Stop retakes after a small trial set for a resistant character and present an alternative take instead of recording without end.

## Report acceptance as a receipt

- Report the literature recheck result with the number of corrections made.

- Report the delivered frame count against the expected frame count.

- Report the pronunciation listen points that remain open.

- Send the draft to the user only after all three gates pass or the open items are named explicitly.

## Available connectors

- Use `muse.connector_search` to find other connectors and `muse.skill_search` to find related skills.

- If nothing here fits, look on the web for a maintained API or MCP server and set it up with [Custom Connectors and MCPs](/opt/muse/skills/custom-connector-setup/SKILL.md), or build a custom connector.

## Alternatives for better results

- Review keyframes for every demonstration segment before full rendering so geometry errors are caught before they reach this gate.

- Let the user decide each open pronunciation listen point instead of holding a finished draft for endless retakes.
