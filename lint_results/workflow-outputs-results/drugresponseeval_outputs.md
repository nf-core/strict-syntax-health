# Workflow outputs migration: drugresponseeval

- Generated: 2026-06-16T14:15:10.735864+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 27 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:30`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:38`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L38)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:46`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L46)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:54`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L54)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:62`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L62)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:70`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:78`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L78)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:86`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L86)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:94`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L94)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:102`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L102)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:111`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L111)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:131`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L131)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:139`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L139)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:158`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L158)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:166`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L166)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:186`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L186)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:206`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L206)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:214`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L214)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:222`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L222)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:241`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L241)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:249`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L249)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:257`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L257)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:266`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L266)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:274`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/conf/modules.config#L274)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:59`](https://github.com/nf-core/drugresponseeval/blob/233128a354a7832d5d2271a3a390c70d6677f45d/nextflow.config#L59)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
