# Workflow outputs migration: deepmutscan

- Generated: 2026-06-24T00:35:38.410749+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 21 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/deepmutscan/blob/afb29ea9bbfe38f7488e1e33f3159b7b559da7ba/conf/modules.config#L15) — 20 references
- [`modules/local/dmsanalysis/process_gatk/main.nf`](https://github.com/nf-core/deepmutscan/blob/afb29ea9bbfe38f7488e1e33f3159b7b559da7ba/modules/local/dmsanalysis/process_gatk/main.nf#L11) — 1 reference
