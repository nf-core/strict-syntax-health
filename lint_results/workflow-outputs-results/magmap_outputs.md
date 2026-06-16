# Workflow outputs migration: magmap

- Generated: 2026-06-16T14:21:36.784150+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 28 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:24`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L24)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:38`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L38)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:53`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L53)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:63`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L63)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:71`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L71)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:83`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L83)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:94`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L94)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:104`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L104)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:113`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L113)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:121`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L121)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:131`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L131)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:140`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L140)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:148`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L148)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:162`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L162)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:179`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L179)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:187`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L187)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:195`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L195)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:204`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L204)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:213`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L213)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:224`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L224)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:233`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L233)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:242`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L242)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:251`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L251)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:259`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L259)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:268`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L268)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/subread/featurecounts/tests/nextflow.config:3`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`nextflow.config:88`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/nextflow.config#L88)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
