# Workflow outputs migration: funcprofiler

- Generated: 2026-08-12T00:19:59.822730+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 11 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/funcprofiler/blob/c08987ad4017b08e7fd6f9b82f318d76dd41622e/conf/modules.config#L15) — 9 references
- [`tests/nextflow.config`](https://github.com/nf-core/funcprofiler/blob/c08987ad4017b08e7fd6f9b82f318d76dd41622e/tests/nextflow.config#L22) — 2 references
