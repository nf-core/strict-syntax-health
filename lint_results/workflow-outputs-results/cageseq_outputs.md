# Workflow outputs migration: cageseq

- Generated: 2026-06-16T14:09:55.310903+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 31 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:39`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:47`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L47)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:55`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L55)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:63`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L63)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:70`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:79`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L79)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:98`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L98)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:105`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L105)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:113`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L113)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:122`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L122)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:131`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L131)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:138`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L138)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:145`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L145)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:154`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L154)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:163`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L163)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:170`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L170)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:177`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L177)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:184`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L184)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:192`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L192)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:200`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L200)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:207`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L207)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:214`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L214)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:221`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L221)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:228`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L228)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:235`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L235)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:242`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L242)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:249`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/conf/modules.config#L249)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:105`](https://github.com/nf-core/cageseq/blob/b4ab44cf1e93c81f5899b12e95dda7c4428f5ca2/nextflow.config#L105)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
