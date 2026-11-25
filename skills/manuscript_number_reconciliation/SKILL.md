# Manuscript number reconciliation

## Extract every number into one table

- List every number that appears in the abstract, the main text, every table, every figure legend, the submission note, and the cover letter.

- Give each row the value, each place it appears, the source table or dataset behind it, and the calculation that produced it.

- Add word counts to the table as numbers, including the abstract count, the stated limit, and any count repeated in the cover letter or submission note.

- Add every total to the table, including sample counts, series counts, and run counts, with the source rows that sum to each total.

- Freeze the source tables before you extract numbers so a late data change cannot silently invalidate the table.

## Check every occurrence against its source

- Compare each value in the table with each place it appears and correct every mismatch before the draft moves on.

- Check that subgroup counts sum to each total they belong to and that every listed series is counted once in the series total.

- Flag any total that has no source row behind it and either find its source or cut it from the draft.

- Verify each cited reference against its source record and correct any mismatched author, title, or identifier.

- Compare each interpretive claim with the source support behind it and soften or cut wording that claims more than the source shows.

## Verify each reference in more than one database

- Search at least two domestic Chinese bibliographic databases before you mark a Chinese language reference as not found, and record the databases you searched beside the verdict in the reconciliation table.

- Leave a reference marked unverified while only one database has been searched or the searches disagree, and never report unverified as not found.

- Record one verdict for every reference, chosen from verified, bibliographic error, not found, and unverified, so an auditor can recount each category.

## Hold the draft until the table balances

- Treat the table as incomplete while any row has a mismatch, a missing source, or an open method detail.

- List every missing method detail as an open item, including the pairing method, trimming parameters, and the sample unit for each dataset.

- Send the draft to audit only after every row balances and every open item is resolved or named explicitly.

- Return the draft to reconciliation when any auditor reports a FAIL and repeat the full check before the next audit round.

- Send the reconciled table with the draft so auditors check the table instead of extracting the numbers again.

- Include the manuscript tables themselves in any package you send to a blind or independent auditor, because an auditor cannot reconcile a number that lives in a table the package omits.

## Available connectors

- Use `muse.connector_search` to find other connectors and `muse.skill_search` to find related skills.

- If nothing here fits, look on the web for a maintained API or MCP server and set it up with [Custom Connectors and MCPs](/opt/muse/skills/custom-connector-setup/SKILL.md), or build a custom connector.

## Websites

- [PubMed](https://pubmed.ncbi.nlm.nih.gov/) for verifying each cited reference against its source record. Carry the PMID or DOI into the search and verify the title, authors, and journal before accepting the citation.

## Alternatives for better results

- Ask a checker who did not build the table to verify it independently before the draft goes to audit.

- Treat an anchor list from a revision check as an input to this table, not as a substitute for extracting every number.

- Split a long manuscript by section and reconcile each section separately when one table grows too large to check in one pass.
