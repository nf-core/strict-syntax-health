# Workflow outputs migration: genomeskim

- Generated: 2026-06-16T14:18:34.319974+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 3 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/genomeskim/blob/0c969583df4a65daf62c2bfb6e2dcd9ead4e850a/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/genomeskim/blob/0c969583df4a65daf62c2bfb6e2dcd9ead4e850a/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:34`](https://github.com/nf-core/genomeskim/blob/0c969583df4a65daf62c2bfb6e2dcd9ead4e850a/conf/modules.config#L34)

  ```nextflow
  publishDir = [
  ```
