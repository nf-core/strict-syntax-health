# Workflow outputs migration: spinningjenny

- Generated: 2026-06-16T14:36:32.085644+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 6 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/spinningjenny/blob/9bb174383c4abda8f432548a34d69cb7f587bb4c/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/spinningjenny/blob/9bb174383c4abda8f432548a34d69cb7f587bb4c/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/spinningjenny/blob/9bb174383c4abda8f432548a34d69cb7f587bb4c/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:41`](https://github.com/nf-core/spinningjenny/blob/9bb174383c4abda8f432548a34d69cb7f587bb4c/conf/modules.config#L41)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:50`](https://github.com/nf-core/spinningjenny/blob/9bb174383c4abda8f432548a34d69cb7f587bb4c/conf/modules.config#L50)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:65`](https://github.com/nf-core/spinningjenny/blob/9bb174383c4abda8f432548a34d69cb7f587bb4c/nextflow.config#L65)

  ```nextflow
  publishDir = [
  ```
