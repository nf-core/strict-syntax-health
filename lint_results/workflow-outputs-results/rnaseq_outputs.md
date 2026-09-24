# Workflow outputs migration: rnaseq

- Generated: 2026-09-24T00:20:45.335332+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 113 `publishDir` references across 42 files that should be migrated to the workflow `output {}` block:

- [`conf/modules/prepare_genome.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/prepare_genome.config#L3) — 18 references
- [`conf/modules/qc_trim_filter.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/qc_trim_filter.config#L5) — 12 references
- [`conf/modules/quantify_bam_salmon.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/quantify_bam_salmon.config#L8) — 11 references
- [`conf/modules/rseqc.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/rseqc.config#L3) — 8 references
- [`conf/modules/umi_dedup.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/umi_dedup.config#L26) — 6 references
- [`conf/modules/quantify_pseudo_alignment.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/quantify_pseudo_alignment.config#L30) — 5 references
- [`conf/modules/fastp.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/fastp.config#L5) — 4 references
- [`conf/modules/quantify_rsem.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/quantify_rsem.config#L7) — 4 references
- [`conf/modules/markduplicates.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/markduplicates.config#L5) — 3 references
- [`conf/modules/stringtie.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/stringtie.config#L8) — 3 references
- [`conf/modules/trimgalore.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/trimgalore.config#L5) — 3 references
- [`conf/modules/alignment.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/alignment.config#L8) — 2 references
- [`conf/modules/bigwig.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/bigwig.config#L22) — 2 references
- [`conf/modules/qualimap.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/qualimap.config#L5) — 2 references
- [`conf/modules/strandedness.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/strandedness.config#L5) — 2 references
- [`subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config#L22) — 2 references
- [`conf/modules/align_bowtie2.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/align_bowtie2.config#L37) — 1 reference
- [`conf/modules/align_hisat2.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/align_hisat2.config#L36) — 1 reference
- [`conf/modules/align_star.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/align_star.config#L136) — 1 reference
- [`conf/modules/bbsplit.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/bbsplit.config#L4) — 1 reference
- [`conf/modules/bracken.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/bracken.config#L4) — 1 reference
- [`conf/modules/cat_fastq.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/cat_fastq.config#L3) — 1 reference
- [`conf/modules/deseq2_qc.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/deseq2_qc.config#L14) — 1 reference
- [`conf/modules/dupradar.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/dupradar.config#L3) — 1 reference
- [`conf/modules/featurecounts.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/featurecounts.config#L8) — 1 reference
- [`conf/modules/kraken2.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/kraken2.config#L6) — 1 reference
- [`conf/modules/multiqc.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/multiqc.config#L7) — 1 reference
- [`conf/modules/multiqc_custom_biotype.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/multiqc_custom_biotype.config#L3) — 1 reference
- [`conf/modules/preseq.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/preseq.config#L4) — 1 reference
- [`conf/modules/rustqc.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/rustqc.config#L15) — 1 reference
- [`conf/modules/sortmerna.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/sortmerna.config#L4) — 1 reference
- [`conf/modules/sylph.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/sylph.config#L7) — 1 reference
- [`conf/modules/sylphtax.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/conf/modules/sylphtax.config#L3) — 1 reference
- [`modules/nf-core/rsem/calculateexpression/tests/alignment.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/modules/nf-core/rsem/calculateexpression/tests/alignment.config#L3) — 1 reference
- [`modules/nf-core/rsem/calculateexpression/tests/nextflow.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/modules/nf-core/rsem/calculateexpression/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/rseqc/bamstat/tests/nextflow.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/modules/nf-core/rseqc/bamstat/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/rseqc/inferexperiment/tests/nextflow.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/modules/nf-core/rseqc/inferexperiment/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
- [`nextflow.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/nextflow.config#L177) — 1 reference
- [`subworkflows/local/align_star/tests/nextflow.extra_args.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/subworkflows/local/align_star/tests/nextflow.extra_args.config#L26) — 1 reference
- [`subworkflows/local/align_star/tests/nextflow.rg.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/subworkflows/local/align_star/tests/nextflow.rg.config#L26) — 1 reference
- [`subworkflows/nf-core/bedgraph_bedclip_bedgraphtobigwig/tests/nextflow.config`](https://github.com/nf-core/rnaseq/blob/a2283f4bce7f779e16ee9e2dcd84d8d288f71fec/subworkflows/nf-core/bedgraph_bedclip_bedgraphtobigwig/tests/nextflow.config#L3) — 1 reference
