# Workflow outputs migration: marsseq

- Generated: 2026-06-16T14:21:50.824884+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 23 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:24`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L24)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:40`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L40)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:48`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:55`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L55)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:61`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L61)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:68`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L68)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:76`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L76)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:84`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L84)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:93`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L93)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:99`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L99)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:107`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L107)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:114`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L114)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:120`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L120)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:127`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L127)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:136`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L136)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:145`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L145)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:154`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L154)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:166`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L166)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:172`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L172)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:181`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L181)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:190`](https://github.com/nf-core/marsseq/blob/c9a702eb7f4b8d25a6fe7a115078dd3ac211f346/conf/modules.config#L190)

  ```nextflow
  publishDir = [
  ```
