# Workflow outputs migration: clipseq

- Generated: 2026-06-16T14:11:13.469392+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 24 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`main.nf:247`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L247)

  ```nextflow
  publishDir "${params.outdir}/pipeline_info", mode: params.publish_dir_mode,
  ```

- [`main.nf:408`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L408)

  ```nextflow
  publishDir path: { params.save_index ? "${params.outdir}/STAR_index" : params.outdir },
  ```

- [`main.nf:438`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L438)

  ```nextflow
  publishDir path: { params.save_index ? "${params.outdir}/STAR_index" : params.outdir },
  ```

- [`main.nf:478`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L478)

  ```nextflow
  publishDir "${params.outdir}/icount", mode: params.publish_dir_mode
  ```

- [`main.nf:509`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L509)

  ```nextflow
  publishDir "${params.outdir}/fastqc", mode: params.publish_dir_mode,
  ```

- [`main.nf:540`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L540)

  ```nextflow
  publishDir "${params.outdir}/umi", mode: params.publish_dir_mode,
  ```

- [`main.nf:570`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L570)

  ```nextflow
  publishDir "${params.outdir}/cutadapt", mode: params.publish_dir_mode
  ```

- [`main.nf:593`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L593)

  ```nextflow
  publishDir "${params.outdir}/premap", mode: params.publish_dir_mode
  ```

- [`main.nf:623`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L623)

  ```nextflow
  publishDir "${params.outdir}/mapped", mode: params.publish_dir_mode
  ```

- [`main.nf:665`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L665)

  ```nextflow
  publishDir "${params.outdir}/preseq", mode: params.publish_dir_mode
  ```

- [`main.nf:693`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L693)

  ```nextflow
  publishDir "${params.outdir}/dedup", mode: params.publish_dir_mode
  ```

- [`main.nf:733`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L733)

  ```nextflow
  publishDir "${params.outdir}/rseqc", mode: params.publish_dir_mode
  ```

- [`main.nf:762`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L762)

  ```nextflow
  publishDir "${params.outdir}/xlinks", mode: params.publish_dir_mode
  ```

- [`main.nf:791`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L791)

  ```nextflow
  publishDir "${params.outdir}/icount", mode: params.publish_dir_mode
  ```

- [`main.nf:822`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L822)

  ```nextflow
  publishDir "${params.outdir}/icount_motif", mode: params.publish_dir_mode
  ```

- [`main.nf:854`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L854)

  ```nextflow
  publishDir "${params.outdir}/paraclu", mode: params.publish_dir_mode
  ```

- [`main.nf:887`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L887)

  ```nextflow
  publishDir "${params.outdir}/paraclu_motif", mode: params.publish_dir_mode
  ```

- [`main.nf:922`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L922)

  ```nextflow
  publishDir "${params.outdir}/pureclip", mode: params.publish_dir_mode
  ```

- [`main.nf:959`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L959)

  ```nextflow
  publishDir "${params.outdir}/pureclip_motif", mode: params.publish_dir_mode
  ```

- [`main.nf:992`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L992)

  ```nextflow
  publishDir "${params.outdir}/piranha", mode: params.publish_dir_mode
  ```

- [`main.nf:1028`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L1028)

  ```nextflow
  publishDir "${params.outdir}/piranha_motif", mode: params.publish_dir_mode
  ```

- [`main.nf:1058`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L1058)

  ```nextflow
  publishDir "${params.outdir}/clipqc", mode: params.publish_dir_mode
  ```

- [`main.nf:1102`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L1102)

  ```nextflow
  publishDir "${params.outdir}/multiqc", mode: params.publish_dir_mode
  ```

- [`main.nf:1139`](https://github.com/nf-core/clipseq/blob/ed1f64863be8cf400b65ffc767ce1e90275c0cea/main.nf#L1139)

  ```nextflow
  publishDir "${params.outdir}/pipeline_info", mode: params.publish_dir_mode
  ```
