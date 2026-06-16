# Workflow outputs migration: slamseq

- Generated: 2026-06-16T14:35:27.952013+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 8 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`main.nf:286`](https://github.com/nf-core/slamseq/blob/c21d0faee30707ffe134f77e0b37887a1610503f/main.nf#L286)

  ```nextflow
  publishDir "${params.outdir}/pipeline_info", mode: 'copy',
  ```

- [`main.nf:422`](https://github.com/nf-core/slamseq/blob/c21d0faee30707ffe134f77e0b37887a1610503f/main.nf#L422)

  ```nextflow
  publishDir path: "${params.outdir}/slamdunk/bam", mode: 'copy',
  ```

- [`main.nf:454`](https://github.com/nf-core/slamseq/blob/c21d0faee30707ffe134f77e0b37887a1610503f/main.nf#L454)

  ```nextflow
  publishDir path: "${params.outdir}/slamdunk/vcf", mode: 'copy',
  ```

- [`main.nf:498`](https://github.com/nf-core/slamseq/blob/c21d0faee30707ffe134f77e0b37887a1610503f/main.nf#L498)

  ```nextflow
  publishDir path: "${params.outdir}/slamdunk/count/utrs", mode: 'copy',
  ```

- [`main.nf:536`](https://github.com/nf-core/slamseq/blob/c21d0faee30707ffe134f77e0b37887a1610503f/main.nf#L536)

  ```nextflow
  publishDir path: "${params.outdir}/slamdunk/count/genes", mode: 'copy',
  ```

- [`main.nf:730`](https://github.com/nf-core/slamseq/blob/c21d0faee30707ffe134f77e0b37887a1610503f/main.nf#L730)

  ```nextflow
  publishDir path: "${params.outdir}/deseq2", mode: 'copy', overwrite: 'true'
  ```

- [`main.nf:752`](https://github.com/nf-core/slamseq/blob/c21d0faee30707ffe134f77e0b37887a1610503f/main.nf#L752)

  ```nextflow
  publishDir "${params.outdir}/multiqc", mode: 'copy'
  ```

- [`main.nf:785`](https://github.com/nf-core/slamseq/blob/c21d0faee30707ffe134f77e0b37887a1610503f/main.nf#L785)

  ```nextflow
  publishDir "${params.outdir}/pipeline_info", mode: 'copy'
  ```
