# Workflow outputs migration: crisprseq

- Generated: 2026-06-16T14:12:03.802111+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 45 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:40`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L40)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:48`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:56`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L56)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:64`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L64)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:73`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L73)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:81`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L81)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:90`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L90)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:98`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L98)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:106`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L106)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:112`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L112)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:118`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L118)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:126`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L126)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:135`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L135)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:147`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L147)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:160`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L160)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:169`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L169)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:178`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L178)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:188`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L188)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:197`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L197)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:206`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L206)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:215`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L215)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:223`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L223)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:232`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L232)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:241`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L241)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:250`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L250)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:259`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L259)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:283`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L283)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:292`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L292)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:302`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L302)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:312`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L312)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:322`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L322)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:332`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L332)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:346`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L346)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:355`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L355)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:368`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L368)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:376`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L376)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:384`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L384)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:394`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L394)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:407`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L407)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:416`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L416)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/guides_to_fasta/main.nf:10`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/modules/local/guides_to_fasta/main.nf#L10)

  ```nextflow
  publishDir "${params.outdir}/reference", enabled: false, mode:'copy'
  ```

- [`modules/nf-core/vsearch/sort/tests/nextflow.config:3`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/modules/nf-core/vsearch/sort/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```
