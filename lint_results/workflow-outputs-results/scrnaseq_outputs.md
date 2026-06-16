# Workflow outputs migration: scrnaseq

- Generated: 2026-06-16T14:34:41.619370+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 26 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:14`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L14)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:28`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L28)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:36`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L36)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:45`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:53`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L53)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:65`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L65)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:77`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L77)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:81`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L81)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:90`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L90)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:98`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L98)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:108`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L108)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:117`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L117)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:124`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L124)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:133`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L133)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:143`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L143)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:157`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L157)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:166`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L166)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:174`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L174)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:183`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L183)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:192`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L192)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:203`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L203)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:211`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L211)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:217`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/conf/modules.config#L217)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/parse_cellrangermulti_samplesheet/main.nf:8`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/modules/local/parse_cellrangermulti_samplesheet/main.nf#L8)

  ```nextflow
  publishDir enabled: false
  ```

- [`modules/nf-core/cellranger/mkref/tests/nextflow.config:3`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/modules/nf-core/cellranger/mkref/tests/nextflow.config#L3)

  ```nextflow
  publishDir = [ path: { "output" } ]
  ```

- [`nextflow.config:109`](https://github.com/nf-core/scrnaseq/blob/de2c003b695a868ec657e96b75117a1e83adb387/nextflow.config#L109)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
