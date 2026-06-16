# Workflow outputs migration: lncpipe

- Generated: 2026-06-16T14:20:25.727258+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 39 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:26`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/conf/modules.config#L26)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:35`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/conf/modules.config#L35)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:43`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/conf/modules.config#L43)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/subread/featurecounts/tests/nextflow.config:3`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/umitools/extract/tests/nextflow.config:3`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/modules/nf-core/umitools/extract/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`subworkflows/local/prepare_genome/nextflow.config:3`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/local/prepare_genome/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/prepare_genome/nextflow.config:15`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/local/prepare_genome/nextflow.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/prepare_genome/nextflow.config:24`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/local/prepare_genome/nextflow.config#L24)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/prepare_genome/nextflow.config:32`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/local/prepare_genome/nextflow.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/prepare_genome/nextflow.config:44`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/local/prepare_genome/nextflow.config#L44)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/prepare_genome/nextflow.config:53`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/local/prepare_genome/nextflow.config#L53)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/prepare_genome/nextflow.config:62`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/local/prepare_genome/nextflow.config#L62)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/prepare_genome/nextflow.config:70`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/local/prepare_genome/nextflow.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/prepare_genome/nextflow.config:78`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/local/prepare_genome/nextflow.config#L78)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/prepare_genome/nextflow.config:87`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/local/prepare_genome/nextflow.config#L87)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/prepare_genome/nextflow.config:95`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/local/prepare_genome/nextflow.config#L95)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/prepare_genome/nextflow.config:107`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/local/prepare_genome/nextflow.config#L107)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/prepare_genome/nextflow.config:120`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/local/prepare_genome/nextflow.config#L120)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/stringtie/nextflow.config:3`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/local/stringtie/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_align_star/nextflow.config:26`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_align_star/nextflow.config#L26)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_align_star/tests/nextflow.config:3`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_align_star/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config:3`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`subworkflows/nf-core/fastq_fastqc_umitools_fastp/nextflow.config:7`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_fastqc_umitools_fastp/nextflow.config#L7)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_fastqc_umitools_fastp/nextflow.config:17`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_fastqc_umitools_fastp/nextflow.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_fastqc_umitools_fastp/nextflow.config:32`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_fastqc_umitools_fastp/nextflow.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_fastqc_umitools_fastp/nextflow.config:64`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_fastqc_umitools_fastp/nextflow.config#L64)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_fastqc_umitools_trimgalore/nextflow.config:7`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_fastqc_umitools_trimgalore/nextflow.config#L7)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_fastqc_umitools_trimgalore/nextflow.config:42`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_fastqc_umitools_trimgalore/nextflow.config#L42)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_fastqc_umitools_trimgalore/nextflow.config:74`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_fastqc_umitools_trimgalore/nextflow.config#L74)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/nextflow.config:5`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/nextflow.config#L5)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/nextflow.config:13`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/nextflow.config#L13)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/nextflow.config:21`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/nextflow.config#L21)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/nextflow.config:29`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/nextflow.config#L29)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config:22`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config:29`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config#L29)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_subsample_fq_salmon/nextflow.config:5`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_subsample_fq_salmon/nextflow.config#L5)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_subsample_fq_salmon/nextflow.config:12`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_subsample_fq_salmon/nextflow.config#L12)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_subsample_fq_salmon/tests/nextflow.config:3`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_subsample_fq_salmon/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```
