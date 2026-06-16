# Workflow outputs migration: pathogensurveillance

- Generated: 2026-06-16T14:26:35.841286+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 52 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:16`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:26`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L26)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:45`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:64`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L64)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:75`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L75)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:88`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L88)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:100`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L100)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:118`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L118)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:131`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L131)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:144`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L144)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:155`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L155)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:167`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L167)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:175`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L175)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:199`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L199)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:212`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L212)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:227`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L227)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:249`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L249)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:262`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L262)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:273`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L273)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:283`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L283)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:296`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L296)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:310`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L310)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:322`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L322)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:334`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L334)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:346`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L346)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:358`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L358)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:372`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L372)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:382`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L382)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:391`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L391)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:399`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L399)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:408`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L408)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:420`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L420)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:431`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L431)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:444`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L444)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:461`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L461)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:469`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L469)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:480`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L480)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:486`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L486)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:499`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L499)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:507`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L507)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:516`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L516)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:525`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L525)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:533`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L533)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:547`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L547)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:559`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L559)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:572`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L572)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:591`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L591)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:600`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L600)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:609`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L609)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:618`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L618)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:637`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L637)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:648`](https://github.com/nf-core/pathogensurveillance/blob/f9a0d73b990e050f13545c071f9eb7d16ca683e1/conf/modules.config#L648)

  ```nextflow
  publishDir = [
  ```
