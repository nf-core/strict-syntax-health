# Workflow outputs migration: rnavar

- Generated: 2026-11-13T00:17:26.833327+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:223`](https://github.com/nf-core/rnavar/blob/b55365bf1f760ef3e4d35669ed4c05243a1167e9/main.nf#L223)

## Legacy `publishDir` references

Found 33 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/rnavar/blob/b55365bf1f760ef3e4d35669ed4c05243a1167e9/conf/modules.config#L16) — 27 references
- [`conf/modules/annotate.config`](https://github.com/nf-core/rnavar/blob/b55365bf1f760ef3e4d35669ed4c05243a1167e9/conf/modules/annotate.config#L37) — 4 references
- [`conf/modules/prepare_cache.config`](https://github.com/nf-core/rnavar/blob/b55365bf1f760ef3e4d35669ed4c05243a1167e9/conf/modules/prepare_cache.config#L14) — 2 references
