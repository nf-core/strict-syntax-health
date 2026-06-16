# Workflow outputs migration: demo

- Generated: 2026-06-16T14:13:20.764549+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 4 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/demo/blob/ed969ce783288a37eb9e98c12aca38176e19a485/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/demo/blob/ed969ce783288a37eb9e98c12aca38176e19a485/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/demo/blob/ed969ce783288a37eb9e98c12aca38176e19a485/conf/modules.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:40`](https://github.com/nf-core/demo/blob/ed969ce783288a37eb9e98c12aca38176e19a485/conf/modules.config#L40)

  ```nextflow
  publishDir = [
  ```
