# Workflow outputs migration: denovotranscript

- Generated: 2026-06-16T14:13:53.043900+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 7 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/denovotranscript/blob/c5f4e32a1c444762e45bc8a2d69d21af4d91dd54/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:25`](https://github.com/nf-core/denovotranscript/blob/c5f4e32a1c444762e45bc8a2d69d21af4d91dd54/conf/modules.config#L25)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:35`](https://github.com/nf-core/denovotranscript/blob/c5f4e32a1c444762e45bc8a2d69d21af4d91dd54/conf/modules.config#L35)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:45`](https://github.com/nf-core/denovotranscript/blob/c5f4e32a1c444762e45bc8a2d69d21af4d91dd54/conf/modules.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:61`](https://github.com/nf-core/denovotranscript/blob/c5f4e32a1c444762e45bc8a2d69d21af4d91dd54/conf/modules.config#L61)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:92`](https://github.com/nf-core/denovotranscript/blob/c5f4e32a1c444762e45bc8a2d69d21af4d91dd54/conf/modules.config#L92)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:112`](https://github.com/nf-core/denovotranscript/blob/c5f4e32a1c444762e45bc8a2d69d21af4d91dd54/conf/modules.config#L112)

  ```nextflow
  publishDir = [
  ```
