# Workflow outputs migration: deepmutscan

- Generated: 2026-06-16T14:13:07.446298+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 22 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:28`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L28)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:36`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L36)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:44`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L44)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:52`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L52)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:60`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L60)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:68`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L68)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:81`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L81)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:89`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L89)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:97`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L97)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:108`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L108)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:120`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L120)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:128`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L128)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:136`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L136)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:144`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L144)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:152`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L152)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:160`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L160)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:168`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L168)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:176`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L176)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:184`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/conf/modules.config#L184)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/dmsanalysis/process_gatk/main.nf:11`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/modules/local/dmsanalysis/process_gatk/main.nf#L11)

  ```nextflow
  publishDir "${params.outdir}/intermediate_files", mode: 'copy'
  ```

- [`nextflow.config:64`](https://github.com/nf-core/deepmutscan/blob/e4b9554bb6c6ad717c4944d4abe08561e9eb5c1e/nextflow.config#L64)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
