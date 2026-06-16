# Workflow outputs migration: funcprofiler

- Generated: 2026-06-16T19:25:57.639821+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 11 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/funcprofiler/blob/b0917e7ce4015dda9cf0f97487fa8ff421143ef9/conf/modules.config#L15) — 8 references
- [`tests/nextflow.config`](https://github.com/nf-core/funcprofiler/blob/b0917e7ce4015dda9cf0f97487fa8ff421143ef9/tests/nextflow.config#L26) — 3 references
