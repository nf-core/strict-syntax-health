# Workflow outputs migration: hicar

- Generated: 2026-06-16T14:19:35.869039+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 157 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:14`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L14)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:21`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L21)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:39`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:48`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:56`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L56)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:62`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L62)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:69`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L69)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:75`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L75)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:82`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L82)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:88`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L88)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:97`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L97)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:105`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L105)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:113`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L113)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:121`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L121)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:130`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L130)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:137`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L137)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:145`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L145)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:152`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L152)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:161`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L161)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:167`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L167)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:173`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L173)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:178`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L178)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:184`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L184)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:190`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L190)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:196`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L196)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:202`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L202)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:212`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L212)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:225`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L225)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:230`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L230)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:237`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L237)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:244`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L244)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:251`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L251)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:258`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L258)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:265`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L265)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:277`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L277)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:285`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L285)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:292`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L292)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:300`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L300)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:306`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L306)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:312`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L312)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:319`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L319)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:325`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L325)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:331`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L331)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:339`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L339)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:346`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L346)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:352`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L352)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:359`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L359)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:366`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L366)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:373`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L373)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:381`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L381)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:393`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L393)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:400`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L400)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:406`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L406)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:413`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L413)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:421`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L421)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:429`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L429)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:435`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L435)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:440`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L440)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:446`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L446)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:453`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L453)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:466`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L466)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:472`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L472)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:479`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L479)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:485`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L485)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:501`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L501)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:508`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L508)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:516`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L516)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:523`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L523)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:530`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L530)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:536`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L536)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:541`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L541)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:549`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L549)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:556`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L556)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:562`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L562)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:567`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L567)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:578`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L578)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:590`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L590)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:595`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L595)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:601`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L601)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:606`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L606)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:612`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L612)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:618`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L618)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:624`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L624)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:629`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L629)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:638`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L638)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:653`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L653)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:659`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L659)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:666`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L666)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:674`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L674)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:682`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L682)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:693`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L693)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:702`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L702)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:713`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L713)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:718`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L718)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:729`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L729)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:735`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L735)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:743`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L743)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:751`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L751)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:758`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L758)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:763`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L763)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:770`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L770)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:777`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L777)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:785`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L785)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:797`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L797)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:805`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L805)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:813`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L813)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:820`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L820)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:827`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L827)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:840`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L840)

  ```nextflow
  //    publishDir  = [
  ```

- [`conf/modules.config:849`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L849)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:857`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L857)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:866`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L866)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:875`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L875)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:884`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L884)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:891`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L891)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:899`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L899)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:905`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L905)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:913`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L913)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:921`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L921)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:929`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L929)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:936`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L936)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:944`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L944)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:953`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L953)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:962`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L962)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:974`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L974)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:982`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L982)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:989`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L989)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:997`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L997)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1011`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1011)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1018`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1018)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1024`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1024)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1031`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1031)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1038`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1038)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1044`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1044)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1051`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1051)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1058`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1058)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1063`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1063)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1070`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1070)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1075`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1075)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1082`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1082)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1088`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1088)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1095`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1095)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1102`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1102)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1115`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1115)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1123`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1123)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1131`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1131)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1140`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1140)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1150`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1150)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1158`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1158)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1166`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1166)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1178`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1178)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1188`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1188)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1199`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1199)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1206`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1206)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1214`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1214)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:1222`](https://github.com/nf-core/hicar/blob/d2d17a924e42d6f88640b79d48d8b332f33a953f/conf/modules.config#L1222)

  ```nextflow
  publishDir  = [
  ```
