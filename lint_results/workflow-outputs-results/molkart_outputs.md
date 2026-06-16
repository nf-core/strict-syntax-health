# Workflow outputs migration: molkart

- Generated: 2026-06-16T14:23:41.516243+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 18 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:39`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:52`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L52)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:65`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L65)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:79`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L79)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:91`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L91)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:101`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L101)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:111`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L111)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:120`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L120)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:129`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L129)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:145`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L145)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:154`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L154)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:184`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L184)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:199`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L199)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:219`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L219)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:228`](https://github.com/nf-core/molkart/blob/fdbb5802a4de87ada9c7aa4b85423726c461db41/conf/modules.config#L228)

  ```nextflow
  publishDir = [
  ```
