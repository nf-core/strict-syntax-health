# Workflow outputs migration: raredisease

- Generated: 2026-06-16T14:29:31.567837+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:782`](https://github.com/nf-core/raredisease/blob/560949bf362ad27bdf214459bf832c8163fa9936/main.nf#L782)

  ```nextflow
  output {
  ```

## Legacy `publishDir` references

Found 3 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/base.config:65`](https://github.com/nf-core/raredisease/blob/560949bf362ad27bdf214459bf832c8163fa9936/conf/base.config#L65)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/spring/decompress/tests/nextflow.config:3`](https://github.com/nf-core/raredisease/blob/560949bf362ad27bdf214459bf832c8163fa9936/modules/nf-core/spring/decompress/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`nextflow.config:192`](https://github.com/nf-core/raredisease/blob/560949bf362ad27bdf214459bf832c8163fa9936/nextflow.config#L192)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
