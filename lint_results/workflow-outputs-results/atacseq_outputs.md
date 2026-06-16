# Workflow outputs migration: atacseq

- Generated: 2026-06-16T14:08:34.100106+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 80 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:18`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L18)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:45`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:55`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L55)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:64`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L64)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:74`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L74)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:83`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L83)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:92`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L92)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:101`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L101)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:110`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L110)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:119`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L119)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:128`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L128)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:139`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L139)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:166`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L166)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:195`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L195)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:205`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L205)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:215`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L215)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:235`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L235)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:253`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L253)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:272`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L272)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:287`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L287)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:308`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L308)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:334`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L334)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:345`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L345)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:361`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L361)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:371`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L371)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:387`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L387)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:397`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L397)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:406`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L406)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:416`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L416)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:427`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L427)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:437`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L437)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:446`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L446)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:460`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L460)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:470`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L470)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:480`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L480)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:491`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L491)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:507`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L507)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:519`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L519)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:538`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L538)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:550`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L550)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:560`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L560)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:569`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L569)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:578`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L578)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:596`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L596)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:615`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L615)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:624`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L624)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:632`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L632)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:644`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L644)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:655`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L655)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:665`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L665)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:677`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L677)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:687`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L687)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:704`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L704)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:716`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L716)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:727`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L727)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:734`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L734)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:746`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L746)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:757`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L757)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:772`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L772)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:781`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L781)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:791`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L791)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:801`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L801)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:811`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L811)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:822`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L822)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:838`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L838)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:857`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L857)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:866`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L866)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:874`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L874)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:886`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L886)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:897`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L897)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:907`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L907)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:918`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L918)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:928`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L928)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:945`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L945)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:957`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L957)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:967`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L967)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:985`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/conf/modules.config#L985)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/umitools/extract/tests/nextflow.config:3`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/modules/nf-core/umitools/extract/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`nextflow.config:115`](https://github.com/nf-core/atacseq/blob/487128bfe873ccd75c2f19563ddbb5ef63ad0e39/nextflow.config#L115)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
