# Workflow outputs migration: lncpipe

- Generated: 2026-06-16T19:29:08.377717+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 39 `publishDir` references across 14 files that should be migrated to the workflow `output {}` block:

- [`subworkflows/local/prepare_genome/nextflow.config`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/local/prepare_genome/nextflow.config#L3) — 13 references
- [`conf/modules.config`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/conf/modules.config#L15) — 4 references
- [`subworkflows/nf-core/fastq_fastqc_umitools_fastp/nextflow.config`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_fastqc_umitools_fastp/nextflow.config#L7) — 4 references
- [`subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/nextflow.config`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/nextflow.config#L5) — 4 references
- [`subworkflows/nf-core/fastq_fastqc_umitools_trimgalore/nextflow.config`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_fastqc_umitools_trimgalore/nextflow.config#L7) — 3 references
- [`subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config#L22) — 2 references
- [`subworkflows/nf-core/fastq_subsample_fq_salmon/nextflow.config`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_subsample_fq_salmon/nextflow.config#L5) — 2 references
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/local/stringtie/nextflow.config`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/local/stringtie/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_align_star/nextflow.config`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_align_star/nextflow.config#L26) — 1 reference
- [`subworkflows/nf-core/fastq_align_star/tests/nextflow.config`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_align_star/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_subsample_fq_salmon/tests/nextflow.config`](https://github.com/nf-core/lncpipe/blob/39e1e236c8a6624912f8e74bbf3e817bd94b987c/subworkflows/nf-core/fastq_subsample_fq_salmon/tests/nextflow.config#L3) — 1 reference
