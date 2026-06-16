# Workflow outputs migration: funcscan

- Generated: 2026-06-16T14:17:24.088925+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 63 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:37`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:50`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L50)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:62`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L62)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:82`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L82)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:96`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L96)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:109`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L109)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:121`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L121)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:131`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L131)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:149`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L149)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:172`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L172)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:185`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L185)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:215`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L215)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:232`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L232)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:249`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L249)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:262`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L262)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:271`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L271)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:288`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L288)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:297`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L297)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:314`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L314)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:356`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L356)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:367`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L367)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:378`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L378)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:413`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L413)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:422`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L422)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:431`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L431)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:441`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L441)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:451`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L451)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:460`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L460)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:485`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L485)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:494`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L494)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:503`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L503)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:522`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L522)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:537`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L537)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:552`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L552)

  ```nextflow
  publishDir    = [
  ```

- [`conf/modules.config:560`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L560)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:568`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L568)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:577`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L577)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:586`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L586)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:595`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L595)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:604`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L604)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:613`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L613)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:621`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L621)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:630`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L630)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:638`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L638)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:660`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L660)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:676`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L676)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:702`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L702)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:710`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L710)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:718`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L718)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:726`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L726)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:736`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L736)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:746`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L746)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:756`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L756)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:764`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L764)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:772`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L772)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:781`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L781)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:790`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L790)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:798`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L798)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:807`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/conf/modules.config#L807)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:287`](https://github.com/nf-core/funcscan/blob/00686cdc522e2a1c750b0edff04f06ddb26b5ea1/nextflow.config#L287)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
