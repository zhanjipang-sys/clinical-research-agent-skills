# Clinical Research Agent Skills

A collection of agent skills distilled from a working clinical-research and surgical-education practice. Each skill is a reproducible playbook: it encodes not just steps, but the failure that taught the rule and the check that now prevents it.

The through-line is a first-principles + systems-thinking approach to clinical work, with a strict division of labour: AI agents execute and cross-check, the clinician keeps final medical judgement. No patient data appears anywhere in this repository — the research skills work on public datasets and de-identified manuscripts only.

## Skills

| Skill | What it does |
|---|---|
| `public_dataset_repro_run` | Reproducible analysis over public sequencing datasets: full census of candidate datasets, dataset-identity verification down to sample level before any run, validated downloads, segmented execution |
| `manuscript_number_reconciliation` | Reconciles every number in a research manuscript against its source tables before the draft goes to audit or submission |
| `gemini_segmented_academic_dispatch` | Routes multi-file academic writing to a large-context model in verified segments, so long-form drafts are source-checked segment by segment instead of accepted from a one-shot draft |
| `surgical_3d_keyframe_dispatch` | Dispatches surgical 3D keyframes from traced reference illustrations, with an operation-mechanics review before full rendering |
| `local-surgical-teaching-figures` | Builds interactive teaching figures for surgical concepts (layered, mechanism-first explanations) |
| `teaching_video_acceptance_gate` | Acceptance gate for medical teaching videos: independent citation checks and frame-level review before release |
| `delegated_work_guardian` | Keeps delegated background agent work from going silent by pairing each dispatch with an independent monitor that checks deliverables and reports stalls |

Each folder contains a `SKILL.md` (the playbook) and most include a `skill.yaml` descriptor, in the Agent Skills format used by Claude Code and compatible agents.

## Related

- [fact-check-gate](https://github.com/zhanjipang-sys/fact-check-gate) — the pre-publication fact-checking gate used by the same content workflow

## Author

Dr. Jipang Zhan — dermatologic surgery, Southern Medical University. Research focus: hidradenitis suppurativa, keloids, skin surgery education, and first-principles disease modelling.
