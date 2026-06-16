# Workflow outputs migration: hgtseq

- Generated: 2026-06-16T14:19:20.330078+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 50 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:20`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L20)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:29`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L29)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:38`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L38)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:54`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L54)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:61`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L61)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:68`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L68)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:76`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L76)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:83`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L83)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:91`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L91)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:98`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L98)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:107`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L107)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:115`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L115)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:123`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L123)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:131`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L131)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:138`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L138)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:145`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L145)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:152`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L152)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:159`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L159)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:166`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L166)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:174`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L174)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:182`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L182)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:192`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L192)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:201`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L201)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:209`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/conf/modules.config#L209)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:16`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:21`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L21)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:30`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:39`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:55`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L55)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:62`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L62)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:69`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L69)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:77`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L77)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:84`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L84)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:92`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L92)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:99`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L99)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:108`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L108)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:116`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L116)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:124`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L124)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:132`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L132)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:139`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L139)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:146`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L146)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:153`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L153)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:160`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L160)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:167`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L167)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:175`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L175)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:183`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L183)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:193`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L193)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:202`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L202)

  ```nextflow
  publishDir = [
  ```

- [`tests/nextflow.config:210`](https://github.com/nf-core/hgtseq/blob/b2b144902c2ec92cfb2c898777b293093f0d4be5/tests/nextflow.config#L210)

  ```nextflow
  publishDir = [
  ```
