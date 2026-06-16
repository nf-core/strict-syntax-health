# Workflow outputs migration: rangeland

- Generated: 2026-06-16T14:29:03.681554+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 12 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/rangeland/blob/941057f630e8c6555ebf79d164da7287eebcff46/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/rangeland/blob/941057f630e8c6555ebf79d164da7287eebcff46/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/rangeland/blob/941057f630e8c6555ebf79d164da7287eebcff46/conf/modules.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:41`](https://github.com/nf-core/rangeland/blob/941057f630e8c6555ebf79d164da7287eebcff46/conf/modules.config#L41)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:65`](https://github.com/nf-core/rangeland/blob/941057f630e8c6555ebf79d164da7287eebcff46/conf/modules.config#L65)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:85`](https://github.com/nf-core/rangeland/blob/941057f630e8c6555ebf79d164da7287eebcff46/conf/modules.config#L85)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:95`](https://github.com/nf-core/rangeland/blob/941057f630e8c6555ebf79d164da7287eebcff46/conf/modules.config#L95)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:104`](https://github.com/nf-core/rangeland/blob/941057f630e8c6555ebf79d164da7287eebcff46/conf/modules.config#L104)

  ```nextflow
  publishDir    = [
  ```

- [`conf/modules.config:110`](https://github.com/nf-core/rangeland/blob/941057f630e8c6555ebf79d164da7287eebcff46/conf/modules.config#L110)

  ```nextflow
  publishDir    = [
  ```

- [`conf/modules.config:117`](https://github.com/nf-core/rangeland/blob/941057f630e8c6555ebf79d164da7287eebcff46/conf/modules.config#L117)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:126`](https://github.com/nf-core/rangeland/blob/941057f630e8c6555ebf79d164da7287eebcff46/conf/modules.config#L126)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:75`](https://github.com/nf-core/rangeland/blob/941057f630e8c6555ebf79d164da7287eebcff46/nextflow.config#L75)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
