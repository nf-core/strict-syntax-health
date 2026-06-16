# Workflow outputs migration: demultiplex

- Generated: 2026-06-16T14:13:36.089305+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:128`](https://github.com/nf-core/demultiplex/blob/257df49988d242fabb42b6d87fb1e3a69c39789f/main.nf#L128)

  ```nextflow
  output {
  ```

## Legacy `publishDir` references

Found 6 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/test.config:38`](https://github.com/nf-core/demultiplex/blob/257df49988d242fabb42b6d87fb1e3a69c39789f/conf/test.config#L38)

  ```nextflow
  publishDir = [
  ```

- [`conf/test.config:66`](https://github.com/nf-core/demultiplex/blob/257df49988d242fabb42b6d87fb1e3a69c39789f/conf/test.config#L66)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_flowcell.config:39`](https://github.com/nf-core/demultiplex/blob/257df49988d242fabb42b6d87fb1e3a69c39789f/conf/test_flowcell.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_uncompressed.config:39`](https://github.com/nf-core/demultiplex/blob/257df49988d242fabb42b6d87fb1e3a69c39789f/conf/test_uncompressed.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_uncompressed.config:65`](https://github.com/nf-core/demultiplex/blob/257df49988d242fabb42b6d87fb1e3a69c39789f/conf/test_uncompressed.config#L65)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/bcl2fastq/tests/nextflow.config:3`](https://github.com/nf-core/demultiplex/blob/257df49988d242fabb42b6d87fb1e3a69c39789f/modules/nf-core/bcl2fastq/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```
