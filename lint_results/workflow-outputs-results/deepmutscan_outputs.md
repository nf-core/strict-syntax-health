# Workflow outputs migration: deepmutscan

- Generated: 2026-07-16T00:27:52.333042+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 26 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/deepmutscan/blob/b890c1d91714cff1786c999d402d066060ac92ea/conf/modules.config#L18) — 25 references
- [`modules/local/dmsanalysis/process_variant_counts/main.nf`](https://github.com/nf-core/deepmutscan/blob/b890c1d91714cff1786c999d402d066060ac92ea/modules/local/dmsanalysis/process_variant_counts/main.nf#L11) — 1 reference
