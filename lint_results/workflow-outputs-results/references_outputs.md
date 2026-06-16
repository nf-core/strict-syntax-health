# Workflow outputs migration: references

- Generated: 2026-06-16T14:30:08.167504+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:308`](https://github.com/nf-core/references/blob/b205e5bc23ad11c224dfea9d25ab9d07b26660d7/main.nf#L308)

  ```nextflow
  output {
  ```

## Legacy `publishDir` references

Found 1 `publishDir` reference that should be migrated to the workflow `output {}` block:

- [`nextflow.config:56`](https://github.com/nf-core/references/blob/b205e5bc23ad11c224dfea9d25ab9d07b26660d7/nextflow.config#L56)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
