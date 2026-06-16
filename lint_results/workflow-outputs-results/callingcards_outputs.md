# Workflow outputs migration: callingcards

- Generated: 2026-06-16T20:18:20.712913+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 38 `publishDir` references across 7 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L15) — 32 references
- [`modules/nf-core/rseqc/bamstat/tests/nextflow.config`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/modules/nf-core/rseqc/bamstat/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/rseqc/inferexperiment/tests/nextflow.config`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/modules/nf-core/rseqc/inferexperiment/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/rseqc/innerdistance/tests/nextflow.config`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/modules/nf-core/rseqc/innerdistance/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
- [`subworkflows/nf-core/fastq_align_bwaaln/nextflow.config`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/subworkflows/nf-core/fastq_align_bwaaln/nextflow.config#L7) — 1 reference
