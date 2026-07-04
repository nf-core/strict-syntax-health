# Workflow outputs migration: raredisease

- Generated: 2026-07-04T00:35:35.695986+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:995`](https://github.com/nf-core/raredisease/blob/161b90cc708a4360f490cd39fb10c67152cbfd5a/main.nf#L995)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/161b90cc708a4360f490cd39fb10c67152cbfd5a/conf/base.config#L65) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/161b90cc708a4360f490cd39fb10c67152cbfd5a/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
