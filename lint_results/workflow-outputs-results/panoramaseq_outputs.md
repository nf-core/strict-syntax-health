# Workflow outputs migration: panoramaseq

- Generated: 2026-06-16T14:26:24.321379+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 16 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:27`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/conf/modules.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:66`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/conf/modules.config#L66)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:97`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/conf/modules.config#L97)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:104`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/conf/modules.config#L104)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:111`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/conf/modules.config#L111)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:119`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/conf/modules.config#L119)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:127`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/conf/modules.config#L127)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:138`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/conf/modules.config#L138)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:150`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/conf/modules.config#L150)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/featurecounts/custom/tests/nextflow.config:2`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/modules/local/featurecounts/custom/tests/nextflow.config#L2)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/local/quik/tests/nextflow.config:2`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/modules/local/quik/tests/nextflow.config#L2)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/local/umicount/custom/tests/nextflow.config:2`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/modules/local/umicount/custom/tests/nextflow.config#L2)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/subread/featurecounts/tests/nextflow.config:3`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/umitools/extract/tests/nextflow.config:3`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/modules/nf-core/umitools/extract/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`tests/nextflow.config:68`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/tests/nextflow.config#L68)

  ```nextflow
  // Disable automatic publishDir
  ```
