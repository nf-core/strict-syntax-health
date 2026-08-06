# Workflow outputs migration: funcprofiler

- Generated: 2026-08-06T00:26:15.318408+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 11 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/funcprofiler/blob/8726325bba2f4c07182fc9b74d62b70491fb1baa/conf/modules.config#L15) — 9 references
- [`tests/nextflow.config`](https://github.com/nf-core/funcprofiler/blob/8726325bba2f4c07182fc9b74d62b70491fb1baa/tests/nextflow.config#L22) — 2 references
