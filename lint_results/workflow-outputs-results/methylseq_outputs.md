# Workflow outputs migration: methylseq

- Generated: 2026-06-16T14:23:08.590598+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 45 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules/bedtools_intersect.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/bedtools_intersect.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bedtools_intersect_cov.config:6`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/bedtools_intersect_cov.config#L6)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bismark_align.config:18`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/bismark_align.config#L18)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bismark_coverage2cytosine.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/bismark_coverage2cytosine.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bismark_deduplicate.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/bismark_deduplicate.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bismark_genomepreparation.config:7`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/bismark_genomepreparation.config#L7)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bismark_methylationextractor.config:13`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/bismark_methylationextractor.config#L13)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bismark_report.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/bismark_report.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bismark_summary.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/bismark_summary.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bwa_index.config:3`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/bwa_index.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bwamem_align.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/bwamem_align.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bwameth_align.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/bwameth_align.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bwameth_index.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/bwameth_index.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/fastqc.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/fastqc.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gunzip.config:3`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/gunzip.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/methyldackel_extract.config:10`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/methyldackel_extract.config#L10)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/methyldackel_mbias.config:7`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/methyldackel_mbias.config#L7)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/multiqc.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/multiqc.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/parabricks_fq2bammeth.config:5`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/parabricks_fq2bammeth.config#L5)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/picard_addorreplacereadgroups.config:5`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/picard_addorreplacereadgroups.config#L5)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/picard_bedtointervallist.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/picard_bedtointervallist.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/picard_collecthsmetrics.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/picard_collecthsmetrics.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/picard_createsequencedictionary.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/picard_createsequencedictionary.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/picard_markduplicates.config:5`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/picard_markduplicates.config#L5)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/picard_removeduplicates.config:5`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/picard_removeduplicates.config#L5)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/preseq_lcextrap.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/preseq_lcextrap.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/qualimap_bamqc.config:7`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/qualimap_bamqc.config#L7)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/rastair_call.config:8`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/rastair_call.config#L8)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/rastair_mbias.config:3`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/rastair_mbias.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/rastair_mbiasparser.config:3`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/rastair_mbiasparser.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/rastair_methylkit.config:3`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/rastair_methylkit.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/samtools_faidx.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/samtools_faidx.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/samtools_flagstat.config:3`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/samtools_flagstat.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/samtools_idxstats.config:3`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/samtools_idxstats.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/samtools_index.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/samtools_index.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/samtools_sort.config:4`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/samtools_sort.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/samtools_stats.config:3`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/samtools_stats.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/trimgalore.config:62`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/modules/trimgalore.config#L62)

  ```nextflow
  publishDir = [
  ```

- [`conf/subworkflows/fastq_align_dedup_bismark.config:17`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/subworkflows/fastq_align_dedup_bismark.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/subworkflows/fastq_align_dedup_bwamem.config:17`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/subworkflows/fastq_align_dedup_bwamem.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/subworkflows/fastq_align_dedup_bwamem.config:29`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/subworkflows/fastq_align_dedup_bwamem.config#L29)

  ```nextflow
  publishDir = [
  ```

- [`conf/subworkflows/fastq_align_dedup_bwamem.config:41`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/subworkflows/fastq_align_dedup_bwamem.config#L41)

  ```nextflow
  publishDir = [
  ```

- [`conf/subworkflows/fastq_align_dedup_bwameth.config:13`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/subworkflows/fastq_align_dedup_bwameth.config#L13)

  ```nextflow
  publishDir = [
  ```

- [`conf/subworkflows/fastq_align_dedup_bwameth.config:25`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/conf/subworkflows/fastq_align_dedup_bwameth.config#L25)

  ```nextflow
  publishDir = [
  ```

- [`workflows/methylseq/nextflow.config:20`](https://github.com/nf-core/methylseq/blob/d39c3deb67e65f0f93f83b0096a54278339731be/workflows/methylseq/nextflow.config#L20)

  ```nextflow
  publishDir = [
  ```
