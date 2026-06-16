# Workflow outputs migration: fastquorum

- Generated: 2026-06-16T14:16:32.984976+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 15 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/fastquorum/blob/1cbfe1450244036706546e50daa6b6c35054ff1a/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:28`](https://github.com/nf-core/fastquorum/blob/1cbfe1450244036706546e50daa6b6c35054ff1a/conf/modules.config#L28)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:37`](https://github.com/nf-core/fastquorum/blob/1cbfe1450244036706546e50daa6b6c35054ff1a/conf/modules.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:46`](https://github.com/nf-core/fastquorum/blob/1cbfe1450244036706546e50daa6b6c35054ff1a/conf/modules.config#L46)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:57`](https://github.com/nf-core/fastquorum/blob/1cbfe1450244036706546e50daa6b6c35054ff1a/conf/modules.config#L57)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:65`](https://github.com/nf-core/fastquorum/blob/1cbfe1450244036706546e50daa6b6c35054ff1a/conf/modules.config#L65)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:73`](https://github.com/nf-core/fastquorum/blob/1cbfe1450244036706546e50daa6b6c35054ff1a/conf/modules.config#L73)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:81`](https://github.com/nf-core/fastquorum/blob/1cbfe1450244036706546e50daa6b6c35054ff1a/conf/modules.config#L81)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:90`](https://github.com/nf-core/fastquorum/blob/1cbfe1450244036706546e50daa6b6c35054ff1a/conf/modules.config#L90)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:98`](https://github.com/nf-core/fastquorum/blob/1cbfe1450244036706546e50daa6b6c35054ff1a/conf/modules.config#L98)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:113`](https://github.com/nf-core/fastquorum/blob/1cbfe1450244036706546e50daa6b6c35054ff1a/conf/modules.config#L113)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:128`](https://github.com/nf-core/fastquorum/blob/1cbfe1450244036706546e50daa6b6c35054ff1a/conf/modules.config#L128)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:136`](https://github.com/nf-core/fastquorum/blob/1cbfe1450244036706546e50daa6b6c35054ff1a/conf/modules.config#L136)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:148`](https://github.com/nf-core/fastquorum/blob/1cbfe1450244036706546e50daa6b6c35054ff1a/conf/modules.config#L148)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:159`](https://github.com/nf-core/fastquorum/blob/1cbfe1450244036706546e50daa6b6c35054ff1a/conf/modules.config#L159)

  ```nextflow
  publishDir = [
  ```
