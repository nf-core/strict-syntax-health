# Workflow outputs migration: seqinspector

- Generated: 2026-06-16T14:35:00.048303+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:128`](https://github.com/nf-core/seqinspector/blob/f3d7f505aa71c17a6943ff13429501e1a029c1ad/main.nf#L128)

  ```nextflow
  output {
  ```

## Legacy `publishDir` references

Found 2 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`nextflow.config:80`](https://github.com/nf-core/seqinspector/blob/f3d7f505aa71c17a6943ff13429501e1a029c1ad/nextflow.config#L80)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```

- [`workflows/seqinspector.nf:102`](https://github.com/nf-core/seqinspector/blob/f3d7f505aa71c17a6943ff13429501e1a029c1ad/workflows/seqinspector.nf#L102)

  ```nextflow
  //     - id: Simple name of the rundir, used for setting unique output names in publishDir
  ```
