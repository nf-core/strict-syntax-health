# Workflow outputs migration: abotyper

- Generated: 2026-06-16T14:07:07.088313+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 16 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:14`](https://github.com/nf-core/abotyper/blob/76f2cd4fa720375ea6becf05dc40113825b9d349/conf/modules.config#L14)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/abotyper/blob/76f2cd4fa720375ea6becf05dc40113825b9d349/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:33`](https://github.com/nf-core/abotyper/blob/76f2cd4fa720375ea6becf05dc40113825b9d349/conf/modules.config#L33)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:43`](https://github.com/nf-core/abotyper/blob/76f2cd4fa720375ea6becf05dc40113825b9d349/conf/modules.config#L43)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:54`](https://github.com/nf-core/abotyper/blob/76f2cd4fa720375ea6becf05dc40113825b9d349/conf/modules.config#L54)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:64`](https://github.com/nf-core/abotyper/blob/76f2cd4fa720375ea6becf05dc40113825b9d349/conf/modules.config#L64)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:74`](https://github.com/nf-core/abotyper/blob/76f2cd4fa720375ea6becf05dc40113825b9d349/conf/modules.config#L74)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:83`](https://github.com/nf-core/abotyper/blob/76f2cd4fa720375ea6becf05dc40113825b9d349/conf/modules.config#L83)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:91`](https://github.com/nf-core/abotyper/blob/76f2cd4fa720375ea6becf05dc40113825b9d349/conf/modules.config#L91)

  ```nextflow
  //     publishDir = [
  ```

- [`conf/modules.config:100`](https://github.com/nf-core/abotyper/blob/76f2cd4fa720375ea6becf05dc40113825b9d349/conf/modules.config#L100)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:110`](https://github.com/nf-core/abotyper/blob/76f2cd4fa720375ea6becf05dc40113825b9d349/conf/modules.config#L110)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:121`](https://github.com/nf-core/abotyper/blob/76f2cd4fa720375ea6becf05dc40113825b9d349/conf/modules.config#L121)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:131`](https://github.com/nf-core/abotyper/blob/76f2cd4fa720375ea6becf05dc40113825b9d349/conf/modules.config#L131)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:141`](https://github.com/nf-core/abotyper/blob/76f2cd4fa720375ea6becf05dc40113825b9d349/conf/modules.config#L141)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/abo/snps2pheno/main.nf:10`](https://github.com/nf-core/abotyper/blob/76f2cd4fa720375ea6becf05dc40113825b9d349/modules/local/abo/snps2pheno/main.nf#L10)

  ```nextflow
  publishDir "${params.outdir}", mode: 'copy'
  ```

- [`nextflow.config:66`](https://github.com/nf-core/abotyper/blob/76f2cd4fa720375ea6becf05dc40113825b9d349/nextflow.config#L66)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
