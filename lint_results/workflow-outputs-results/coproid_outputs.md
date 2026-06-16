# Workflow outputs migration: coproid

- Generated: 2026-06-16T14:11:20.260930+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 11 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/coproid/blob/1c63bc8fe75e3ee3c0b884e2bcb94d23dc3b281f/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:27`](https://github.com/nf-core/coproid/blob/1c63bc8fe75e3ee3c0b884e2bcb94d23dc3b281f/conf/modules.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:70`](https://github.com/nf-core/coproid/blob/1c63bc8fe75e3ee3c0b884e2bcb94d23dc3b281f/conf/modules.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:81`](https://github.com/nf-core/coproid/blob/1c63bc8fe75e3ee3c0b884e2bcb94d23dc3b281f/conf/modules.config#L81)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:90`](https://github.com/nf-core/coproid/blob/1c63bc8fe75e3ee3c0b884e2bcb94d23dc3b281f/conf/modules.config#L90)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:96`](https://github.com/nf-core/coproid/blob/1c63bc8fe75e3ee3c0b884e2bcb94d23dc3b281f/conf/modules.config#L96)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:103`](https://github.com/nf-core/coproid/blob/1c63bc8fe75e3ee3c0b884e2bcb94d23dc3b281f/conf/modules.config#L103)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:110`](https://github.com/nf-core/coproid/blob/1c63bc8fe75e3ee3c0b884e2bcb94d23dc3b281f/conf/modules.config#L110)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:116`](https://github.com/nf-core/coproid/blob/1c63bc8fe75e3ee3c0b884e2bcb94d23dc3b281f/conf/modules.config#L116)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:122`](https://github.com/nf-core/coproid/blob/1c63bc8fe75e3ee3c0b884e2bcb94d23dc3b281f/conf/modules.config#L122)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:128`](https://github.com/nf-core/coproid/blob/1c63bc8fe75e3ee3c0b884e2bcb94d23dc3b281f/conf/modules.config#L128)

  ```nextflow
  publishDir = [
  ```
