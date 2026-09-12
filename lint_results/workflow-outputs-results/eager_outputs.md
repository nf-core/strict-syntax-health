# Workflow outputs migration: eager

- Generated: 2026-09-12T00:19:14.408322+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 126 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/eager/blob/4c7ed5bba146bab7628db71d5eabda740b847c9b/conf/modules.config#L15) — 125 references
- [`subworkflows/nf-core/fastq_align_bwaaln/nextflow.config`](https://github.com/nf-core/eager/blob/4c7ed5bba146bab7628db71d5eabda740b847c9b/subworkflows/nf-core/fastq_align_bwaaln/nextflow.config#L7) — 1 reference
