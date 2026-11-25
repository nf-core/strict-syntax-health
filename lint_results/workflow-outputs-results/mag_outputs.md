# Workflow outputs migration: mag

- Generated: 2026-11-25T00:13:05.376350+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:381`](https://github.com/nf-core/mag/blob/a1c1c10438e055c8fb7b614685d2d87928141fa5/main.nf#L381)

## Legacy `publishDir` references

Found 1 `publishDir` reference across 1 file that should be migrated to the workflow `output {}` block:

- [`modules/nf-core/dastool/dastool/tests/nextflow.config`](https://github.com/nf-core/mag/blob/a1c1c10438e055c8fb7b614685d2d87928141fa5/modules/nf-core/dastool/dastool/tests/nextflow.config#L3) — 1 reference
