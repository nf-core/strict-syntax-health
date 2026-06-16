# Workflow outputs migration: chipseq

- Generated: 2026-06-16T14:10:27.971317+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 57 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:19`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L19)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:27`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:35`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L35)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:43`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L43)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:52`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L52)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:60`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L60)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:70`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:78`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L78)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:87`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L87)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:94`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L94)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:107`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L107)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:132`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L132)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:163`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L163)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:171`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L171)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:180`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L180)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:197`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L197)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:212`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L212)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:228`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L228)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:239`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L239)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:258`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L258)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:286`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L286)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:297`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L297)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:313`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L313)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:323`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L323)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:344`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L344)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:354`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L354)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:363`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L363)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:373`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L373)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:384`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L384)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:394`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L394)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:403`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L403)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:417`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L417)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:425`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L425)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:453`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L453)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:464`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L464)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:478`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L478)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:499`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L499)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:512`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L512)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:520`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L520)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:528`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L528)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:541`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L541)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:560`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L560)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:568`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L568)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:575`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L575)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:589`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L589)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:598`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L598)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:607`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L607)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:620`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L620)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:629`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L629)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:638`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L638)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:647`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L647)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:667`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L667)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:679`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L679)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:699`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/conf/modules.config#L699)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/subread/featurecounts/tests/nextflow.config:3`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/umitools/extract/tests/nextflow.config:3`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/modules/nf-core/umitools/extract/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`nextflow.config:105`](https://github.com/nf-core/chipseq/blob/4969914099b0dd3c438a2d5acb1a7ea30dabb494/nextflow.config#L105)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
