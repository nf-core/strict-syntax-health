# Workflow outputs migration: pacvar

- Generated: 2026-06-26T00:44:02.390816+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 15 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/pacvar/blob/8498d079d38a14d7b2e7ba9dc03d3079228a8cd6/conf/modules.config#L14) — 9 references
- [`conf/modules/ensemblvep.config`](https://github.com/nf-core/pacvar/blob/8498d079d38a14d7b2e7ba9dc03d3079228a8cd6/conf/modules/ensemblvep.config#L18) — 4 references
- [`conf/modules/fibertools.config`](https://github.com/nf-core/pacvar/blob/8498d079d38a14d7b2e7ba9dc03d3079228a8cd6/conf/modules/fibertools.config#L3) — 1 reference
- [`modules/nf-core/lima/tests/nextflow.config`](https://github.com/nf-core/pacvar/blob/8498d079d38a14d7b2e7ba9dc03d3079228a8cd6/modules/nf-core/lima/tests/nextflow.config#L3) — 1 reference
