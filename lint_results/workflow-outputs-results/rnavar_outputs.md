# Workflow outputs migration: rnavar

- Generated: 2026-06-16T19:41:15.067284+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:223`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/main.nf#L223)

## Legacy `publishDir` references

Found 33 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L16) — 27 references
- [`conf/modules/annotate.config`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules/annotate.config#L37) — 4 references
- [`conf/modules/prepare_cache.config`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules/prepare_cache.config#L14) — 2 references
