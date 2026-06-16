# Workflow outputs migration: dartseq

- Generated: 2026-06-16T14:12:33.678504+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 14 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/dartseq/blob/8c0d918bfb4b770e1b717e17459595cd9805aa38/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:40`](https://github.com/nf-core/dartseq/blob/8c0d918bfb4b770e1b717e17459595cd9805aa38/conf/modules.config#L40)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:63`](https://github.com/nf-core/dartseq/blob/8c0d918bfb4b770e1b717e17459595cd9805aa38/conf/modules.config#L63)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:72`](https://github.com/nf-core/dartseq/blob/8c0d918bfb4b770e1b717e17459595cd9805aa38/conf/modules.config#L72)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:80`](https://github.com/nf-core/dartseq/blob/8c0d918bfb4b770e1b717e17459595cd9805aa38/conf/modules.config#L80)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:88`](https://github.com/nf-core/dartseq/blob/8c0d918bfb4b770e1b717e17459595cd9805aa38/conf/modules.config#L88)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:96`](https://github.com/nf-core/dartseq/blob/8c0d918bfb4b770e1b717e17459595cd9805aa38/conf/modules.config#L96)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:104`](https://github.com/nf-core/dartseq/blob/8c0d918bfb4b770e1b717e17459595cd9805aa38/conf/modules.config#L104)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:112`](https://github.com/nf-core/dartseq/blob/8c0d918bfb4b770e1b717e17459595cd9805aa38/conf/modules.config#L112)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:120`](https://github.com/nf-core/dartseq/blob/8c0d918bfb4b770e1b717e17459595cd9805aa38/conf/modules.config#L120)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:128`](https://github.com/nf-core/dartseq/blob/8c0d918bfb4b770e1b717e17459595cd9805aa38/conf/modules.config#L128)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:136`](https://github.com/nf-core/dartseq/blob/8c0d918bfb4b770e1b717e17459595cd9805aa38/conf/modules.config#L136)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:144`](https://github.com/nf-core/dartseq/blob/8c0d918bfb4b770e1b717e17459595cd9805aa38/conf/modules.config#L144)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:153`](https://github.com/nf-core/dartseq/blob/8c0d918bfb4b770e1b717e17459595cd9805aa38/conf/modules.config#L153)

  ```nextflow
  publishDir = [
  ```
