# Workflow outputs migration: provenancereport

- Generated: 2026-06-16T14:28:44.844569+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 2 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/provenancereport/blob/e858f86c3595ba490c60b36b8fe086ef676a8944/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:43`](https://github.com/nf-core/provenancereport/blob/e858f86c3595ba490c60b36b8fe086ef676a8944/nextflow.config#L43)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
