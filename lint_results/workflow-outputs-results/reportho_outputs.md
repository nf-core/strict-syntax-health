# Workflow outputs migration: reportho

- Generated: 2026-06-16T14:30:25.193598+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 37 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:26`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L26)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:37`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:48`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:59`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L59)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:70`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:85`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L85)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:94`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L94)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:103`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L103)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:112`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L112)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:121`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L121)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:130`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L130)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:143`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L143)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:155`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L155)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:168`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L168)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:183`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L183)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:196`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L196)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:206`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L206)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:220`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L220)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:233`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L233)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:257`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L257)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:272`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L272)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:284`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L284)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:299`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L299)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:311`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L311)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:324`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L324)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:332`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L332)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:341`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L341)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:349`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L349)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:363`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L363)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:371`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L371)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:385`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L385)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:393`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L393)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:402`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L402)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:416`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L416)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:428`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L428)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:437`](https://github.com/nf-core/reportho/blob/de4ba462df58d43eb438ea529074519edbb9058f/conf/modules.config#L437)

  ```nextflow
  publishDir = [
  ```
