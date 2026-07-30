# Workflow outputs migration: riboseq

- Generated: 2026-07-30T00:31:53.556550+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 134 `publishDir` references across 6 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/riboseq/blob/813a792ed2f1102e459ab0085e081b447276bfaa/conf/modules.config#L18) — 128 references
- [`subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config`](https://github.com/nf-core/riboseq/blob/813a792ed2f1102e459ab0085e081b447276bfaa/subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config#L22) — 2 references
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/riboseq/blob/813a792ed2f1102e459ab0085e081b447276bfaa/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_align_star/tests/nextflow.config`](https://github.com/nf-core/riboseq/blob/813a792ed2f1102e459ab0085e081b447276bfaa/subworkflows/nf-core/fastq_align_star/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config`](https://github.com/nf-core/riboseq/blob/813a792ed2f1102e459ab0085e081b447276bfaa/subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_subsample_fq_salmon/tests/nextflow.config`](https://github.com/nf-core/riboseq/blob/813a792ed2f1102e459ab0085e081b447276bfaa/subworkflows/nf-core/fastq_subsample_fq_salmon/tests/nextflow.config#L3) — 1 reference
