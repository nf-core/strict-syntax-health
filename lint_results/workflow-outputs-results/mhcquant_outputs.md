# Workflow outputs migration: mhcquant

- Generated: 2026-06-16T14:23:16.948289+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 47 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:34`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L34)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:42`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L42)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:50`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L50)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:58`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L58)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:68`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L68)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:79`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L79)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:87`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L87)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:119`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L119)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:132`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L132)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:142`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L142)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:152`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L152)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:165`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L165)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:181`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L181)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:195`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L195)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:204`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L204)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:210`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L210)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:222`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L222)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:237`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L237)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:247`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L247)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:253`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L253)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:259`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L259)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:266`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L266)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:282`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L282)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:296`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L296)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:313`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L313)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:321`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L321)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:330`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L330)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`conf/modules.config:334`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L334)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:340`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L340)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:350`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L350)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:359`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L359)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:370`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L370)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:383`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L383)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:404`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L404)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:423`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L423)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:429`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L429)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:438`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L438)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:453`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L453)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:461`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L461)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:469`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L469)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:496`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L496)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:517`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L517)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:526`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L526)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:534`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L534)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:550`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/conf/modules.config#L550)

  ```nextflow
  publishDir  = [
  ```

- [`nextflow.config:118`](https://github.com/nf-core/mhcquant/blob/fd72a07e3356c386bed506e920a2d8b8fe3a8d9a/nextflow.config#L118)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
