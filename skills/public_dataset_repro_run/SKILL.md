# Public dataset reproduction run

## Census every candidate before you select

- Run a full sweep of the source registry before you select any dataset, and search every synonym for the condition, including older names such as acne inversa for hidradenitis suppurativa.

- Write the frozen selection criteria down before you adjudicate any candidate.

- Adjudicate every candidate the sweep returns, and write the reason for every inclusion and every exclusion.

- Never drop a candidate silently, and never inherit a list without checking each entry against the sweep.

- Check identity down to sample level before you build a plan, and confirm each dataset actually holds the disease samples it claims.

- Treat a check that only verifies the included datasets as incomplete, and ask what the sweep may have missed.

## Validate every download before you merge

- Check gzip integrity for every downloaded file before you merge it, and compare its record count with the registry read count for the same run.

- Establish what the registry read count counts before you compare any file with it, and write the convention down for each registry and each segment.

- Accept a single file from a paired end run only when its count equals the registered count exactly or equals exactly half of it, because the ENA read count for a paired end ERR run is the total across both files while each file holds one half.

- Apply the halving acceptance only where the registry count is a total across files, and keep the plain equality check where the registry count already counts read pairs, as the SRR registry does.

- Stop and fix the validation rule before you retry when every run in a segment fails the count check in the same way, because a uniform failure across a whole segment points at the comparison rule rather than at the downloads.

- Retry a failed download up to four times before you declare it failed.

- Name every failed run in a written failure list, and never merge an HTML error page or a truncated file silently.

- Freeze the analysis parameters in writing before the run, including depth and random seed, and reuse them for any repair run.

- Compare the final run count with the frozen count before you run statistics, and stop when runs are missing.

## Guard the driver against empty and misquoted input

- Test the driver call form on a small case before the full run, and use the exact call form that passed.

- Add an empty data guard before any summary over a list that can be empty, so an empty input stops with a clear error instead of crashing mid run.

- Check the output directory names after the first run, and fix any quoting that turns a quote character into part of a name.

- Keep each shell step in plain shell form, and check that no argument is cut short by a special character.

## Segment long runs so a prune costs one segment

- Split a long run into one segment per dataset series, with a done marker and a local backup for each segment.

- Make the setup idempotent so a resumed segment does not redo finished work.

- Resume from the next unfinished segment after any interruption, and never restart a finished segment from scratch.

- Check progress every 30 minutes while a long run is going, and report a stall when nothing changes.

- When a hosted session is pruned twice before producing output, switch to segmented runs on a steadier machine instead of rebuilding the same session again.

## Available connectors

- Use `muse.connector_search` to find other connectors and `muse.skill_search` to find related skills.

- If nothing here fits, look on the web for a maintained API or MCP server and set it up with [Custom Connectors and MCPs](/opt/muse/skills/custom-connector-setup/SKILL.md), or build a custom connector.

## Websites

- [ENA portal API](https://www.ebi.ac.uk/ena/portal/api/filereport) for fetching registered run accessions and read counts. Carry the accession and the fields run_accession and read_count into the request and compare the returned set with the manuscript table run by run.

## Alternatives for better results

- Ask a checker who did not build the census to verify it independently before the analysis starts.

- Keep the raw downloads and the failure list beside the analysis so a later auditor can recount them.
