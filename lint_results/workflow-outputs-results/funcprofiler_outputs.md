# Workflow outputs migration: funcprofiler

- Generated: 2026-07-31T00:31:21.241983+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 10 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/funcprofiler/blob/9acfccad2aaf9e9d7272a1518730c4c623b2c4fa/conf/modules.config#L15) — 8 references
- [`tests/nextflow.config`](https://github.com/nf-core/funcprofiler/blob/9acfccad2aaf9e9d7272a1518730c4c623b2c4fa/tests/nextflow.config#L24) — 2 references
