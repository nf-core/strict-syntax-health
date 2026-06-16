# Workflow outputs migration: multiplesequencealign

- Generated: 2026-06-16T14:24:14.284050+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 18 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:20`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L20)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:45`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:59`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L59)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:79`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L79)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:104`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L104)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:123`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L123)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:143`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L143)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:162`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L162)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:174`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L174)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:200`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L200)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:227`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L227)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:261`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L261)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:271`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L271)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:285`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L285)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:296`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L296)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:308`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/conf/modules.config#L308)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:97`](https://github.com/nf-core/multiplesequencealign/blob/1fd8bda62787418bff4c2df9dbff4561e888dadc/nextflow.config#L97)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
