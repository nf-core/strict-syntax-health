# Workflow outputs migration: omicsgenetraitassociation

- Generated: 2026-06-16T19:33:59.600308+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 11 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/omicsgenetraitassociation/blob/f64a3c7867ffe159a0f347d3b07d11c99ade49fb/conf/modules.config#L15) — 9 references
- [`conf/cma_mea.config`](https://github.com/nf-core/omicsgenetraitassociation/blob/f64a3c7867ffe159a0f347d3b07d11c99ade49fb/conf/cma_mea.config#L32) — 1 reference
- [`conf/test_local.config`](https://github.com/nf-core/omicsgenetraitassociation/blob/f64a3c7867ffe159a0f347d3b07d11c99ade49fb/conf/test_local.config#L53) — 1 reference
