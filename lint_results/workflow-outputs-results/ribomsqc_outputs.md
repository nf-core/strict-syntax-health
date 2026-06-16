# Workflow outputs migration: ribomsqc

- Generated: 2026-06-16T14:30:30.231960+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 1 `publishDir` reference that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/ribomsqc/blob/8a0e1ed486cbeade43845c428c9ef939bd0379a9/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```
