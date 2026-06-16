# Workflow outputs migration: proteinannotator

- Generated: 2026-06-16T14:27:47.307198+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 20 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:48`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:60`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L60)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:70`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:78`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L78)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:86`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L86)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:94`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L94)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:102`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L102)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:111`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L111)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:121`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L121)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:131`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L131)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:141`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L141)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:150`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L150)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:158`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L158)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:166`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L166)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:181`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L181)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:190`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/conf/modules.config#L190)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:82`](https://github.com/nf-core/proteinannotator/blob/6bcb8b0e40b8368e864d929cde63aa446020ee62/nextflow.config#L82)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
