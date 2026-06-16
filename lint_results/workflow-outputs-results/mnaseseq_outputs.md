# Workflow outputs migration: mnaseseq

- Generated: 2026-06-16T14:23:34.901215+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 26 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`main.nf:279`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L279)

  ```nextflow
  publishDir "${params.outdir}/pipeline_info", mode: 'copy'
  ```

- [`main.nf:334`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L334)

  ```nextflow
  publishDir path: { params.save_reference ? "${params.outdir}/reference_genome" : params.outdir },
  ```

- [`main.nf:358`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L358)

  ```nextflow
  publishDir "${params.outdir}/reference_genome", mode: 'copy'
  ```

- [`main.nf:379`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L379)

  ```nextflow
  publishDir "${params.outdir}/reference_genome", mode: 'copy'
  ```

- [`main.nf:399`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L399)

  ```nextflow
  publishDir "${params.outdir}/reference_genome", mode: 'copy'
  ```

- [`main.nf:439`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L439)

  ```nextflow
  publishDir "${params.outdir}/fastqc", mode: 'copy',
  ```

- [`main.nf:489`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L489)

  ```nextflow
  publishDir "${params.outdir}/trim_galore", mode: 'copy',
  ```

- [`main.nf:584`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L584)

  ```nextflow
  publishDir path: "${params.outdir}/bwa/library", mode: 'copy',
  ```

- [`main.nf:631`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L631)

  ```nextflow
  publishDir "${params.outdir}/bwa/mergedLibrary", mode: 'copy',
  ```

- [`main.nf:708`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L708)

  ```nextflow
  publishDir path: "${params.outdir}/bwa/mergedLibrary", mode: 'copy',
  ```

- [`main.nf:782`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L782)

  ```nextflow
  publishDir path: "${params.outdir}/bwa/mergedLibrary", mode: 'copy',
  ```

- [`main.nf:833`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L833)

  ```nextflow
  publishDir "${params.outdir}/bwa/mergedLibrary/preseq", mode: 'copy'
  ```

- [`main.nf:857`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L857)

  ```nextflow
  publishDir path: "${params.outdir}/bwa/mergedLibrary", mode: 'copy',
  ```

- [`main.nf:899`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L899)

  ```nextflow
  publishDir path: "${params.outdir}/bwa/mergedLibrary", mode: 'copy',
  ```

- [`main.nf:941`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L941)

  ```nextflow
  publishDir "${params.outdir}/bwa/mergedLibrary/bigwig", mode: 'copy',
  ```

- [`main.nf:978`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L978)

  ```nextflow
  publishDir "${params.outdir}/bwa/mergedLibrary/deepTools/plotFingerprint", mode: 'copy'
  ```

- [`main.nf:1045`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L1045)

  ```nextflow
  publishDir "${params.outdir}/bwa/mergedLibrary/danpos", mode: 'copy',
  ```

- [`main.nf:1095`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L1095)

  ```nextflow
  publishDir "${params.outdir}/bwa/mergedLibrary/deepTools/plotProfile", mode: 'copy'
  ```

- [`main.nf:1149`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L1149)

  ```nextflow
  publishDir "${params.outdir}/bwa/mergedReplicate", mode: 'copy',
  ```

- [`main.nf:1258`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L1258)

  ```nextflow
  publishDir "${params.outdir}/bwa/mergedReplicate/bigwig", mode: 'copy',
  ```

- [`main.nf:1330`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L1330)

  ```nextflow
  publishDir "${params.outdir}/bwa/mergedReplicate/danpos", mode: 'copy',
  ```

- [`main.nf:1380`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L1380)

  ```nextflow
  publishDir "${params.outdir}/bwa/mergedReplicate/deepTools/plotProfile", mode: 'copy'
  ```

- [`main.nf:1426`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L1426)

  ```nextflow
  publishDir "${params.outdir}/igv", mode: 'copy'
  ```

- [`main.nf:1462`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L1462)

  ```nextflow
  publishDir "${params.outdir}/pipeline_info", mode: 'copy',
  ```

- [`main.nf:1513`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L1513)

  ```nextflow
  publishDir "${params.outdir}/multiqc", mode: 'copy'
  ```

- [`main.nf:1573`](https://github.com/nf-core/mnaseseq/blob/b7c0d8a13111bebc995186f3217bd7d1b768594f/main.nf#L1573)

  ```nextflow
  publishDir "${params.outdir}/Documentation", mode: 'copy'
  ```
