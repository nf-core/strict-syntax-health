# Workflow outputs migration: nanostring

- Generated: 2026-06-16T14:24:39.550296+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 7 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/nanostring/blob/915f51d2d8892f3c702cdc59e9ab997372375a40/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/nanostring/blob/915f51d2d8892f3c702cdc59e9ab997372375a40/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:30`](https://github.com/nf-core/nanostring/blob/915f51d2d8892f3c702cdc59e9ab997372375a40/conf/modules.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:39`](https://github.com/nf-core/nanostring/blob/915f51d2d8892f3c702cdc59e9ab997372375a40/conf/modules.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:47`](https://github.com/nf-core/nanostring/blob/915f51d2d8892f3c702cdc59e9ab997372375a40/conf/modules.config#L47)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:56`](https://github.com/nf-core/nanostring/blob/915f51d2d8892f3c702cdc59e9ab997372375a40/conf/modules.config#L56)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:66`](https://github.com/nf-core/nanostring/blob/915f51d2d8892f3c702cdc59e9ab997372375a40/conf/modules.config#L66)

  ```nextflow
  publishDir = [
  ```
