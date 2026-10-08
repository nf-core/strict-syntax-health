# Workflow outputs migration: spinningjenny

- Generated: 2026-10-08T00:34:01.910109+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 6 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/spinningjenny/blob/d41309a18020121ad1a0130a03eb5a6822b8a41c/conf/modules.config#L15) — 5 references
- [`nextflow.config`](https://github.com/nf-core/spinningjenny/blob/d41309a18020121ad1a0130a03eb5a6822b8a41c/nextflow.config#L65) — 1 reference
