# Workflow outputs migration: mcmicro

- Generated: 2026-06-16T14:21:57.237516+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 10 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/mcmicro/blob/1974c653761d9a8baac05a8d57ac3a019d79b943/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/mcmicro/blob/1974c653761d9a8baac05a8d57ac3a019d79b943/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:33`](https://github.com/nf-core/mcmicro/blob/1974c653761d9a8baac05a8d57ac3a019d79b943/conf/modules.config#L33)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:42`](https://github.com/nf-core/mcmicro/blob/1974c653761d9a8baac05a8d57ac3a019d79b943/conf/modules.config#L42)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:57`](https://github.com/nf-core/mcmicro/blob/1974c653761d9a8baac05a8d57ac3a019d79b943/conf/modules.config#L57)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:66`](https://github.com/nf-core/mcmicro/blob/1974c653761d9a8baac05a8d57ac3a019d79b943/conf/modules.config#L66)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:79`](https://github.com/nf-core/mcmicro/blob/1974c653761d9a8baac05a8d57ac3a019d79b943/conf/modules.config#L79)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:87`](https://github.com/nf-core/mcmicro/blob/1974c653761d9a8baac05a8d57ac3a019d79b943/conf/modules.config#L87)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:100`](https://github.com/nf-core/mcmicro/blob/1974c653761d9a8baac05a8d57ac3a019d79b943/conf/modules.config#L100)

  ```nextflow
  publishDir = [
  ```

- [`tests/lib/utils.nf:15`](https://github.com/nf-core/mcmicro/blob/1974c653761d9a8baac05a8d57ac3a019d79b943/tests/lib/utils.nf#L15)

  ```nextflow
  publishDir enabled: false
  ```
