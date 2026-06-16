# Workflow outputs migration: methylong

- Generated: 2026-06-16T14:22:49.716244+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 41 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:17`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:26`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L26)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:66`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L66)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:76`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L76)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:84`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L84)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:98`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L98)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:113`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L113)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:130`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L130)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:139`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L139)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:148`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L148)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:157`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L157)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:171`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L171)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:180`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L180)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:195`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L195)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:204`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L204)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:220`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L220)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:235`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L235)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:248`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L248)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:257`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L257)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:279`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L279)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:301`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L301)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:316`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L316)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:324`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L324)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:332`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L332)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:340`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L340)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:348`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L348)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:361`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L361)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:374`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L374)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:387`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L387)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:395`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L395)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:407`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L407)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:415`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L415)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:429`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L429)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:442`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L442)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:458`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L458)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:474`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L474)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:495`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L495)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:508`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L508)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:521`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L521)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:533`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L533)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:548`](https://github.com/nf-core/methylong/blob/7b03e9a9821d8ea9a137dc4b1bde7856d4e7ae1e/conf/modules.config#L548)

  ```nextflow
  publishDir = [
  ```
