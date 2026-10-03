# Workflow outputs migration: proteinfamilies

- Generated: 2026-10-03T00:24:09.215696+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:106`](https://github.com/nf-core/proteinfamilies/blob/03fc799bdcb341b05e611cac68fca1a9b4993144/main.nf#L106)

## Legacy `publishDir` references

Found 78 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/proteinfamilies/blob/03fc799bdcb341b05e611cac68fca1a9b4993144/conf/modules.config#L15) — 76 references
- [`modules/nf-core/mmseqs/cluster/tests/nextflow.config`](https://github.com/nf-core/proteinfamilies/blob/03fc799bdcb341b05e611cac68fca1a9b4993144/modules/nf-core/mmseqs/cluster/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/mmseqs/linclust/tests/nextflow.config`](https://github.com/nf-core/proteinfamilies/blob/03fc799bdcb341b05e611cac68fca1a9b4993144/modules/nf-core/mmseqs/linclust/tests/nextflow.config#L3) — 1 reference
