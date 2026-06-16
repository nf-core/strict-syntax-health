# Workflow outputs migration: sammyseq

- Generated: 2026-06-16T14:33:04.066945+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 30 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:14`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L14)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:21`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L21)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:41`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L41)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:50`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L50)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:63`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L63)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:73`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L73)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:95`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L95)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:119`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L119)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:128`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L128)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:147`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L147)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:157`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L157)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:173`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L173)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:182`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L182)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:192`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L192)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:201`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L201)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:218`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L218)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:232`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L232)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:248`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L248)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:259`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L259)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:277`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L277)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:296`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L296)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:310`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L310)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:321`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L321)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:330`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L330)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:340`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L340)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:349`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L349)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:365`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L365)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:373`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/conf/modules.config#L373)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_align_bwaaln/nextflow.config:7`](https://github.com/nf-core/sammyseq/blob/ff3da4b7c7e312e117427761cc388b694eca3ef5/subworkflows/nf-core/fastq_align_bwaaln/nextflow.config#L7)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```
