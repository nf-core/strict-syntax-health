# Workflow outputs migration: fetchngs

- Generated: 2026-06-16T14:16:50.235456+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 10 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/base.config:16`](https://github.com/nf-core/fetchngs/blob/0ae5518f251fd8ea78c5785f8c9e55fdf0e1db2c/conf/base.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/aspera_cli/nextflow.config:4`](https://github.com/nf-core/fetchngs/blob/0ae5518f251fd8ea78c5785f8c9e55fdf0e1db2c/modules/local/aspera_cli/nextflow.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/multiqc_mappings_config/nextflow.config:3`](https://github.com/nf-core/fetchngs/blob/0ae5518f251fd8ea78c5785f8c9e55fdf0e1db2c/modules/local/multiqc_mappings_config/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/sra_fastq_ftp/nextflow.config:4`](https://github.com/nf-core/fetchngs/blob/0ae5518f251fd8ea78c5785f8c9e55fdf0e1db2c/modules/local/sra_fastq_ftp/nextflow.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/sra_ids_to_runinfo/nextflow.config:3`](https://github.com/nf-core/fetchngs/blob/0ae5518f251fd8ea78c5785f8c9e55fdf0e1db2c/modules/local/sra_ids_to_runinfo/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/sra_runinfo_to_ftp/nextflow.config:3`](https://github.com/nf-core/fetchngs/blob/0ae5518f251fd8ea78c5785f8c9e55fdf0e1db2c/modules/local/sra_runinfo_to_ftp/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/sra_to_samplesheet/nextflow.config:3`](https://github.com/nf-core/fetchngs/blob/0ae5518f251fd8ea78c5785f8c9e55fdf0e1db2c/modules/local/sra_to_samplesheet/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/fastqdl/nextflow.config:3`](https://github.com/nf-core/fetchngs/blob/0ae5518f251fd8ea78c5785f8c9e55fdf0e1db2c/modules/nf-core/fastqdl/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/sratools/fasterqdump/nextflow.config:4`](https://github.com/nf-core/fetchngs/blob/0ae5518f251fd8ea78c5785f8c9e55fdf0e1db2c/modules/nf-core/sratools/fasterqdump/nextflow.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/sratools/prefetch/nextflow.config:3`](https://github.com/nf-core/fetchngs/blob/0ae5518f251fd8ea78c5785f8c9e55fdf0e1db2c/modules/nf-core/sratools/prefetch/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```
