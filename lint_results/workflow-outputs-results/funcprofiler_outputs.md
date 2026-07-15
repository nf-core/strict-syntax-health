# Workflow outputs migration: funcprofiler

- Generated: 2026-07-15T00:24:17.074777+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 10 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/funcprofiler/blob/a0d2bf94826ad7de416a42071e3315c37cb8dee1/conf/modules.config#L15) — 8 references
- [`tests/nextflow.config`](https://github.com/nf-core/funcprofiler/blob/a0d2bf94826ad7de416a42071e3315c37cb8dee1/tests/nextflow.config#L26) — 2 references
