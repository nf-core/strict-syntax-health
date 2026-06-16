# Workflow outputs migration: dualrnaseq

- Generated: 2026-06-16T14:15:25.144103+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 32 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:27`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:40`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L40)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:50`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L50)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:55`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L55)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:65`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L65)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:84`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L84)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:91`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L91)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:98`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L98)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:105`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L105)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:112`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L112)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:119`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L119)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:135`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L135)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:151`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L151)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:159`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L159)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:166`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L166)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:173`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L173)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:180`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L180)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:187`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L187)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:204`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L204)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:220`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L220)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:237`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L237)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:246`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L246)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:266`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L266)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:286`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L286)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:302`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L302)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:322`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L322)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:337`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/conf/modules.config#L337)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/collate_processed_reads/main.nf:6`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/modules/local/collate_processed_reads/main.nf#L6)

  ```nextflow
  // Set publishDir to the process using inputs.process
  ```

- [`modules/local/collate_processed_reads/main.nf:7`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/modules/local/collate_processed_reads/main.nf#L7)

  ```nextflow
  publishDir path: "${params.outdir}/mapping_statistics/${process}/", mode: params.publish_dir_mode
  ```

- [`modules/local/extract_processed_reads/main.nf:11`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/modules/local/extract_processed_reads/main.nf#L11)

  ```nextflow
  // Set publishDir to the process using inputs.process
  ```

- [`modules/local/extract_processed_reads/main.nf:12`](https://github.com/nf-core/dualrnaseq/blob/df992a7516a2018b7bffefd069c21b2ff956d404/modules/local/extract_processed_reads/main.nf#L12)

  ```nextflow
  publishDir path: "${params.outdir}/mapping_statistics/${process}/", mode: params.publish_dir_mode
  ```
