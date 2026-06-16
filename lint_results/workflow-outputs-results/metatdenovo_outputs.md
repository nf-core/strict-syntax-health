# Workflow outputs migration: metatdenovo

- Generated: 2026-06-16T14:22:25.762459+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 39 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:13`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L13)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:29`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L29)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:52`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L52)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:68`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L68)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:84`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L84)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:92`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L92)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:101`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L101)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:109`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L109)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:123`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L123)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:143`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L143)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:167`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L167)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:175`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L175)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:183`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L183)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:193`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L193)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:207`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L207)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:216`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L216)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:225`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L225)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:233`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L233)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:243`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L243)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:251`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L251)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:260`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L260)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:269`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L269)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:277`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L277)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:290`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L290)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:310`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L310)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:332`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L332)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:341`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L341)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:349`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L349)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:358`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L358)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:365`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L365)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:373`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L373)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:382`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L382)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:392`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L392)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:410`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L410)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:419`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L419)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:428`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L428)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:437`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/conf/modules.config#L437)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/subread/featurecounts/tests/nextflow.config:3`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`nextflow.config:114`](https://github.com/nf-core/metatdenovo/blob/2be548eabe0f1a1932e8c11e85830c1175dd7f68/nextflow.config#L114)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
