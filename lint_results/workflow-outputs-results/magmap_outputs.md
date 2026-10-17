# Workflow outputs migration: magmap

- Generated: 2026-10-17T00:20:14.182739+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 30 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/magmap/blob/dfbd3ad34c315642c2dab434b49122f76de11a18/conf/modules.config#L15) — 29 references
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/magmap/blob/dfbd3ad34c315642c2dab434b49122f76de11a18/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
