# Workflow outputs migration: genomeqc

- Generated: 2026-06-16T19:27:05.263256+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 37 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L15) — 36 references
- [`modules/local/tree_summary.nf`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/modules/local/tree_summary.nf#L6) — 1 reference
