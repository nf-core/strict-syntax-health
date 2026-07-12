# Workflow outputs migration: scrnaseq

- Generated: 2026-07-12T00:29:09.344713+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 26 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/scrnaseq/blob/96dadeb2088a496970d68f0633e490f677c3dc7f/conf/modules.config#L14) — 24 references
- [`modules/local/parse_cellrangermulti_samplesheet/main.nf`](https://github.com/nf-core/scrnaseq/blob/96dadeb2088a496970d68f0633e490f677c3dc7f/modules/local/parse_cellrangermulti_samplesheet/main.nf#L8) — 1 reference
- [`modules/nf-core/cellranger/mkref/tests/nextflow.config`](https://github.com/nf-core/scrnaseq/blob/96dadeb2088a496970d68f0633e490f677c3dc7f/modules/nf-core/cellranger/mkref/tests/nextflow.config#L3) — 1 reference
