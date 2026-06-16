# Workflow outputs migration: createtaxdb

- Generated: 2026-06-16T14:11:45.907003+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 18 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/conf/modules.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:41`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/conf/modules.config#L41)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:50`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/conf/modules.config#L50)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:59`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/conf/modules.config#L59)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:68`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/conf/modules.config#L68)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:77`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/conf/modules.config#L77)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:88`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/conf/modules.config#L88)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:124`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/conf/modules.config#L124)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:136`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/conf/modules.config#L136)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:144`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/conf/modules.config#L144)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:164`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/conf/modules.config#L164)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:174`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/conf/modules.config#L174)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`conf/modules.config:183`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/conf/modules.config#L183)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`nextflow.config:105`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/nextflow.config#L105)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```

- [`subworkflows/local/sourmash_create/tests/dna.config:4`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/subworkflows/local/sourmash_create/tests/dna.config#L4)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`subworkflows/local/sourmash_create/tests/protein.config:4`](https://github.com/nf-core/createtaxdb/blob/d6024a30aba12bf4120348b672c15e84181d1792/subworkflows/local/sourmash_create/tests/protein.config#L4)

  ```nextflow
  publishDir = [enabled: false]
  ```
