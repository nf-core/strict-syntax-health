# Workflow outputs migration: chipseq

- Generated: 2026-07-25T00:31:03.493262+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 57 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/chipseq/blob/f3bb13a4a82be9f0603e2d6610f93f9f64ec5b09/conf/modules.config#L19) — 55 references
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/chipseq/blob/f3bb13a4a82be9f0603e2d6610f93f9f64ec5b09/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/chipseq/blob/f3bb13a4a82be9f0603e2d6610f93f9f64ec5b09/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
