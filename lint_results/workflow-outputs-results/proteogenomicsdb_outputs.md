# Workflow outputs migration: proteogenomicsdb

- Generated: 2026-06-16T14:28:40.055798+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 5 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`main.nf:127`](https://github.com/nf-core/proteogenomicsdb/blob/e700d967253c5c80985fdcdc48e482dace2bb2d0/main.nf#L127)

  ```nextflow
  publishDir "${params.outdir}/pipeline_info", mode: params.publish_dir_mode,
  ```

- [`main.nf:736`](https://github.com/nf-core/proteogenomicsdb/blob/e700d967253c5c80985fdcdc48e482dace2bb2d0/main.nf#L736)

  ```nextflow
  publishDir "${params.outdir}/", mode: params.publish_dir_mode,
  ```

- [`main.nf:759`](https://github.com/nf-core/proteogenomicsdb/blob/e700d967253c5c80985fdcdc48e482dace2bb2d0/main.nf#L759)

  ```nextflow
  publishDir "${params.outdir}/", mode: params.publish_dir_mode,
  ```

- [`main.nf:799`](https://github.com/nf-core/proteogenomicsdb/blob/e700d967253c5c80985fdcdc48e482dace2bb2d0/main.nf#L799)

  ```nextflow
  publishDir "${params.outdir}/", mode: params.publish_dir_mode,
  ```

- [`main.nf:830`](https://github.com/nf-core/proteogenomicsdb/blob/e700d967253c5c80985fdcdc48e482dace2bb2d0/main.nf#L830)

  ```nextflow
  publishDir "${params.outdir}/pipeline_info", mode: params.publish_dir_mode
  ```
