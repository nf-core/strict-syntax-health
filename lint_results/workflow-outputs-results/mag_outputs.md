# Workflow outputs migration: mag

- Generated: 2026-11-24T00:12:04.332452+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:382`](https://github.com/nf-core/mag/blob/4b845c844d41602508c2d926af7953c2776c2dbd/main.nf#L382)

## Legacy `publishDir` references

Found 1 `publishDir` reference across 1 file that should be migrated to the workflow `output {}` block:

- [`modules/nf-core/dastool/dastool/tests/nextflow.config`](https://github.com/nf-core/mag/blob/4b845c844d41602508c2d926af7953c2776c2dbd/modules/nf-core/dastool/dastool/tests/nextflow.config#L3) — 1 reference
