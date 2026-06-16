# Workflow outputs migration: mspepid

- Generated: 2026-06-16T14:23:56.434148+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 10 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/mspepid/blob/6b5c623d878e520308eb0feb61d7ae36428f88d7/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/mspepid/blob/6b5c623d878e520308eb0feb61d7ae36428f88d7/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:39`](https://github.com/nf-core/mspepid/blob/6b5c623d878e520308eb0feb61d7ae36428f88d7/conf/modules.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:47`](https://github.com/nf-core/mspepid/blob/6b5c623d878e520308eb0feb61d7ae36428f88d7/conf/modules.config#L47)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:55`](https://github.com/nf-core/mspepid/blob/6b5c623d878e520308eb0feb61d7ae36428f88d7/conf/modules.config#L55)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:74`](https://github.com/nf-core/mspepid/blob/6b5c623d878e520308eb0feb61d7ae36428f88d7/conf/modules.config#L74)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/cometconfig/main.nf:5`](https://github.com/nf-core/mspepid/blob/6b5c623d878e520308eb0feb61d7ae36428f88d7/modules/local/cometconfig/main.nf#L5)

  ```nextflow
  publishDir path: { "${params.outdir}/comet" }, mode: params.publish_dir_mode
  ```

- [`modules/local/ms2rescore/getmodel/main.nf:5`](https://github.com/nf-core/mspepid/blob/6b5c623d878e520308eb0feb61d7ae36428f88d7/modules/local/ms2rescore/getmodel/main.nf#L5)

  ```nextflow
  publishDir path: { "${params.outdir}/ms2rescore" }, mode: params.publish_dir_mode
  ```

- [`modules/local/psmutilsconversions/main.nf:6`](https://github.com/nf-core/mspepid/blob/6b5c623d878e520308eb0feb61d7ae36428f88d7/modules/local/psmutilsconversions/main.nf#L6)

  ```nextflow
  publishDir path: { "${params.outdir}/${meta.searchengine ?: 'unknown'}" }, mode: params.publish_dir_mode
  ```

- [`nextflow.config:70`](https://github.com/nf-core/mspepid/blob/6b5c623d878e520308eb0feb61d7ae36428f88d7/nextflow.config#L70)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
