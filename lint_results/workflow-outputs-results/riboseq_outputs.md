# Workflow outputs migration: riboseq

- Generated: 2026-07-07T00:38:01.083534+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 123 `publishDir` references across 6 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/riboseq/blob/68002f9b8da43389a23d8f9b4f6ac89dc9d95409/conf/modules.config#L18) — 117 references
- [`subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config`](https://github.com/nf-core/riboseq/blob/68002f9b8da43389a23d8f9b4f6ac89dc9d95409/subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config#L22) — 2 references
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/riboseq/blob/68002f9b8da43389a23d8f9b4f6ac89dc9d95409/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_align_star/tests/nextflow.config`](https://github.com/nf-core/riboseq/blob/68002f9b8da43389a23d8f9b4f6ac89dc9d95409/subworkflows/nf-core/fastq_align_star/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config`](https://github.com/nf-core/riboseq/blob/68002f9b8da43389a23d8f9b4f6ac89dc9d95409/subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_subsample_fq_salmon/tests/nextflow.config`](https://github.com/nf-core/riboseq/blob/68002f9b8da43389a23d8f9b4f6ac89dc9d95409/subworkflows/nf-core/fastq_subsample_fq_salmon/tests/nextflow.config#L3) — 1 reference
