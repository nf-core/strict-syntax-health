# Workflow outputs migration: methylseq

- Generated: 2026-07-16T00:28:47.523891+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 45 `publishDir` references across 42 files that should be migrated to the workflow `output {}` block:

- [`conf/subworkflows/fastq_align_dedup_bwamem.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/subworkflows/fastq_align_dedup_bwamem.config#L17) — 3 references
- [`conf/subworkflows/fastq_align_dedup_bwameth.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/subworkflows/fastq_align_dedup_bwameth.config#L13) — 2 references
- [`conf/modules/bedtools_intersect.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/bedtools_intersect.config#L4) — 1 reference
- [`conf/modules/bedtools_intersect_cov.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/bedtools_intersect_cov.config#L6) — 1 reference
- [`conf/modules/bismark_align.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/bismark_align.config#L18) — 1 reference
- [`conf/modules/bismark_coverage2cytosine.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/bismark_coverage2cytosine.config#L4) — 1 reference
- [`conf/modules/bismark_deduplicate.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/bismark_deduplicate.config#L4) — 1 reference
- [`conf/modules/bismark_genomepreparation.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/bismark_genomepreparation.config#L7) — 1 reference
- [`conf/modules/bismark_methylationextractor.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/bismark_methylationextractor.config#L13) — 1 reference
- [`conf/modules/bismark_report.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/bismark_report.config#L4) — 1 reference
- [`conf/modules/bismark_summary.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/bismark_summary.config#L4) — 1 reference
- [`conf/modules/bwa_index.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/bwa_index.config#L3) — 1 reference
- [`conf/modules/bwamem_align.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/bwamem_align.config#L4) — 1 reference
- [`conf/modules/bwameth_align.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/bwameth_align.config#L4) — 1 reference
- [`conf/modules/bwameth_index.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/bwameth_index.config#L4) — 1 reference
- [`conf/modules/fastqc.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/fastqc.config#L4) — 1 reference
- [`conf/modules/gunzip.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/gunzip.config#L3) — 1 reference
- [`conf/modules/methyldackel_extract.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/methyldackel_extract.config#L10) — 1 reference
- [`conf/modules/methyldackel_mbias.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/methyldackel_mbias.config#L7) — 1 reference
- [`conf/modules/multiqc.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/multiqc.config#L4) — 1 reference
- [`conf/modules/parabricks_fq2bammeth.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/parabricks_fq2bammeth.config#L5) — 1 reference
- [`conf/modules/picard_addorreplacereadgroups.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/picard_addorreplacereadgroups.config#L5) — 1 reference
- [`conf/modules/picard_bedtointervallist.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/picard_bedtointervallist.config#L4) — 1 reference
- [`conf/modules/picard_collecthsmetrics.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/picard_collecthsmetrics.config#L4) — 1 reference
- [`conf/modules/picard_createsequencedictionary.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/picard_createsequencedictionary.config#L4) — 1 reference
- [`conf/modules/picard_markduplicates.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/picard_markduplicates.config#L5) — 1 reference
- [`conf/modules/picard_removeduplicates.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/picard_removeduplicates.config#L5) — 1 reference
- [`conf/modules/preseq_lcextrap.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/preseq_lcextrap.config#L4) — 1 reference
- [`conf/modules/qualimap_bamqc.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/qualimap_bamqc.config#L7) — 1 reference
- [`conf/modules/rastair_call.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/rastair_call.config#L8) — 1 reference
- [`conf/modules/rastair_mbias.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/rastair_mbias.config#L3) — 1 reference
- [`conf/modules/rastair_mbiasparser.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/rastair_mbiasparser.config#L3) — 1 reference
- [`conf/modules/rastair_methylkit.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/rastair_methylkit.config#L3) — 1 reference
- [`conf/modules/samtools_faidx.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/samtools_faidx.config#L4) — 1 reference
- [`conf/modules/samtools_flagstat.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/samtools_flagstat.config#L3) — 1 reference
- [`conf/modules/samtools_idxstats.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/samtools_idxstats.config#L3) — 1 reference
- [`conf/modules/samtools_index.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/samtools_index.config#L4) — 1 reference
- [`conf/modules/samtools_sort.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/samtools_sort.config#L4) — 1 reference
- [`conf/modules/samtools_stats.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/samtools_stats.config#L3) — 1 reference
- [`conf/modules/trimgalore.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/modules/trimgalore.config#L62) — 1 reference
- [`conf/subworkflows/fastq_align_dedup_bismark.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/conf/subworkflows/fastq_align_dedup_bismark.config#L17) — 1 reference
- [`workflows/methylseq/nextflow.config`](https://github.com/nf-core/methylseq/blob/ba449675bbaa47c4f198c60fc1bcc2c1fba0cedf/workflows/methylseq/nextflow.config#L20) — 1 reference
