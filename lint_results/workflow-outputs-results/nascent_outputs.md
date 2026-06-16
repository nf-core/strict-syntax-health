# Workflow outputs migration: nascent

- Generated: 2026-06-16T14:24:55.621759+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 41 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:45`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:51`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L51)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:64`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L64)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:77`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L77)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:83`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L83)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:89`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L89)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:101`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L101)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:112`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L112)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:152`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L152)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:181`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L181)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:190`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L190)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:199`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L199)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:208`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L208)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:222`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L222)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:238`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L238)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:251`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L251)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:271`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L271)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:279`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L279)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:288`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L288)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:303`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L303)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:317`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L317)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:345`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L345)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:369`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L369)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:379`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L379)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:385`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L385)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:396`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L396)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:404`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L404)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:416`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L416)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:428`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L428)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:443`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L443)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:451`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L451)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:459`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/conf/modules.config#L459)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/rseqc/bamstat/tests/nextflow.config:3`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/modules/nf-core/rseqc/bamstat/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/rseqc/inferexperiment/tests/nextflow.config:3`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/modules/nf-core/rseqc/inferexperiment/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/rseqc/innerdistance/tests/nextflow.config:3`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/modules/nf-core/rseqc/innerdistance/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/subread/featurecounts/tests/nextflow.config:3`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`subworkflows/nf-core/fastq_align_star/tests/nextflow.config:3`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/subworkflows/nf-core/fastq_align_star/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config:3`](https://github.com/nf-core/nascent/blob/8d094841b348aca2e857c9d40b4e0c8f5f8320ec/subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```
