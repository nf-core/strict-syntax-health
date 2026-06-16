# Workflow outputs migration: genephylomodeler

- Generated: 2026-06-16T14:17:41.732361+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 12 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/genephylomodeler/blob/c812faefe0574c87ceab07bee654cb0052225872/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:34`](https://github.com/nf-core/genephylomodeler/blob/c812faefe0574c87ceab07bee654cb0052225872/conf/modules.config#L34)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:42`](https://github.com/nf-core/genephylomodeler/blob/c812faefe0574c87ceab07bee654cb0052225872/conf/modules.config#L42)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:50`](https://github.com/nf-core/genephylomodeler/blob/c812faefe0574c87ceab07bee654cb0052225872/conf/modules.config#L50)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:58`](https://github.com/nf-core/genephylomodeler/blob/c812faefe0574c87ceab07bee654cb0052225872/conf/modules.config#L58)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:66`](https://github.com/nf-core/genephylomodeler/blob/c812faefe0574c87ceab07bee654cb0052225872/conf/modules.config#L66)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:74`](https://github.com/nf-core/genephylomodeler/blob/c812faefe0574c87ceab07bee654cb0052225872/conf/modules.config#L74)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:83`](https://github.com/nf-core/genephylomodeler/blob/c812faefe0574c87ceab07bee654cb0052225872/conf/modules.config#L83)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:91`](https://github.com/nf-core/genephylomodeler/blob/c812faefe0574c87ceab07bee654cb0052225872/conf/modules.config#L91)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:100`](https://github.com/nf-core/genephylomodeler/blob/c812faefe0574c87ceab07bee654cb0052225872/conf/modules.config#L100)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:108`](https://github.com/nf-core/genephylomodeler/blob/c812faefe0574c87ceab07bee654cb0052225872/conf/modules.config#L108)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:116`](https://github.com/nf-core/genephylomodeler/blob/c812faefe0574c87ceab07bee654cb0052225872/conf/modules.config#L116)

  ```nextflow
  publishDir = [
  ```
