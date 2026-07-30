# Workflow outputs migration: longraredisease

- Generated: 2026-07-30T00:28:30.371621+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 76 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/longraredisease/blob/4f3fe625c53ee1ea6e00f0173fb09d00c0748932/conf/modules.config#L15) — 75 references
- [`subworkflows/local/call_sv/tests/nextflow.config`](https://github.com/nf-core/longraredisease/blob/4f3fe625c53ee1ea6e00f0173fb09d00c0748932/subworkflows/local/call_sv/tests/nextflow.config#L22) — 1 reference
