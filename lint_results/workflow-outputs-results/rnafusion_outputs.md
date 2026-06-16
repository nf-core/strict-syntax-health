# Workflow outputs migration: rnafusion

- Generated: 2026-06-16T14:31:31.128186+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 36 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:27`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:37`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:45`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:59`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L59)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:67`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L67)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:76`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L76)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:86`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L86)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:95`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L95)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:105`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L105)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:123`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L123)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:133`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L133)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:142`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L142)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:150`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L150)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:158`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L158)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:166`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L166)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:175`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L175)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:184`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L184)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:192`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L192)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:201`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L201)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:210`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L210)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:225`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L225)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:233`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L233)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:245`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L245)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:253`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L253)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:262`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L262)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:270`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L270)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:283`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L283)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:319`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L319)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:332`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L332)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:342`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L342)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:351`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/conf/modules.config#L351)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/umitools/extract/tests/nextflow.config:3`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/modules/nf-core/umitools/extract/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`nextflow.config:113`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/nextflow.config#L113)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```

- [`subworkflows/nf-core/fastq_align_star/tests/nextflow.config:3`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/subworkflows/nf-core/fastq_align_star/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config:3`](https://github.com/nf-core/rnafusion/blob/d91904e05490eef579ca4c28d17a6172ddbb864b/subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```
