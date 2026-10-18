# Workflow outputs migration: circrna

- Generated: 2026-10-18T00:19:48.231435+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 128 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/circrna/blob/ff26767df62cdeae4b8b5a47d2abbb0881846cf6/conf/modules.config#L15) — 127 references
- [`subworkflows/local/mirna_prediction/tests/no_correlation.config`](https://github.com/nf-core/circrna/blob/ff26767df62cdeae4b8b5a47d2abbb0881846cf6/subworkflows/local/mirna_prediction/tests/no_correlation.config#L7) — 1 reference
