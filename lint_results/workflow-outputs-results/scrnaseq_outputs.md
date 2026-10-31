# Workflow outputs migration: scrnaseq

- Generated: 2026-10-31T00:18:59.282043+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 26 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/scrnaseq/blob/a45ac11ba806fbc17dd421a0d1cb8aaa3f519dbf/conf/modules.config#L14) — 24 references
- [`modules/local/parse_cellrangermulti_samplesheet/main.nf`](https://github.com/nf-core/scrnaseq/blob/a45ac11ba806fbc17dd421a0d1cb8aaa3f519dbf/modules/local/parse_cellrangermulti_samplesheet/main.nf#L8) — 1 reference
- [`modules/nf-core/cellranger/mkref/tests/nextflow.config`](https://github.com/nf-core/scrnaseq/blob/a45ac11ba806fbc17dd421a0d1cb8aaa3f519dbf/modules/nf-core/cellranger/mkref/tests/nextflow.config#L8) — 1 reference
