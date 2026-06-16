# Workflow outputs migration: fastqrepair

- Generated: 2026-06-16T14:16:25.680046+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 6 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/fastqrepair/blob/7282b520275d81f6400b798059e6dea7621c1f1a/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/fastqrepair/blob/7282b520275d81f6400b798059e6dea7621c1f1a/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:51`](https://github.com/nf-core/fastqrepair/blob/7282b520275d81f6400b798059e6dea7621c1f1a/conf/modules.config#L51)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:73`](https://github.com/nf-core/fastqrepair/blob/7282b520275d81f6400b798059e6dea7621c1f1a/conf/modules.config#L73)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:96`](https://github.com/nf-core/fastqrepair/blob/7282b520275d81f6400b798059e6dea7621c1f1a/conf/modules.config#L96)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:105`](https://github.com/nf-core/fastqrepair/blob/7282b520275d81f6400b798059e6dea7621c1f1a/conf/modules.config#L105)

  ```nextflow
  publishDir = [
  ```
