# Workflow outputs migration: smrnaseq

- Generated: 2026-11-28T00:14:25.918511+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:249`](https://github.com/nf-core/smrnaseq/blob/a5f502ee2095f81cdbe943057b800fa46863f440/main.nf#L249)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/smrnaseq/blob/a5f502ee2095f81cdbe943057b800fa46863f440/conf/modules.config#L192) — 1 reference
- [`tests/strand_orientation/main.nf`](https://github.com/nf-core/smrnaseq/blob/a5f502ee2095f81cdbe943057b800fa46863f440/tests/strand_orientation/main.nf#L17) — 1 reference
