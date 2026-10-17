# Workflow outputs migration: proteinfamilies

- Generated: 2026-10-17T00:21:15.629173+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:181`](https://github.com/nf-core/proteinfamilies/blob/700d0e1f497651a9abdc5cac78bcd0df656b8414/main.nf#L181)

## Legacy `publishDir` references

Found 81 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/proteinfamilies/blob/700d0e1f497651a9abdc5cac78bcd0df656b8414/conf/modules.config#L15) — 79 references
- [`modules/nf-core/mmseqs/cluster/tests/nextflow.config`](https://github.com/nf-core/proteinfamilies/blob/700d0e1f497651a9abdc5cac78bcd0df656b8414/modules/nf-core/mmseqs/cluster/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/mmseqs/linclust/tests/nextflow.config`](https://github.com/nf-core/proteinfamilies/blob/700d0e1f497651a9abdc5cac78bcd0df656b8414/modules/nf-core/mmseqs/linclust/tests/nextflow.config#L3) — 1 reference
