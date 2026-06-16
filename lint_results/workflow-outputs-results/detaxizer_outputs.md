# Workflow outputs migration: detaxizer

- Generated: 2026-06-16T14:14:00.184360+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 20 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:49`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L49)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:61`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L61)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:70`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:83`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L83)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:96`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L96)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:109`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L109)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:118`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L118)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:127`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L127)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:137`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L137)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:151`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L151)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:160`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L160)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:169`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L169)

  ```nextflow
  publishDir = [[
  ```

- [`conf/modules.config:186`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L186)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:197`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L197)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:206`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L206)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:215`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L215)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:224`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L224)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:234`](https://github.com/nf-core/detaxizer/blob/e352a73bf1d8b3d0fb884aa2baf15dc29f43775e/conf/modules.config#L234)

  ```nextflow
  publishDir = [
  ```
