# Workflow outputs migration: deepmutscan

- Generated: 2026-06-16T20:21:06.656419+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 21 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L15) — 20 references
- [`modules/local/dmsanalysis/process_gatk/main.nf`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/modules/local/dmsanalysis/process_gatk/main.nf#L11) — 1 reference
