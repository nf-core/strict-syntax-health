# Workflow outputs migration: proteinfamilies

- Generated: 2026-10-10T00:23:46.433605+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:181`](https://github.com/nf-core/proteinfamilies/blob/5ff3c558d7968b1a58949587e1e2d484dd1c8e4b/main.nf#L181)

## Legacy `publishDir` references

Found 81 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/proteinfamilies/blob/5ff3c558d7968b1a58949587e1e2d484dd1c8e4b/conf/modules.config#L15) — 79 references
- [`modules/nf-core/mmseqs/cluster/tests/nextflow.config`](https://github.com/nf-core/proteinfamilies/blob/5ff3c558d7968b1a58949587e1e2d484dd1c8e4b/modules/nf-core/mmseqs/cluster/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/mmseqs/linclust/tests/nextflow.config`](https://github.com/nf-core/proteinfamilies/blob/5ff3c558d7968b1a58949587e1e2d484dd1c8e4b/modules/nf-core/mmseqs/linclust/tests/nextflow.config#L3) — 1 reference
