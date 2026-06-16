# Workflow outputs migration: pacvar

- Generated: 2026-06-16T19:34:42.286461+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 15 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules.config#L14) — 9 references
- [`conf/modules/ensemblvep.config`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules/ensemblvep.config#L18) — 4 references
- [`conf/modules/fibertools.config`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules/fibertools.config#L3) — 1 reference
- [`modules/nf-core/lima/tests/nextflow.config`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/modules/nf-core/lima/tests/nextflow.config#L3) — 1 reference
