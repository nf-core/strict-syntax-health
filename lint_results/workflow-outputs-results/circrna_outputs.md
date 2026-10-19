# Workflow outputs migration: circrna

- Generated: 2026-10-19T00:19:35.503337+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 137 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/circrna/blob/a47ab59b5dce516a517a3e643d92257fa87a5c93/conf/modules.config#L15) — 136 references
- [`subworkflows/local/mirna_prediction/tests/no_correlation.config`](https://github.com/nf-core/circrna/blob/a47ab59b5dce516a517a3e643d92257fa87a5c93/subworkflows/local/mirna_prediction/tests/no_correlation.config#L7) — 1 reference
