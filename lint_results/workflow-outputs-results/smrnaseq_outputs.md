# Workflow outputs migration: smrnaseq

- Generated: 2026-11-25T00:17:55.324771+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:248`](https://github.com/nf-core/smrnaseq/blob/7375b116cc7fa4a8491f62b4f0fb65b85ccd72fa/main.nf#L248)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/smrnaseq/blob/7375b116cc7fa4a8491f62b4f0fb65b85ccd72fa/conf/modules.config#L201) — 1 reference
- [`tests/strand_orientation/main.nf`](https://github.com/nf-core/smrnaseq/blob/7375b116cc7fa4a8491f62b4f0fb65b85ccd72fa/tests/strand_orientation/main.nf#L17) — 1 reference
