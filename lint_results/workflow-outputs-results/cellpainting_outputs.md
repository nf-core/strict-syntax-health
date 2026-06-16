# Workflow outputs migration: cellpainting

- Generated: 2026-06-16T14:10:18.233100+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 7 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/cellpainting/blob/eebfc70c4fc381335540854fefbc47c219cfa854/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/cellpainting/blob/eebfc70c4fc381335540854fefbc47c219cfa854/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:30`](https://github.com/nf-core/cellpainting/blob/eebfc70c4fc381335540854fefbc47c219cfa854/conf/modules.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:41`](https://github.com/nf-core/cellpainting/blob/eebfc70c4fc381335540854fefbc47c219cfa854/conf/modules.config#L41)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:49`](https://github.com/nf-core/cellpainting/blob/eebfc70c4fc381335540854fefbc47c219cfa854/conf/modules.config#L49)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:64`](https://github.com/nf-core/cellpainting/blob/eebfc70c4fc381335540854fefbc47c219cfa854/conf/modules.config#L64)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:73`](https://github.com/nf-core/cellpainting/blob/eebfc70c4fc381335540854fefbc47c219cfa854/conf/modules.config#L73)

  ```nextflow
  publishDir = [
  ```
