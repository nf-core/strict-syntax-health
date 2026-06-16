# Workflow outputs migration: epigenomesegmentation

- Generated: 2026-06-16T14:15:46.478272+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 15 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/epigenomesegmentation/blob/3b57d5ad96536a6b2e6e331e246d94ba1b8395e9/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:24`](https://github.com/nf-core/epigenomesegmentation/blob/3b57d5ad96536a6b2e6e331e246d94ba1b8395e9/conf/modules.config#L24)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/epigenomesegmentation/blob/3b57d5ad96536a6b2e6e331e246d94ba1b8395e9/conf/modules.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:40`](https://github.com/nf-core/epigenomesegmentation/blob/3b57d5ad96536a6b2e6e331e246d94ba1b8395e9/conf/modules.config#L40)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:48`](https://github.com/nf-core/epigenomesegmentation/blob/3b57d5ad96536a6b2e6e331e246d94ba1b8395e9/conf/modules.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:56`](https://github.com/nf-core/epigenomesegmentation/blob/3b57d5ad96536a6b2e6e331e246d94ba1b8395e9/conf/modules.config#L56)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:63`](https://github.com/nf-core/epigenomesegmentation/blob/3b57d5ad96536a6b2e6e331e246d94ba1b8395e9/conf/modules.config#L63)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:72`](https://github.com/nf-core/epigenomesegmentation/blob/3b57d5ad96536a6b2e6e331e246d94ba1b8395e9/conf/modules.config#L72)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:80`](https://github.com/nf-core/epigenomesegmentation/blob/3b57d5ad96536a6b2e6e331e246d94ba1b8395e9/conf/modules.config#L80)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:87`](https://github.com/nf-core/epigenomesegmentation/blob/3b57d5ad96536a6b2e6e331e246d94ba1b8395e9/conf/modules.config#L87)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:96`](https://github.com/nf-core/epigenomesegmentation/blob/3b57d5ad96536a6b2e6e331e246d94ba1b8395e9/conf/modules.config#L96)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:104`](https://github.com/nf-core/epigenomesegmentation/blob/3b57d5ad96536a6b2e6e331e246d94ba1b8395e9/conf/modules.config#L104)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:112`](https://github.com/nf-core/epigenomesegmentation/blob/3b57d5ad96536a6b2e6e331e246d94ba1b8395e9/conf/modules.config#L112)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:121`](https://github.com/nf-core/epigenomesegmentation/blob/3b57d5ad96536a6b2e6e331e246d94ba1b8395e9/conf/modules.config#L121)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:131`](https://github.com/nf-core/epigenomesegmentation/blob/3b57d5ad96536a6b2e6e331e246d94ba1b8395e9/conf/modules.config#L131)

  ```nextflow
  publishDir = [
  ```
