# Workflow outputs migration: sopa

- Generated: 2026-06-16T14:35:53.278576+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 4 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:16`](https://github.com/nf-core/sopa/blob/60b77214078bcfa789cfe6cf84aecf914138e266/conf/modules.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/explorer/main.nf:10`](https://github.com/nf-core/sopa/blob/60b77214078bcfa789cfe6cf84aecf914138e266/modules/local/explorer/main.nf#L10)

  ```nextflow
  publishDir "${params.outdir}", mode: params.publish_dir_mode
  ```

- [`modules/local/explorer_raw/main.nf:12`](https://github.com/nf-core/sopa/blob/60b77214078bcfa789cfe6cf84aecf914138e266/modules/local/explorer_raw/main.nf#L12)

  ```nextflow
  publishDir "${params.outdir}", mode: params.publish_dir_mode
  ```

- [`modules/local/report/main.nf:10`](https://github.com/nf-core/sopa/blob/60b77214078bcfa789cfe6cf84aecf914138e266/modules/local/report/main.nf#L10)

  ```nextflow
  publishDir "${params.outdir}", mode: params.publish_dir_mode
  ```
