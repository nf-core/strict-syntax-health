# Workflow outputs migration: createpanelrefs

- Generated: 2026-06-16T14:11:27.528264+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:199`](https://github.com/nf-core/createpanelrefs/blob/57e700eda43dd38c994417260d97ed98952e9d73/main.nf#L199)

  ```nextflow
  output {
  ```

## Legacy `publishDir` references

Found 1 `publishDir` reference that should be migrated to the workflow `output {}` block:

- [`nextflow.config:84`](https://github.com/nf-core/createpanelrefs/blob/57e700eda43dd38c994417260d97ed98952e9d73/nextflow.config#L84)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
