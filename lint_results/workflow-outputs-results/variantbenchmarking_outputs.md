# Workflow outputs migration: variantbenchmarking

- Generated: 2026-06-16T14:38:09.828364+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 80 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:34`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L34)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:42`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L42)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:51`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L51)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:67`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L67)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:78`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L78)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:87`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L87)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:94`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L94)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:102`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L102)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:110`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L110)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:120`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L120)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:130`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L130)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:137`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L137)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:145`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L145)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:153`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L153)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:159`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L159)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:169`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L169)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:178`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L178)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:185`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L185)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:197`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L197)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:206`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L206)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:215`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L215)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:224`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L224)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:237`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L237)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:243`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L243)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:250`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L250)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:260`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L260)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:268`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L268)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:277`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L277)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:285`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L285)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:293`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L293)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:302`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L302)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:309`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L309)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:318`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L318)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:324`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L324)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:334`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L334)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:348`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L348)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:360`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L360)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:370`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L370)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:384`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L384)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:394`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L394)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:404`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L404)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:414`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L414)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:424`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L424)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:433`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L433)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:441`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L441)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:458`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L458)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:473`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L473)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:482`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L482)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:492`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L492)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:499`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L499)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:506`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L506)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:513`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L513)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:521`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L521)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:528`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L528)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:543`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L543)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:561`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L561)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:570`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L570)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:576`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L576)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:584`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L584)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:592`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L592)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:600`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L600)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:608`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L608)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:616`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L616)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:624`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L624)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:633`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L633)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:642`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L642)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:651`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L651)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:662`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L662)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:669`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L669)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:680`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L680)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:687`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L687)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:696`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L696)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:704`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L704)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:711`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L711)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:720`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L720)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:730`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L730)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:737`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/conf/modules.config#L737)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:98`](https://github.com/nf-core/variantbenchmarking/blob/4d07dcda08ddcce51933018df2c9daec8479bbc1/nextflow.config#L98)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
