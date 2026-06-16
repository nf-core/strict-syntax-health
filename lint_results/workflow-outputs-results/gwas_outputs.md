# Workflow outputs migration: gwas

- Generated: 2026-06-16T14:18:59.154465+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 3 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/gwas/blob/2e6660aa8db59c674df4a70a25449cf2aedc630c/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/gwas/blob/2e6660aa8db59c674df4a70a25449cf2aedc630c/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/gwas/blob/2e6660aa8db59c674df4a70a25449cf2aedc630c/conf/modules.config#L32)

  ```nextflow
  publishDir = [
  ```
