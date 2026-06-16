# Workflow outputs migration: diaproteomics

- Generated: 2026-06-16T14:14:04.747571+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 13 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`main.nf:323`](https://github.com/nf-core/diaproteomics/blob/92314aba5cc590906a4e4616be55781a1dd4d530/main.nf#L323)

  ```nextflow
  publishDir "${params.outdir}/pipeline_info", mode: params.publish_dir_mode,
  ```

- [`main.nf:460`](https://github.com/nf-core/diaproteomics/blob/92314aba5cc590906a4e4616be55781a1dd4d530/main.nf#L460)

  ```nextflow
  publishDir "${params.outdir}/spectral_library_files"
  ```

- [`main.nf:488`](https://github.com/nf-core/diaproteomics/blob/92314aba5cc590906a4e4616be55781a1dd4d530/main.nf#L488)

  ```nextflow
  publishDir "${params.outdir}/spectral_library_files"
  ```

- [`main.nf:521`](https://github.com/nf-core/diaproteomics/blob/92314aba5cc590906a4e4616be55781a1dd4d530/main.nf#L521)

  ```nextflow
  publishDir "${params.outdir}/spectral_library_files"
  ```

- [`main.nf:573`](https://github.com/nf-core/diaproteomics/blob/92314aba5cc590906a4e4616be55781a1dd4d530/main.nf#L573)

  ```nextflow
  publishDir "${params.outdir}/openswathworkflow_output"
  ```

- [`main.nf:747`](https://github.com/nf-core/diaproteomics/blob/92314aba5cc590906a4e4616be55781a1dd4d530/main.nf#L747)

  ```nextflow
  publishDir "${params.outdir}/pyprophet_output"
  ```

- [`main.nf:819`](https://github.com/nf-core/diaproteomics/blob/92314aba5cc590906a4e4616be55781a1dd4d530/main.nf#L819)

  ```nextflow
  publishDir "${params.outdir}/pyprophet_output"
  ```

- [`main.nf:890`](https://github.com/nf-core/diaproteomics/blob/92314aba5cc590906a4e4616be55781a1dd4d530/main.nf#L890)

  ```nextflow
  publishDir "${params.outdir}/"
  ```

- [`main.nf:930`](https://github.com/nf-core/diaproteomics/blob/92314aba5cc590906a4e4616be55781a1dd4d530/main.nf#L930)

  ```nextflow
  publishDir "${params.outdir}/"
  ```

- [`main.nf:980`](https://github.com/nf-core/diaproteomics/blob/92314aba5cc590906a4e4616be55781a1dd4d530/main.nf#L980)

  ```nextflow
  publishDir "${params.outdir}/"
  ```

- [`main.nf:1026`](https://github.com/nf-core/diaproteomics/blob/92314aba5cc590906a4e4616be55781a1dd4d530/main.nf#L1026)

  ```nextflow
  publishDir "${params.outdir}/"
  ```

- [`main.nf:1057`](https://github.com/nf-core/diaproteomics/blob/92314aba5cc590906a4e4616be55781a1dd4d530/main.nf#L1057)

  ```nextflow
  publishDir "${params.outdir}/"
  ```

- [`main.nf:1080`](https://github.com/nf-core/diaproteomics/blob/92314aba5cc590906a4e4616be55781a1dd4d530/main.nf#L1080)

  ```nextflow
  publishDir "${params.outdir}/pipeline_info", mode: params.publish_dir_mode
  ```
