# Workflow outputs migration: rnastructurome

- Generated: 2026-08-14T00:22:52.878413+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 53 `publishDir` references across 7 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/rnastructurome/blob/605dd9f6f14dfb0d802bb2994cbef0393c8797e1/conf/modules.config#L14) — 47 references
- [`modules/local/r2dt/tests/nextflow.config`](https://github.com/nf-core/rnastructurome/blob/605dd9f6f14dfb0d802bb2994cbef0393c8797e1/modules/local/r2dt/tests/nextflow.config#L4) — 1 reference
- [`modules/local/rnaframework/fold/tests/nextflow.config`](https://github.com/nf-core/rnastructurome/blob/605dd9f6f14dfb0d802bb2994cbef0393c8797e1/modules/local/rnaframework/fold/tests/nextflow.config#L4) — 1 reference
- [`modules/local/samtools/qnames/tests/nextflow.config`](https://github.com/nf-core/rnastructurome/blob/605dd9f6f14dfb0d802bb2994cbef0393c8797e1/modules/local/samtools/qnames/tests/nextflow.config#L3) — 1 reference
- [`modules/local/viennarna/tests/nextflow.config`](https://github.com/nf-core/rnastructurome/blob/605dd9f6f14dfb0d802bb2994cbef0393c8797e1/modules/local/viennarna/tests/nextflow.config#L4) — 1 reference
- [`modules/nf-core/rseqc/inferexperiment/tests/nextflow.config`](https://github.com/nf-core/rnastructurome/blob/605dd9f6f14dfb0d802bb2994cbef0393c8797e1/modules/nf-core/rseqc/inferexperiment/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/rnastructurome/blob/605dd9f6f14dfb0d802bb2994cbef0393c8797e1/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
