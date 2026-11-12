# Workflow outputs migration: rnafusion

- Generated: 2026-11-12T00:17:56.362079+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 36 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/rnafusion/blob/70998bc008a5bad6bf4302d6fb4fa948b72d7eaf/conf/modules.config#L15) — 34 references
- [`subworkflows/nf-core/fastq_align_star/tests/nextflow.config`](https://github.com/nf-core/rnafusion/blob/70998bc008a5bad6bf4302d6fb4fa948b72d7eaf/subworkflows/nf-core/fastq_align_star/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config`](https://github.com/nf-core/rnafusion/blob/70998bc008a5bad6bf4302d6fb4fa948b72d7eaf/subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config#L3) — 1 reference
