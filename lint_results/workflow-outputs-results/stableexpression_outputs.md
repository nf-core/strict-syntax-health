# Workflow outputs migration: stableexpression

- Generated: 2026-06-16T14:36:39.936885+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 16 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:14`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules.config#L14)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gene_length.config:4`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/gene_length.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/gene_length.config:11`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/gene_length.config#L11)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/id_mapping.config:4`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/id_mapping.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/id_mapping.config:11`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/id_mapping.config#L11)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/id_mapping.config:18`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/id_mapping.config#L18)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/normalisation.config:4`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/normalisation.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/normalisation.config:14`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/normalisation.config#L14)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/normalisation.config:24`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/normalisation.config#L24)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/public_data.config:4`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/public_data.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/public_data.config:12`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/public_data.config#L12)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/public_data.config:23`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/public_data.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/public_data.config:30`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/public_data.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/reporting.config:4`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/reporting.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/reporting.config:14`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/reporting.config#L14)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/reporting.config:21`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/reporting.config#L21)

  ```nextflow
  publishDir = [
  ```
