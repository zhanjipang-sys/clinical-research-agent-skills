# Gemini Segmented Academic Dispatch

## Choose the channel first

- Route academic or long-form work that reconciles many files, tables or references to Gemini web Work or Task mode and deliver it in segments.

- Reserve Gemini web Chat for short single-source drafting, polishing and light revision, and never use a Chat one-shot draft as the basis for a multi-file academic model or manuscript.

- Use Antigravity only when the work needs heavy local resources such as large local files, code execution or batch processing, and state that reason before switching.

- Keep patient identifiable material and unpublished sensitive material out of any channel the user has not approved for that material.

## Roundtable borrowings (adopted 2026-11-24, from Li Jigang roundtable audit)

- Definition segment first: before any drafting or debate segment, run a standalone definition segment where each perspective independently defines the core concept and its core elements. Surface definition divergence explicitly; do not proceed until the working definition is settled or the divergence is recorded as a premise difference.
- Outsider seat: when a job uses multiple perspectives or reviewers, include at least one perspective from outside the topic's own field that can cover a blind-spot variable. Note what variable that seat owns.
- Deepest crack only: in synthesis and repair rounds, rank disagreements and advance only the single deepest contradiction first; derive the next segment or question from that crack instead of covering every issue at once. Park the rest in a visible list.

## Write one brief per segment

- Split the job into segments that each end in a checkable deliverable, such as one manuscript section, one chapter batch or one model stage.

- Give each segment brief the exact source files, tables and reference list it may use, and name anything outside that set as out of scope.

- Require the worker to mark every claim it cannot source with a pending check marker instead of filling the gap, and to report the sources it actually used.

- State the numbers, terms and conclusions already settled by earlier segments, so a later segment cannot quietly change them.

## Verify each segment before the next

- Check each returned segment item by item against its sources before dispatching the next segment, covering numbers, reference title author year alignment, and whether cited results say what the draft claims.

- Reject a segment that writes an unsourced effect, a quantitative prediction with no source, or a negative result as a positive one, and send only the failed items back for repair.

- Resolve every pending check marker yourself from the primary source or cut the claim, and record the resolution beside the segment.

- Never let the worker that wrote a segment be its only checker, and hold assembly until every segment has passed.

## Assemble and hand over

- Assemble the passed segments yourself and recheck cross-segment consistency, including reference numbering, totals repeated across sections, and terminology.

- Report the channel used, the segment pass results, and any claim you cut or softened for lack of source, so the user sees what verification changed.

- Stop before submission, external audit or sending whenever the user's chosen route requires a further independent check that has not happened yet.

## Available connectors

- [Google Gemini Free](~/workspace/custom-connectors/custom.google-gemini-free/CONNECTOR.md) for Gemini API access when a segment is small enough for API drafting.

- [Ncbi](~/workspace/custom-connectors/custom.ncbi/CONNECTOR.md) for verifying cited references against their source records during segment checks.

- Use `muse.connector_search` to find other connectors and `muse.skill_search` to find related skills.

- If nothing here fits, look on the web for a maintained API or MCP server and set it up with [Custom Connectors and MCPs](/opt/muse/skills/custom-connector-setup/SKILL.md), or build a custom connector.

## Websites

- [PubMed](https://pubmed.ncbi.nlm.nih.gov/) for verifying each cited reference during a segment check. Carry the PMID or DOI into `browser.browse` and verify the title, authors and year before accepting the citation.

## Alternatives for better results

- Run the manuscript number reconciliation skill on the assembled draft as a second gate when the work is number heavy.

- Run the AI revision anchor check skill when a passed segment later goes through revision, so settled content cannot drift back.

- Shrink a segment further when its check fails twice, because a smaller brief gives the worker fewer gaps to fill.
