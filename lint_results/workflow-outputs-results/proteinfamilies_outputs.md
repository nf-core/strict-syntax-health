# Workflow outputs migration: proteinfamilies

- Generated: 2026-08-08T00:16:22.398380+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:106`](https://github.com/nf-core/proteinfamilies/blob/a2b6a091814778459c0508a1918a11b98ce7c734/main.nf#L106)

## Legacy `publishDir` references

Found 79 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/proteinfamilies/blob/a2b6a091814778459c0508a1918a11b98ce7c734/conf/modules.config#L15) — 77 references
- [`modules/nf-core/mmseqs/cluster/tests/nextflow.config`](https://github.com/nf-core/proteinfamilies/blob/a2b6a091814778459c0508a1918a11b98ce7c734/modules/nf-core/mmseqs/cluster/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/mmseqs/linclust/tests/nextflow.config`](https://github.com/nf-core/proteinfamilies/blob/a2b6a091814778459c0508a1918a11b98ce7c734/modules/nf-core/mmseqs/linclust/tests/nextflow.config#L3) — 1 reference
