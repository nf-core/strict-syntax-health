# Workflow outputs migration: isoseq

- Generated: 2026-08-18T00:13:39.855904+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 15 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/isoseq/blob/f7d11f3993cd5a56d2faf2875dbf06a4c40d88f8/conf/modules.config#L15) — 14 references
- [`modules/nf-core/lima/tests/nextflow.config`](https://github.com/nf-core/isoseq/blob/f7d11f3993cd5a56d2faf2875dbf06a4c40d88f8/modules/nf-core/lima/tests/nextflow.config#L3) — 1 reference
