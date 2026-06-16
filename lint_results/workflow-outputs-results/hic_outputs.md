# Workflow outputs migration: hic

- Generated: 2026-06-16T14:19:28.041079+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 39 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:3`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:19`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L19)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:29`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L29)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:37`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:45`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:56`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L56)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:67`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L67)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:75`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L75)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:86`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L86)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:95`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L95)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:109`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L109)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:126`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L126)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:136`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L136)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:152`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L152)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:160`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L160)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:168`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L168)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:177`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L177)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:188`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L188)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:198`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L198)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:212`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L212)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:220`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L220)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:228`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L228)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:236`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L236)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:247`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L247)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:257`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L257)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:266`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L266)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:277`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L277)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:296`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L296)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:305`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L305)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:316`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L316)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:327`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L327)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:336`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L336)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:347`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L347)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:358`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L358)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:366`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L366)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:382`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L382)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:394`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L394)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:407`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L407)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:417`](https://github.com/nf-core/hic/blob/e0084aec16e0b5c6ce5f11e00a0a995585fde3ed/conf/modules.config#L417)

  ```nextflow
  publishDir = [
  ```
