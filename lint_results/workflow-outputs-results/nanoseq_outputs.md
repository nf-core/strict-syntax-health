# Workflow outputs migration: nanoseq

- Generated: 2026-06-16T19:33:19.558029+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 3 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/nanoseq/blob/b175040bc1bb03d675c982e15668ee073f241933/conf/modules.config#L15) — 2 references
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/nanoseq/blob/b175040bc1bb03d675c982e15668ee073f241933/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
