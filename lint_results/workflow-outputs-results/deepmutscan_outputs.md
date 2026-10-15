# Workflow outputs migration: deepmutscan

- Generated: 2026-10-15T00:19:16.947746+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 29 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/deepmutscan/blob/5da2094eb39f87eb82169f1eecdbb140951f87e4/conf/modules.config#L18) — 28 references
- [`modules/local/dmsanalysis/process_variant_counts/main.nf`](https://github.com/nf-core/deepmutscan/blob/5da2094eb39f87eb82169f1eecdbb140951f87e4/modules/local/dmsanalysis/process_variant_counts/main.nf#L11) — 1 reference
