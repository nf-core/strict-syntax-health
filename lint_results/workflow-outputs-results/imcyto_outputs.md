# Workflow outputs migration: imcyto

- Generated: 2026-06-16T14:19:56.343076+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 7 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/imcyto/blob/fac968e589a298cd5087cde684c46a1c1c292d0d/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/imcyto/blob/fac968e589a298cd5087cde684c46a1c1c292d0d/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:30`](https://github.com/nf-core/imcyto/blob/fac968e589a298cd5087cde684c46a1c1c292d0d/conf/modules.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:40`](https://github.com/nf-core/imcyto/blob/fac968e589a298cd5087cde684c46a1c1c292d0d/conf/modules.config#L40)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:50`](https://github.com/nf-core/imcyto/blob/fac968e589a298cd5087cde684c46a1c1c292d0d/conf/modules.config#L50)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:59`](https://github.com/nf-core/imcyto/blob/fac968e589a298cd5087cde684c46a1c1c292d0d/conf/modules.config#L59)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:69`](https://github.com/nf-core/imcyto/blob/fac968e589a298cd5087cde684c46a1c1c292d0d/conf/modules.config#L69)

  ```nextflow
  publishDir = [
  ```
