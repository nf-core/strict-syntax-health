# Workflow outputs migration: sammyseq

- Generated: 2026-06-16T19:41:34.731590+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 30 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L14) — 29 references
- [`subworkflows/nf-core/fastq_align_bwaaln/nextflow.config`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/subworkflows/nf-core/fastq_align_bwaaln/nextflow.config#L7) — 1 reference
