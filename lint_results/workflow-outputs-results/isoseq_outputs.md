# Workflow outputs migration: isoseq

- Generated: 2026-06-16T20:27:16.510606+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 16 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/conf/modules.config#L15) — 14 references
- [`modules/nf-core/isoseq/refine/tests/nextflow.config`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/modules/nf-core/isoseq/refine/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/lima/tests/nextflow.config`](https://github.com/nf-core/isoseq/blob/6f7705489a38e6152d1ea9f9d11c484b2356f440/modules/nf-core/lima/tests/nextflow.config#L3) — 1 reference
