# Workflow outputs migration: methylarray

- Generated: 2026-06-16T14:22:40.349072+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 2 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/methylarray/blob/eb5fb7db5015069030bc6c0cf0d2f0985b93cefb/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:27`](https://github.com/nf-core/methylarray/blob/eb5fb7db5015069030bc6c0cf0d2f0985b93cefb/conf/modules.config#L27)

  ```nextflow
  publishDir = [
  ```
