# Workflow outputs migration: genomicrelatedness

- Generated: 2026-06-16T14:18:43.890385+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 62 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/angsd_ngsrelate.config:18`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/angsd_ngsrelate.config#L18)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bcftools_call.config:17`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/bcftools_call.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bcftools_concat.config:17`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/bcftools_concat.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bcftools_index.config:17`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/bcftools_index.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bcftools_isec.config:17`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/bcftools_isec.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bcftools_mpileup.config:17`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/bcftools_mpileup.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bcftools_query.config:18`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/bcftools_query.config#L18)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bcftools_sort.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/bcftools_sort.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bcftools_sort.config:23`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/bcftools_sort.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bcftools_stats.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/bcftools_stats.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bcftools_stats.config:23`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/bcftools_stats.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/bwamem2_mem.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/bwamem2_mem.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/fastp.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/fastp.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_addorreplacereadgroups.config:21`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_addorreplacereadgroups.config#L21)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_analyzecovariates.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_analyzecovariates.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_analyzecovariates.config:23`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_analyzecovariates.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_applybqsr.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_applybqsr.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_applybqsr.config:23`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_applybqsr.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_baserecalibrator.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_baserecalibrator.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_baserecalibrator.config:23`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_baserecalibrator.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_gatherbqsrreports.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_gatherbqsrreports.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_gatherbqsrreports.config:23`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_gatherbqsrreports.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_genomicsdbimport.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_genomicsdbimport.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_genomicsdbimport.config:23`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_genomicsdbimport.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_genotypegvcfs.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_genotypegvcfs.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_genotypegvcfs.config:23`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_genotypegvcfs.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_haplotypecaller.config:19`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_haplotypecaller.config#L19)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_haplotypecaller.config:26`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_haplotypecaller.config#L26)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_markduplicates.config:17`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_markduplicates.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_mergevcfs.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_mergevcfs.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gatk4_mergevcfs.config:23`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gatk4_mergevcfs.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gunzip.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/gunzip.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/make_scaffold_bed.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/make_scaffold_bed.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/make_scaffold_bed.config:23`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/make_scaffold_bed.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/mosdepth.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/mosdepth.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/normalize_bam_names.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/normalize_bam_names.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/preseq_ccurve.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/preseq_ccurve.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/preseq_lcextrap.config:18`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/preseq_lcextrap.config#L18)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/samtools_convert.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/samtools_convert.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/samtools_index.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/samtools_index.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/samtools_index.config:23`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/samtools_index.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/samtools_index.config:30`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/samtools_index.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/samtools_merge.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/samtools_merge.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/samtools_merge.config:25`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/samtools_merge.config#L25)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/samtools_merge.config:33`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/samtools_merge.config#L33)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/samtools_stats.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/samtools_stats.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/splitintervals.config:17`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/splitintervals.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/spring.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/spring.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/vcftools.config:18`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/vcftools.config#L18)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/vcftools.config:26`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/modules/vcftools.config#L26)

  ```nextflow
  publishDir = [
  ```

- [`conf/subworkflows/cram_baserecalibrator.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/subworkflows/cram_baserecalibrator.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/subworkflows/cram_baserecalibrator.config:23`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/subworkflows/cram_baserecalibrator.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/subworkflows/filter_variants.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/subworkflows/filter_variants.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/subworkflows/filter_variants.config:24`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/subworkflows/filter_variants.config#L24)

  ```nextflow
  publishDir = [
  ```

- [`conf/subworkflows/prepare_genome.config:17`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/subworkflows/prepare_genome.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/subworkflows/prepare_genome.config:25`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/subworkflows/prepare_genome.config#L25)

  ```nextflow
  publishDir = [
  ```

- [`conf/subworkflows/prepare_genome.config:33`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/subworkflows/prepare_genome.config#L33)

  ```nextflow
  publishDir = [
  ```

- [`conf/subworkflows/prepare_intervals.config:16`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/conf/subworkflows/prepare_intervals.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/spring/decompress/tests/nextflow.config:3`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/modules/nf-core/spring/decompress/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`nextflow.config:76`](https://github.com/nf-core/genomicrelatedness/blob/14c1035344db22683551b3455e42fddaed9ea60c/nextflow.config#L76)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
