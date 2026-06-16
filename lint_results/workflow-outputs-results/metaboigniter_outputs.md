# Workflow outputs migration: metaboigniter

- Generated: 2026-06-16T14:22:09.769478+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 31 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:43`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L43)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:55`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L55)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:99`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L99)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:141`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L141)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:179`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L179)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:219`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L219)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:252`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L252)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:295`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L295)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:318`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L318)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:334`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L334)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:353`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L353)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:371`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L371)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:406`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L406)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:422`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L422)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:438`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L438)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:453`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L453)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:468`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L468)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:490`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L490)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:516`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L516)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:561`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L561)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:579`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L579)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:597`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L597)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:615`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L615)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:629`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L629)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:646`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L646)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:663`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L663)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:681`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L681)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:699`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L699)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:716`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L716)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:733`](https://github.com/nf-core/metaboigniter/blob/6239953247efcf1d7c69ed6986227584470bd8db/conf/modules.config#L733)

  ```nextflow
  publishDir = [
  ```
