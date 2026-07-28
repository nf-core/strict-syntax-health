# Workflow outputs migration: sammyseq

- Generated: 2026-07-28T00:35:07.423834+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 34 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/sammyseq/blob/aa5def92cf320d2815d2276b16682f712dd1aba3/conf/modules.config#L14) — 33 references
- [`subworkflows/nf-core/fastq_align_bwaaln/nextflow.config`](https://github.com/nf-core/sammyseq/blob/aa5def92cf320d2815d2276b16682f712dd1aba3/subworkflows/nf-core/fastq_align_bwaaln/nextflow.config#L7) — 1 reference
