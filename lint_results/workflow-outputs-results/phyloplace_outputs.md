# Workflow outputs migration: phyloplace

- Generated: 2026-06-16T14:27:18.309874+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 3 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/phyloplace/blob/1bb88024c934e0bbcf25c58dcf96c6eeb6ff045e/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:90`](https://github.com/nf-core/phyloplace/blob/1bb88024c934e0bbcf25c58dcf96c6eeb6ff045e/conf/modules.config#L90)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:59`](https://github.com/nf-core/phyloplace/blob/1bb88024c934e0bbcf25c58dcf96c6eeb6ff045e/nextflow.config#L59)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
