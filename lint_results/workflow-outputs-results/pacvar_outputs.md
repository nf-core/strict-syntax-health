# Workflow outputs migration: pacvar

- Generated: 2026-06-16T14:25:56.719855+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 16 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:14`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules.config#L14)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:65`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules.config#L65)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:74`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules.config#L74)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:82`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules.config#L82)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:91`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules.config#L91)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:100`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules.config#L100)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:131`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules.config#L131)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:139`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules.config#L139)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/ensemblvep.config:18`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules/ensemblvep.config#L18)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/ensemblvep.config:32`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules/ensemblvep.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/ensemblvep.config:48`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules/ensemblvep.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/ensemblvep.config:64`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules/ensemblvep.config#L64)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/fibertools.config:3`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/conf/modules/fibertools.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/lima/tests/nextflow.config:3`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/modules/nf-core/lima/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`nextflow.config:100`](https://github.com/nf-core/pacvar/blob/beb0ed2d0ed639448df72aee1bc54c6d2027f4cb/nextflow.config#L100)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
