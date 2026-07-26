# Workflow outputs migration: deepmutscan

- Generated: 2026-07-26T00:32:32.795401+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 29 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/deepmutscan/blob/e53c89c3f3bcb0d6b1315d0daf8bc8a6ae5b88be/conf/modules.config#L18) — 28 references
- [`modules/local/dmsanalysis/process_variant_counts/main.nf`](https://github.com/nf-core/deepmutscan/blob/e53c89c3f3bcb0d6b1315d0daf8bc8a6ae5b88be/modules/local/dmsanalysis/process_variant_counts/main.nf#L11) — 1 reference
