# Workflow outputs migration: omicsgenetraitassociation

- Generated: 2026-06-16T14:25:13.803366+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 12 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/cma_mea.config:32`](https://github.com/nf-core/omicsgenetraitassociation/blob/f64a3c7867ffe159a0f347d3b07d11c99ade49fb/conf/cma_mea.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:15`](https://github.com/nf-core/omicsgenetraitassociation/blob/f64a3c7867ffe159a0f347d3b07d11c99ade49fb/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/omicsgenetraitassociation/blob/f64a3c7867ffe159a0f347d3b07d11c99ade49fb/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:30`](https://github.com/nf-core/omicsgenetraitassociation/blob/f64a3c7867ffe159a0f347d3b07d11c99ade49fb/conf/modules.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:38`](https://github.com/nf-core/omicsgenetraitassociation/blob/f64a3c7867ffe159a0f347d3b07d11c99ade49fb/conf/modules.config#L38)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:46`](https://github.com/nf-core/omicsgenetraitassociation/blob/f64a3c7867ffe159a0f347d3b07d11c99ade49fb/conf/modules.config#L46)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:59`](https://github.com/nf-core/omicsgenetraitassociation/blob/f64a3c7867ffe159a0f347d3b07d11c99ade49fb/conf/modules.config#L59)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:72`](https://github.com/nf-core/omicsgenetraitassociation/blob/f64a3c7867ffe159a0f347d3b07d11c99ade49fb/conf/modules.config#L72)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:85`](https://github.com/nf-core/omicsgenetraitassociation/blob/f64a3c7867ffe159a0f347d3b07d11c99ade49fb/conf/modules.config#L85)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:98`](https://github.com/nf-core/omicsgenetraitassociation/blob/f64a3c7867ffe159a0f347d3b07d11c99ade49fb/conf/modules.config#L98)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_local.config:53`](https://github.com/nf-core/omicsgenetraitassociation/blob/f64a3c7867ffe159a0f347d3b07d11c99ade49fb/conf/test_local.config#L53)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/pascal/main.nf:6`](https://github.com/nf-core/omicsgenetraitassociation/blob/f64a3c7867ffe159a0f347d3b07d11c99ade49fb/modules/local/pascal/main.nf#L6)

  ```nextflow
  // publishDir "results/pascal", mode:'copy', saveAs: { filename  -> filename.endsWith(".csv") ? "PASCAL.csv" : filename}
  ```
