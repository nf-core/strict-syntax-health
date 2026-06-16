# Workflow outputs migration: alleleexpression

- Generated: 2026-06-16T14:07:44.783202+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 15 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:14`](https://github.com/nf-core/alleleexpression/blob/862bd3453274865736c12ccbb78bf7247827174e/conf/modules.config#L14)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:21`](https://github.com/nf-core/alleleexpression/blob/862bd3453274865736c12ccbb78bf7247827174e/conf/modules.config#L21)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:30`](https://github.com/nf-core/alleleexpression/blob/862bd3453274865736c12ccbb78bf7247827174e/conf/modules.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:38`](https://github.com/nf-core/alleleexpression/blob/862bd3453274865736c12ccbb78bf7247827174e/conf/modules.config#L38)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:46`](https://github.com/nf-core/alleleexpression/blob/862bd3453274865736c12ccbb78bf7247827174e/conf/modules.config#L46)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:54`](https://github.com/nf-core/alleleexpression/blob/862bd3453274865736c12ccbb78bf7247827174e/conf/modules.config#L54)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:64`](https://github.com/nf-core/alleleexpression/blob/862bd3453274865736c12ccbb78bf7247827174e/conf/modules.config#L64)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:73`](https://github.com/nf-core/alleleexpression/blob/862bd3453274865736c12ccbb78bf7247827174e/conf/modules.config#L73)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:81`](https://github.com/nf-core/alleleexpression/blob/862bd3453274865736c12ccbb78bf7247827174e/conf/modules.config#L81)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:90`](https://github.com/nf-core/alleleexpression/blob/862bd3453274865736c12ccbb78bf7247827174e/conf/modules.config#L90)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:98`](https://github.com/nf-core/alleleexpression/blob/862bd3453274865736c12ccbb78bf7247827174e/conf/modules.config#L98)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:106`](https://github.com/nf-core/alleleexpression/blob/862bd3453274865736c12ccbb78bf7247827174e/conf/modules.config#L106)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:114`](https://github.com/nf-core/alleleexpression/blob/862bd3453274865736c12ccbb78bf7247827174e/conf/modules.config#L114)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:122`](https://github.com/nf-core/alleleexpression/blob/862bd3453274865736c12ccbb78bf7247827174e/conf/modules.config#L122)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:131`](https://github.com/nf-core/alleleexpression/blob/862bd3453274865736c12ccbb78bf7247827174e/conf/modules.config#L131)

  ```nextflow
  publishDir = [
  ```
