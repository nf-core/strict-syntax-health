# Workflow outputs migration: isoseq

- Generated: 2026-06-16T14:20:02.670781+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 16 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:41`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/conf/modules.config#L41)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:49`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/conf/modules.config#L49)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:58`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/conf/modules.config#L58)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:67`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/conf/modules.config#L67)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:76`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/conf/modules.config#L76)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:85`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/conf/modules.config#L85)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:94`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/conf/modules.config#L94)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:102`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/conf/modules.config#L102)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:111`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/conf/modules.config#L111)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:123`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/conf/modules.config#L123)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:131`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/conf/modules.config#L131)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/isoseq/refine/tests/nextflow.config:3`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/modules/nf-core/isoseq/refine/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/lima/tests/nextflow.config:3`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/modules/nf-core/lima/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```
