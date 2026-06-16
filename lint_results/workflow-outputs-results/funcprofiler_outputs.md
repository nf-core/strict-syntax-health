# Workflow outputs migration: funcprofiler

- Generated: 2026-06-16T14:17:05.006084+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 12 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/funcprofiler/blob/b0917e7ce4015dda9cf0f97487fa8ff421143ef9/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:26`](https://github.com/nf-core/funcprofiler/blob/b0917e7ce4015dda9cf0f97487fa8ff421143ef9/conf/modules.config#L26)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:44`](https://github.com/nf-core/funcprofiler/blob/b0917e7ce4015dda9cf0f97487fa8ff421143ef9/conf/modules.config#L44)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:51`](https://github.com/nf-core/funcprofiler/blob/b0917e7ce4015dda9cf0f97487fa8ff421143ef9/conf/modules.config#L51)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:60`](https://github.com/nf-core/funcprofiler/blob/b0917e7ce4015dda9cf0f97487fa8ff421143ef9/conf/modules.config#L60)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:67`](https://github.com/nf-core/funcprofiler/blob/b0917e7ce4015dda9cf0f97487fa8ff421143ef9/conf/modules.config#L67)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:75`](https://github.com/nf-core/funcprofiler/blob/b0917e7ce4015dda9cf0f97487fa8ff421143ef9/conf/modules.config#L75)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:83`](https://github.com/nf-core/funcprofiler/blob/b0917e7ce4015dda9cf0f97487fa8ff421143ef9/conf/modules.config#L83)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:77`](https://github.com/nf-core/funcprofiler/blob/b0917e7ce4015dda9cf0f97487fa8ff421143ef9/nextflow.config#L77)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```

- [`tests/nextflow.config:26`](https://github.com/nf-core/funcprofiler/blob/b0917e7ce4015dda9cf0f97487fa8ff421143ef9/tests/nextflow.config#L26)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:32`](https://github.com/nf-core/funcprofiler/blob/b0917e7ce4015dda9cf0f97487fa8ff421143ef9/tests/nextflow.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:40`](https://github.com/nf-core/funcprofiler/blob/b0917e7ce4015dda9cf0f97487fa8ff421143ef9/tests/nextflow.config#L40)

  ```nextflow
  publishDir = [
  ```
