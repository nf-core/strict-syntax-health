# Workflow outputs migration: pacvar

- Generated: 2026-06-24T00:36:48.034934+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 15 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/pacvar/blob/7a7ab8f18feb8b3d59c177a17d7d684bb900c1b7/conf/modules.config#L14) — 9 references
- [`conf/modules/ensemblvep.config`](https://github.com/nf-core/pacvar/blob/7a7ab8f18feb8b3d59c177a17d7d684bb900c1b7/conf/modules/ensemblvep.config#L18) — 4 references
- [`conf/modules/fibertools.config`](https://github.com/nf-core/pacvar/blob/7a7ab8f18feb8b3d59c177a17d7d684bb900c1b7/conf/modules/fibertools.config#L3) — 1 reference
- [`modules/nf-core/lima/tests/nextflow.config`](https://github.com/nf-core/pacvar/blob/7a7ab8f18feb8b3d59c177a17d7d684bb900c1b7/modules/nf-core/lima/tests/nextflow.config#L3) — 1 reference
