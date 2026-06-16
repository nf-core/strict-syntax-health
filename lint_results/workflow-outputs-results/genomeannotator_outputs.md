# Workflow outputs migration: genomeannotator

- Generated: 2026-06-16T14:17:58.679764+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 14 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/genomeannotator/blob/cbd878f7997d367ccbe952648e114ad25962963f/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:21`](https://github.com/nf-core/genomeannotator/blob/cbd878f7997d367ccbe952648e114ad25962963f/conf/modules.config#L21)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:28`](https://github.com/nf-core/genomeannotator/blob/cbd878f7997d367ccbe952648e114ad25962963f/conf/modules.config#L28)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:35`](https://github.com/nf-core/genomeannotator/blob/cbd878f7997d367ccbe952648e114ad25962963f/conf/modules.config#L35)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:42`](https://github.com/nf-core/genomeannotator/blob/cbd878f7997d367ccbe952648e114ad25962963f/conf/modules.config#L42)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:49`](https://github.com/nf-core/genomeannotator/blob/cbd878f7997d367ccbe952648e114ad25962963f/conf/modules.config#L49)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:56`](https://github.com/nf-core/genomeannotator/blob/cbd878f7997d367ccbe952648e114ad25962963f/conf/modules.config#L56)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:63`](https://github.com/nf-core/genomeannotator/blob/cbd878f7997d367ccbe952648e114ad25962963f/conf/modules.config#L63)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:70`](https://github.com/nf-core/genomeannotator/blob/cbd878f7997d367ccbe952648e114ad25962963f/conf/modules.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:77`](https://github.com/nf-core/genomeannotator/blob/cbd878f7997d367ccbe952648e114ad25962963f/conf/modules.config#L77)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:99`](https://github.com/nf-core/genomeannotator/blob/cbd878f7997d367ccbe952648e114ad25962963f/conf/modules.config#L99)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:121`](https://github.com/nf-core/genomeannotator/blob/cbd878f7997d367ccbe952648e114ad25962963f/conf/modules.config#L121)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:128`](https://github.com/nf-core/genomeannotator/blob/cbd878f7997d367ccbe952648e114ad25962963f/conf/modules.config#L128)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:141`](https://github.com/nf-core/genomeannotator/blob/cbd878f7997d367ccbe952648e114ad25962963f/conf/modules.config#L141)

  ```nextflow
  publishDir = [
  ```
