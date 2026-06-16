# Workflow outputs migration: deepmodeloptim

- Generated: 2026-06-16T14:13:00.244413+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 12 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:20`](https://github.com/nf-core/deepmodeloptim/blob/151accd47c04e24cde6fdefc7aa0e371b9ab157a/conf/modules.config#L20)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:29`](https://github.com/nf-core/deepmodeloptim/blob/151accd47c04e24cde6fdefc7aa0e371b9ab157a/conf/modules.config#L29)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:39`](https://github.com/nf-core/deepmodeloptim/blob/151accd47c04e24cde6fdefc7aa0e371b9ab157a/conf/modules.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:49`](https://github.com/nf-core/deepmodeloptim/blob/151accd47c04e24cde6fdefc7aa0e371b9ab157a/conf/modules.config#L49)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:60`](https://github.com/nf-core/deepmodeloptim/blob/151accd47c04e24cde6fdefc7aa0e371b9ab157a/conf/modules.config#L60)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:67`](https://github.com/nf-core/deepmodeloptim/blob/151accd47c04e24cde6fdefc7aa0e371b9ab157a/conf/modules.config#L67)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:75`](https://github.com/nf-core/deepmodeloptim/blob/151accd47c04e24cde6fdefc7aa0e371b9ab157a/conf/modules.config#L75)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:94`](https://github.com/nf-core/deepmodeloptim/blob/151accd47c04e24cde6fdefc7aa0e371b9ab157a/conf/modules.config#L94)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:106`](https://github.com/nf-core/deepmodeloptim/blob/151accd47c04e24cde6fdefc7aa0e371b9ab157a/conf/modules.config#L106)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:117`](https://github.com/nf-core/deepmodeloptim/blob/151accd47c04e24cde6fdefc7aa0e371b9ab157a/conf/modules.config#L117)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:145`](https://github.com/nf-core/deepmodeloptim/blob/151accd47c04e24cde6fdefc7aa0e371b9ab157a/conf/modules.config#L145)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:174`](https://github.com/nf-core/deepmodeloptim/blob/151accd47c04e24cde6fdefc7aa0e371b9ab157a/conf/modules.config#L174)

  ```nextflow
  publishDir = [
  ```
