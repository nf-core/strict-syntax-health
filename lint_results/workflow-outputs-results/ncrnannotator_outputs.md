# Workflow outputs migration: ncrnannotator

- Generated: 2026-06-16T14:25:01.051959+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 6 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/ncrnannotator/blob/1a57ac306827ace09b52473a1e8f64dcb33c55a5/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:24`](https://github.com/nf-core/ncrnannotator/blob/1a57ac306827ace09b52473a1e8f64dcb33c55a5/conf/modules.config#L24)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/ncrnannotator/blob/1a57ac306827ace09b52473a1e8f64dcb33c55a5/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:40`](https://github.com/nf-core/ncrnannotator/blob/1a57ac306827ace09b52473a1e8f64dcb33c55a5/conf/modules.config#L40)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:49`](https://github.com/nf-core/ncrnannotator/blob/1a57ac306827ace09b52473a1e8f64dcb33c55a5/conf/modules.config#L49)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:58`](https://github.com/nf-core/ncrnannotator/blob/1a57ac306827ace09b52473a1e8f64dcb33c55a5/conf/modules.config#L58)

  ```nextflow
  publishDir = [
  ```
