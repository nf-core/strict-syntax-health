# Workflow outputs migration: funcprofiler

- Generated: 2026-08-01T00:30:02.623103+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 11 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/funcprofiler/blob/4d53c0cde8960ab3b73734d6423c210c9e20411c/conf/modules.config#L15) — 9 references
- [`tests/nextflow.config`](https://github.com/nf-core/funcprofiler/blob/4d53c0cde8960ab3b73734d6423c210c9e20411c/tests/nextflow.config#L24) — 2 references
