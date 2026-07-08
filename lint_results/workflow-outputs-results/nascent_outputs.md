# Workflow outputs migration: nascent

- Generated: 2026-07-08T00:29:07.904704+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 41 `publishDir` references across 7 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/nascent/blob/3d5462861e331eba7c090b1e81dd107182228a74/conf/modules.config#L15) — 35 references
- [`modules/nf-core/rseqc/bamstat/tests/nextflow.config`](https://github.com/nf-core/nascent/blob/3d5462861e331eba7c090b1e81dd107182228a74/modules/nf-core/rseqc/bamstat/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/rseqc/inferexperiment/tests/nextflow.config`](https://github.com/nf-core/nascent/blob/3d5462861e331eba7c090b1e81dd107182228a74/modules/nf-core/rseqc/inferexperiment/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/rseqc/innerdistance/tests/nextflow.config`](https://github.com/nf-core/nascent/blob/3d5462861e331eba7c090b1e81dd107182228a74/modules/nf-core/rseqc/innerdistance/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/nascent/blob/3d5462861e331eba7c090b1e81dd107182228a74/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_align_star/tests/nextflow.config`](https://github.com/nf-core/nascent/blob/3d5462861e331eba7c090b1e81dd107182228a74/subworkflows/nf-core/fastq_align_star/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config`](https://github.com/nf-core/nascent/blob/3d5462861e331eba7c090b1e81dd107182228a74/subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config#L3) — 1 reference
