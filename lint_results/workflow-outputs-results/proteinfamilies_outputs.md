# Workflow outputs migration: proteinfamilies

- Generated: 2026-10-06T00:22:43.771202+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:108`](https://github.com/nf-core/proteinfamilies/blob/f44e15e43178a6cf72c9756134017715dc9d2c3b/main.nf#L108)

## Legacy `publishDir` references

Found 84 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/proteinfamilies/blob/f44e15e43178a6cf72c9756134017715dc9d2c3b/conf/modules.config#L15) — 82 references
- [`modules/nf-core/mmseqs/cluster/tests/nextflow.config`](https://github.com/nf-core/proteinfamilies/blob/f44e15e43178a6cf72c9756134017715dc9d2c3b/modules/nf-core/mmseqs/cluster/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/mmseqs/linclust/tests/nextflow.config`](https://github.com/nf-core/proteinfamilies/blob/f44e15e43178a6cf72c9756134017715dc9d2c3b/modules/nf-core/mmseqs/linclust/tests/nextflow.config#L3) — 1 reference
