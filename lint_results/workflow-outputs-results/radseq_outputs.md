# Workflow outputs migration: radseq

- Generated: 2026-06-16T14:28:57.681159+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 54 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:35`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L35)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:58`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L58)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:91`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L91)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:114`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L114)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:123`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L123)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:133`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L133)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:143`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L143)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:166`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L166)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:184`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L184)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:212`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L212)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:237`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L237)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:254`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L254)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:263`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L263)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:277`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L277)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:291`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L291)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:301`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L301)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:311`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L311)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:321`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L321)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:332`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L332)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:346`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L346)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:361`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L361)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:372`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L372)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:382`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L382)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:399`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L399)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:428`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L428)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:440`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L440)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:458`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L458)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:469`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L469)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:479`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L479)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:489`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L489)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:499`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L499)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:510`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L510)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:522`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L522)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:535`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L535)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:547`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L547)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:559`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L559)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:572`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L572)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:596`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L596)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:609`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L609)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:623`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L623)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:644`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L644)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:657`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L657)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:669`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L669)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:681`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L681)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:693`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L693)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:705`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L705)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:719`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L719)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:730`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L730)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:742`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L742)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:761`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L761)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:779`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L779)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:790`](https://github.com/nf-core/radseq/blob/26ff6763ac5d6e5d9306ed262efc8e002c08bb7f/conf/modules.config#L790)

  ```nextflow
  publishDir = [
  ```
