# Workflow outputs migration: datasync

- Generated: 2026-06-16T14:12:47.383515+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 3 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/datasync/blob/3addfb1c2fad86c6bccbbb654fe42f9f1412302b/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:27`](https://github.com/nf-core/datasync/blob/3addfb1c2fad86c6bccbbb654fe42f9f1412302b/conf/modules.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:55`](https://github.com/nf-core/datasync/blob/3addfb1c2fad86c6bccbbb654fe42f9f1412302b/nextflow.config#L55)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
