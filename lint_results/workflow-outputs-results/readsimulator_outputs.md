# Workflow outputs migration: readsimulator

- Generated: 2026-06-16T14:30:01.034555+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 18 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:39`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:59`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L59)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:67`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L67)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:75`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L75)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:82`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L82)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:90`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L90)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:110`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L110)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:117`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L117)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:125`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L125)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:133`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L133)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:142`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L142)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:149`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L149)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:156`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L156)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:164`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L164)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:183`](https://github.com/nf-core/readsimulator/blob/0594160e22d147aed283553c4fc06839914fa036/conf/modules.config#L183)

  ```nextflow
  publishDir = [
  ```
