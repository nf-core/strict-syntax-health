# Workflow outputs migration: nascent

- Generated: 2026-07-17T00:30:21.814001+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 42 `publishDir` references across 7 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/nascent/blob/ebf514a90e677515733aa62314a98dbf8df2e5ef/conf/modules.config#L15) — 36 references
- [`modules/nf-core/rseqc/bamstat/tests/nextflow.config`](https://github.com/nf-core/nascent/blob/ebf514a90e677515733aa62314a98dbf8df2e5ef/modules/nf-core/rseqc/bamstat/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/rseqc/inferexperiment/tests/nextflow.config`](https://github.com/nf-core/nascent/blob/ebf514a90e677515733aa62314a98dbf8df2e5ef/modules/nf-core/rseqc/inferexperiment/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/rseqc/innerdistance/tests/nextflow.config`](https://github.com/nf-core/nascent/blob/ebf514a90e677515733aa62314a98dbf8df2e5ef/modules/nf-core/rseqc/innerdistance/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/nascent/blob/ebf514a90e677515733aa62314a98dbf8df2e5ef/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_align_star/tests/nextflow.config`](https://github.com/nf-core/nascent/blob/ebf514a90e677515733aa62314a98dbf8df2e5ef/subworkflows/nf-core/fastq_align_star/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config`](https://github.com/nf-core/nascent/blob/ebf514a90e677515733aa62314a98dbf8df2e5ef/subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config#L3) — 1 reference
