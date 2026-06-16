# Workflow outputs migration: datasync

- Generated: 2026-06-16T18:06:51.356263+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 3 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/datasync/blob/b02e7f6161ca62b7e27f3f3cc183414ea0959f36/conf/modules.config#L15) — 2 references
- [`nextflow.config`](https://github.com/nf-core/datasync/blob/b02e7f6161ca62b7e27f3f3cc183414ea0959f36/nextflow.config#L55) — 1 reference
