# Workflow outputs migration: omicsgenetraitassociation

- Generated: 2026-10-08T00:27:55.487772+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 11 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/omicsgenetraitassociation/blob/f6702ce5f9e423dd896f55034af2f4f78ba7223f/conf/modules.config#L15) — 9 references
- [`conf/cma_mea.config`](https://github.com/nf-core/omicsgenetraitassociation/blob/f6702ce5f9e423dd896f55034af2f4f78ba7223f/conf/cma_mea.config#L32) — 1 reference
- [`conf/test_local.config`](https://github.com/nf-core/omicsgenetraitassociation/blob/f6702ce5f9e423dd896f55034af2f4f78ba7223f/conf/test_local.config#L53) — 1 reference
