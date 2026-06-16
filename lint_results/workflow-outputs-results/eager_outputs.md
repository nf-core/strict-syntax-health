# Workflow outputs migration: eager

- Generated: 2026-06-16T20:23:22.429018+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 127 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L15) — 126 references
- [`subworkflows/nf-core/fastq_align_bwaaln/nextflow.config`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/subworkflows/nf-core/fastq_align_bwaaln/nextflow.config#L7) — 1 reference
