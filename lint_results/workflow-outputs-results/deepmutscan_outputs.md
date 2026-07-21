# Workflow outputs migration: deepmutscan

- Generated: 2026-07-21T00:29:05.791263+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 29 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/deepmutscan/blob/f3947ce4a5d57d31eeb865f802bc56ebcb675f6a/conf/modules.config#L18) — 28 references
- [`modules/local/dmsanalysis/process_variant_counts/main.nf`](https://github.com/nf-core/deepmutscan/blob/f3947ce4a5d57d31eeb865f802bc56ebcb675f6a/modules/local/dmsanalysis/process_variant_counts/main.nf#L11) — 1 reference
