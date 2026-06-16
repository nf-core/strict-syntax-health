# Workflow outputs migration: dualrnaseq

- Generated: 2026-06-16T20:23:10.435172+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 30 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L15) — 28 references
- [`modules/local/collate_processed_reads/main.nf`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/modules/local/collate_processed_reads/main.nf#L7) — 1 reference
- [`modules/local/extract_processed_reads/main.nf`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/modules/local/extract_processed_reads/main.nf#L12) — 1 reference
