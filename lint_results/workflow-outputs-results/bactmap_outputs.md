# Workflow outputs migration: bactmap

- Generated: 2026-06-16T14:09:32.869433+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 53 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:29`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L29)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:36`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L36)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:45`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:54`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L54)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:64`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L64)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:74`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L74)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:83`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L83)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:92`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L92)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:107`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L107)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:139`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L139)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:167`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L167)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:197`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L197)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:222`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L222)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:235`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L235)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:259`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L259)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:288`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L288)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:317`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L317)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:341`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L341)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:350`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L350)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:359`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L359)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:367`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L367)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:376`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L376)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:395`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L395)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:406`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L406)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:416`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L416)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:425`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L425)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:434`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L434)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:443`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L443)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:452`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L452)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:461`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L461)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:471`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L471)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:480`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L480)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:490`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L490)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:499`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L499)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:509`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L509)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:519`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L519)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:531`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L531)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:541`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L541)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:552`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L552)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:562`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L562)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:572`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L572)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:582`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L582)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:592`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L592)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:602`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L602)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:612`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L612)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:620`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L620)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:629`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L629)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:638`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L638)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:647`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L647)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:656`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L656)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:665`](https://github.com/nf-core/bactmap/blob/3f2b135db97d1e9172a5326312616cfc762c7f60/conf/modules.config#L665)

  ```nextflow
  publishDir = [
  ```
