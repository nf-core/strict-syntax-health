# Workflow outputs migration: genomeqc

- Generated: 2026-06-16T14:18:17.821803+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 39 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:28`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L28)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:37`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:45`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:54`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L54)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:62`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L62)

  ```nextflow
  //    publishDir = [
  ```

- [`conf/modules.config:71`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L71)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:79`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L79)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:87`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L87)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:96`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L96)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:104`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L104)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:110`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L110)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:116`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L116)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:124`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L124)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:133`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L133)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:142`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L142)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:149`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L149)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:156`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L156)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:163`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L163)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:170`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L170)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:177`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L177)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:184`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L184)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:192`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L192)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:200`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L200)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:208`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L208)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:217`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L217)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:226`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L226)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:234`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L234)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:242`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L242)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:249`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L249)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:256`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L256)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:273`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L273)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:285`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L285)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:293`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L293)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:303`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L303)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:311`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L311)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:319`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/conf/modules.config#L319)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/tree_summary.nf:6`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/modules/local/tree_summary.nf#L6)

  ```nextflow
  publishDir "$params.outdir/tree_plots" , mode: "${params.publish_dir_mode}", pattern:"*.pdf"
  ```

- [`nextflow.config:106`](https://github.com/nf-core/genomeqc/blob/49b7cbd1c2e703896cd0553b3080f8ab148ce8c1/nextflow.config#L106)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
