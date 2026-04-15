# RDL alert workflow

**Radboud Diagnostic Lab (RDL)** data are planned to follow a pattern **similar to CDL** (raw exports, linking file, processing into per-participant results and alert-style routing). Exact folder names, file formats, and clinical follow-up cadence should be aligned with the CDL workflow once RDL onboarding is complete.

## Intended shape (to confirm with the team)

1. Raw RDL exports and any **admin / linkage file** arrive on an agreed schedule and are placed under a defined path on Research Drive (TBD).
2. **Data team** runs agreed Python (or other) processing: raw → structured per-participant outputs, including any **normal / abnormal / alert** classification if applicable (TBD).
3. Clinical or study follow-up for flagged results follows the same governance as CDL (TBD: which roles, which weekdays).

## Handover notes

- Work plan: QC rules for RDL are to be written; treat this page as a **placeholder** until SOPs and paths are fixed.
- When live, mirror the evidence checklist used for CDL: sample raw file, processing script location, output layout, and archive rules.

## Related

- [CDL alert workflow](cdl-alert-workflow.md) — reference pattern
- [Multi-centre sample data workflow](multicentre-sample-data-workflow.md) — Radboud **RL** blood-tube file (separate from RDL diagnostic-lab alert exports)
