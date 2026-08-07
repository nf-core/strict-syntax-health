# Workflow outputs migration: raredisease

- Generated: 2026-08-07T01:16:03.762428+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:1035`](https://github.com/nf-core/raredisease/blob/154b4331e2408a29e2abb9de3e0d227df5f1d61e/main.nf#L1035)

## Legacy `publishDir` references

Found 2 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/base.config`](https://github.com/nf-core/raredisease/blob/154b4331e2408a29e2abb9de3e0d227df5f1d61e/conf/base.config#L65) — 1 reference
- [`modules/nf-core/spring/decompress/tests/nextflow.config`](https://github.com/nf-core/raredisease/blob/154b4331e2408a29e2abb9de3e0d227df5f1d61e/modules/nf-core/spring/decompress/tests/nextflow.config#L3) — 1 reference
