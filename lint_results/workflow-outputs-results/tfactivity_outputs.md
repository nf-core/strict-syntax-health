# Workflow outputs migration: tfactivity

- Generated: 2026-06-16T14:37:28.762999+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 76 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:20`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L20)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:28`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L28)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:37`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:45`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:53`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L53)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:65`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L65)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:73`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L73)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:81`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L81)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:89`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L89)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:97`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L97)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:105`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L105)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:117`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L117)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:125`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L125)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:133`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L133)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:141`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L141)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:149`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L149)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:157`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L157)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:172`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L172)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:183`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L183)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:191`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L191)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:202`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L202)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:212`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L212)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:222`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L222)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:233`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L233)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:243`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L243)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:255`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L255)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:263`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L263)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:271`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L271)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:279`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L279)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:287`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L287)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:295`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L295)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:305`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L305)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:313`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L313)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:325`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L325)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:336`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L336)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:344`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L344)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:355`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L355)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:366`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L366)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:377`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L377)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:388`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L388)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:396`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L396)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:407`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L407)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:419`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L419)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:428`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L428)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:436`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L436)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:444`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L444)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:452`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L452)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:460`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L460)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:472`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L472)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:483`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L483)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:495`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L495)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:507`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L507)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:515`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L515)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:525`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L525)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:533`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L533)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:543`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L543)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:551`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L551)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:559`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L559)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:571`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L571)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:579`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L579)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:587`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L587)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:596`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L596)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:605`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L605)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:614`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L614)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:622`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L622)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:633`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L633)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:645`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L645)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:656`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L656)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:664`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L664)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:674`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L674)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:686`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L686)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:694`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L694)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:706`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L706)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:712`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L712)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:718`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/conf/modules.config#L718)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:87`](https://github.com/nf-core/tfactivity/blob/4ac627e7439087a4a8be3dfe7bcb6f6ed55a3d1d/nextflow.config#L87)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
