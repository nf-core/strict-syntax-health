# Workflow outputs migration: evexplorer

- Generated: 2026-06-16T14:16:19.360742+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 9 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/evexplorer/blob/f446969e762a9f7398842d38952207e71991aaad/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:24`](https://github.com/nf-core/evexplorer/blob/f446969e762a9f7398842d38952207e71991aaad/conf/modules.config#L24)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:34`](https://github.com/nf-core/evexplorer/blob/f446969e762a9f7398842d38952207e71991aaad/conf/modules.config#L34)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:45`](https://github.com/nf-core/evexplorer/blob/f446969e762a9f7398842d38952207e71991aaad/conf/modules.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:62`](https://github.com/nf-core/evexplorer/blob/f446969e762a9f7398842d38952207e71991aaad/conf/modules.config#L62)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:75`](https://github.com/nf-core/evexplorer/blob/f446969e762a9f7398842d38952207e71991aaad/conf/modules.config#L75)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:84`](https://github.com/nf-core/evexplorer/blob/f446969e762a9f7398842d38952207e71991aaad/conf/modules.config#L84)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:93`](https://github.com/nf-core/evexplorer/blob/f446969e762a9f7398842d38952207e71991aaad/conf/modules.config#L93)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:103`](https://github.com/nf-core/evexplorer/blob/f446969e762a9f7398842d38952207e71991aaad/conf/modules.config#L103)

  ```nextflow
  publishDir = [
  ```
