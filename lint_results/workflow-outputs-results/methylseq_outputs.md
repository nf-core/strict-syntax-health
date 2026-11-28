# Workflow outputs migration: methylseq

- Generated: 2026-11-28T00:12:57.848348+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 73 `publishDir` references across 57 files that should be migrated to the workflow `output {}` block:

- [`conf/subworkflows/fastq_controls_bismark.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/subworkflows/fastq_controls_bismark.config#L5) — 6 references
- [`conf/subworkflows/fastq_align_dedup_umi_bwamem3.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/subworkflows/fastq_align_dedup_umi_bwamem3.config#L7) — 4 references
- [`conf/modules/rastair2_call.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/rastair2_call.config#L5) — 3 references
- [`conf/subworkflows/fastq_align_dedup_bwamem.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/subworkflows/fastq_align_dedup_bwamem.config#L19) — 3 references
- [`conf/modules/methylation_summary.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/methylation_summary.config#L11) — 2 references
- [`conf/modules/methylsieve.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/methylsieve.config#L8) — 2 references
- [`conf/modules/preseq_lcextrap.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/preseq_lcextrap.config#L4) — 2 references
- [`conf/subworkflows/fastq_align_dedup_bwameth.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/subworkflows/fastq_align_dedup_bwameth.config#L13) — 2 references
- [`conf/modules/bedtools_intersect.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/bedtools_intersect.config#L4) — 1 reference
- [`conf/modules/bismark_align.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/bismark_align.config#L40) — 1 reference
- [`conf/modules/bismark_coverage2cytosine.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/bismark_coverage2cytosine.config#L4) — 1 reference
- [`conf/modules/bismark_deduplicate.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/bismark_deduplicate.config#L4) — 1 reference
- [`conf/modules/bismark_genomepreparation.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/bismark_genomepreparation.config#L9) — 1 reference
- [`conf/modules/bismark_methylationextractor.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/bismark_methylationextractor.config#L24) — 1 reference
- [`conf/modules/bismark_report.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/bismark_report.config#L4) — 1 reference
- [`conf/modules/bismark_summary.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/bismark_summary.config#L4) — 1 reference
- [`conf/modules/bwa_index.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/bwa_index.config#L3) — 1 reference
- [`conf/modules/bwamem3_index.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/bwamem3_index.config#L8) — 1 reference
- [`conf/modules/bwamem3_mem.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/bwamem3_mem.config#L7) — 1 reference
- [`conf/modules/bwamem_align.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/bwamem_align.config#L4) — 1 reference
- [`conf/modules/bwameth_align.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/bwameth_align.config#L4) — 1 reference
- [`conf/modules/bwameth_index.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/bwameth_index.config#L4) — 1 reference
- [`conf/modules/fastqc.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/fastqc.config#L4) — 1 reference
- [`conf/modules/filter_cov_targets.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/filter_cov_targets.config#L4) — 1 reference
- [`conf/modules/gunzip.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/gunzip.config#L3) — 1 reference
- [`conf/modules/merge_targets.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/merge_targets.config#L3) — 1 reference
- [`conf/modules/methurator_gtestimator.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/methurator_gtestimator.config#L9) — 1 reference
- [`conf/modules/methurator_plot.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/methurator_plot.config#L3) — 1 reference
- [`conf/modules/methyldackel_extract.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/methyldackel_extract.config#L10) — 1 reference
- [`conf/modules/methyldackel_mbias.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/methyldackel_mbias.config#L7) — 1 reference
- [`conf/modules/multiqc.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/multiqc.config#L4) — 1 reference
- [`conf/modules/parabricks_fq2bam.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/parabricks_fq2bam.config#L4) — 1 reference
- [`conf/modules/parabricks_fq2bammeth.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/parabricks_fq2bammeth.config#L5) — 1 reference
- [`conf/modules/picard_addorreplacereadgroups.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/picard_addorreplacereadgroups.config#L5) — 1 reference
- [`conf/modules/picard_bedtointervallist.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/picard_bedtointervallist.config#L4) — 1 reference
- [`conf/modules/picard_collecthsmetrics.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/picard_collecthsmetrics.config#L5) — 1 reference
- [`conf/modules/picard_createsequencedictionary.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/picard_createsequencedictionary.config#L4) — 1 reference
- [`conf/modules/picard_markduplicates.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/picard_markduplicates.config#L5) — 1 reference
- [`conf/modules/picard_removeduplicates.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/picard_removeduplicates.config#L5) — 1 reference
- [`conf/modules/qualimap_bamqc.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/qualimap_bamqc.config#L7) — 1 reference
- [`conf/modules/rastair2_mbias.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/rastair2_mbias.config#L13) — 1 reference
- [`conf/modules/rastair_call.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/rastair_call.config#L3) — 1 reference
- [`conf/modules/rastair_mbias.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/rastair_mbias.config#L3) — 1 reference
- [`conf/modules/rastair_mbiasparser.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/rastair_mbiasparser.config#L3) — 1 reference
- [`conf/modules/rastair_methylkit.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/rastair_methylkit.config#L3) — 1 reference
- [`conf/modules/riker_multi.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/riker_multi.config#L12) — 1 reference
- [`conf/modules/samtools_faidx.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/samtools_faidx.config#L4) — 1 reference
- [`conf/modules/samtools_flagstat.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/samtools_flagstat.config#L3) — 1 reference
- [`conf/modules/samtools_idxstats.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/samtools_idxstats.config#L3) — 1 reference
- [`conf/modules/samtools_index.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/samtools_index.config#L4) — 1 reference
- [`conf/modules/samtools_sort.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/samtools_sort.config#L4) — 1 reference
- [`conf/modules/samtools_stats.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/samtools_stats.config#L3) — 1 reference
- [`conf/modules/trimgalore.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/trimgalore.config#L64) — 1 reference
- [`conf/modules/widen_targets_cpg.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/modules/widen_targets_cpg.config#L3) — 1 reference
- [`conf/subworkflows/fastq_align_dedup_bismark.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/subworkflows/fastq_align_dedup_bismark.config#L17) — 1 reference
- [`conf/subworkflows/fastq_align_dedup_bwamem3.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/conf/subworkflows/fastq_align_dedup_bwamem3.config#L10) — 1 reference
- [`workflows/methylseq/nextflow.config`](https://github.com/nf-core/methylseq/blob/979532009f2e9a31eadfbd9004086c7bc9f0d75c/workflows/methylseq/nextflow.config#L31) — 1 reference
