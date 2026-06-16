# Workflow outputs migration: nanoseq

- Generated: 2026-06-16T14:24:34.007177+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 3 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/nanoseq/blob/b175040bc1bb03d675c982e15668ee073f241933/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:27`](https://github.com/nf-core/nanoseq/blob/b175040bc1bb03d675c982e15668ee073f241933/conf/modules.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/subread/featurecounts/tests/nextflow.config:3`](https://github.com/nf-core/nanoseq/blob/b175040bc1bb03d675c982e15668ee073f241933/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```
