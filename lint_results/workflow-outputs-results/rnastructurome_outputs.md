# Workflow outputs migration: rnastructurome

- Generated: 2026-07-28T00:34:45.394521+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 53 `publishDir` references across 7 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/rnastructurome/blob/2678cdd9f6a82c25d62b0ba1d4f862167064c464/conf/modules.config#L14) — 47 references
- [`modules/local/r2dt/tests/nextflow.config`](https://github.com/nf-core/rnastructurome/blob/2678cdd9f6a82c25d62b0ba1d4f862167064c464/modules/local/r2dt/tests/nextflow.config#L4) — 1 reference
- [`modules/local/rnaframework/fold/tests/nextflow.config`](https://github.com/nf-core/rnastructurome/blob/2678cdd9f6a82c25d62b0ba1d4f862167064c464/modules/local/rnaframework/fold/tests/nextflow.config#L4) — 1 reference
- [`modules/local/samtools/qnames/tests/nextflow.config`](https://github.com/nf-core/rnastructurome/blob/2678cdd9f6a82c25d62b0ba1d4f862167064c464/modules/local/samtools/qnames/tests/nextflow.config#L3) — 1 reference
- [`modules/local/viennarna/tests/nextflow.config`](https://github.com/nf-core/rnastructurome/blob/2678cdd9f6a82c25d62b0ba1d4f862167064c464/modules/local/viennarna/tests/nextflow.config#L4) — 1 reference
- [`modules/nf-core/rseqc/inferexperiment/tests/nextflow.config`](https://github.com/nf-core/rnastructurome/blob/2678cdd9f6a82c25d62b0ba1d4f862167064c464/modules/nf-core/rseqc/inferexperiment/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/rnastructurome/blob/2678cdd9f6a82c25d62b0ba1d4f862167064c464/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
