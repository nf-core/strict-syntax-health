# Workflow outputs migration: callingcards

- Generated: 2026-06-16T14:10:11.970131+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 40 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:42`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L42)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:59`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L59)

  ```nextflow
  // default publishDir for prepare_reads steps
  ```

- [`conf/modules.config:68`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L68)

  ```nextflow
  publishDir = PREPARED_READS_DEFAULT_PUBLISHDIR +
  ```

- [`conf/modules.config:88`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L88)

  ```nextflow
  publishDir = PREPARED_READS_DEFAULT_PUBLISHDIR
  ```

- [`conf/modules.config:94`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L94)

  ```nextflow
  publishDir = PREPARED_READS_DEFAULT_PUBLISHDIR +
  ```

- [`conf/modules.config:107`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L107)

  ```nextflow
  publishDir = PREPARED_READS_DEFAULT_PUBLISHDIR +
  ```

- [`conf/modules.config:120`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L120)

  ```nextflow
  publishDir = PREPARED_READS_DEFAULT_PUBLISHDIR
  ```

- [`conf/modules.config:126`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L126)

  ```nextflow
  publishDir = PREPARED_READS_DEFAULT_PUBLISHDIR
  ```

- [`conf/modules.config:134`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L134)

  ```nextflow
  publishDir = PREPARED_READS_DEFAULT_PUBLISHDIR +
  ```

- [`conf/modules.config:144`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L144)

  ```nextflow
  publishDir = PREPARED_READS_DEFAULT_PUBLISHDIR +
  ```

- [`conf/modules.config:155`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L155)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:166`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L166)

  ```nextflow
  publishDir = PREPARED_READS_DEFAULT_PUBLISHDIR +
  ```

- [`conf/modules.config:185`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L185)

  ```nextflow
  publishDir = ALIGN_DEFAULT_PUBLISHDIR +
  ```

- [`conf/modules.config:202`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L202)

  ```nextflow
  // set default publishDir for all ALIGN steps.
  ```

- [`conf/modules.config:206`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L206)

  ```nextflow
  publishDir = ALIGN_DEFAULT_PUBLISHDIR +
  ```

- [`conf/modules.config:237`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L237)

  ```nextflow
  publishDir = PROCESS_ALIGNMENTS_DEFAULT_PUBLISHDIR +
  ```

- [`conf/modules.config:248`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L248)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:259`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L259)

  ```nextflow
  publishDir = PROCESS_ALIGNMENTS_DEFAULT_PUBLISHDIR +
  ```

- [`conf/modules.config:267`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L267)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:278`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L278)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:286`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L286)

  ```nextflow
  publishDir = PROCESS_ALIGNMENTS_DEFAULT_PUBLISHDIR
  ```

- [`conf/modules.config:293`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L293)

  ```nextflow
  publishDir = PROCESS_ALIGNMENTS_DEFAULT_PUBLISHDIR
  ```

- [`conf/modules.config:300`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L300)

  ```nextflow
  publishDir = PROCESS_ALIGNMENTS_DEFAULT_PUBLISHDIR
  ```

- [`conf/modules.config:310`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L310)

  ```nextflow
  publishDir = PROCESS_ALIGNMENTS_DEFAULT_PUBLISHDIR
  ```

- [`conf/modules.config:321`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L321)

  ```nextflow
  publishDir = PROCESS_ALIGNMENTS_DEFAULT_PUBLISHDIR
  ```

- [`conf/modules.config:333`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L333)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:343`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L343)

  ```nextflow
  publishDir = PROCESS_ALIGNMENTS_DEFAULT_PUBLISHDIR
  ```

- [`conf/modules.config:350`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L350)

  ```nextflow
  publishDir = PROCESS_ALIGNMENTS_DEFAULT_PUBLISHDIR
  ```

- [`conf/modules.config:357`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L357)

  ```nextflow
  publishDir = PROCESS_ALIGNMENTS_DEFAULT_PUBLISHDIR
  ```

- [`conf/modules.config:367`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L367)

  ```nextflow
  publishDir = PROCESS_ALIGNMENTS_DEFAULT_PUBLISHDIR
  ```

- [`conf/modules.config:378`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/conf/modules.config#L378)

  ```nextflow
  publishDir = PROCESS_ALIGNMENTS_DEFAULT_PUBLISHDIR
  ```

- [`modules/nf-core/rseqc/bamstat/tests/nextflow.config:3`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/modules/nf-core/rseqc/bamstat/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/rseqc/inferexperiment/tests/nextflow.config:3`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/modules/nf-core/rseqc/inferexperiment/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/rseqc/innerdistance/tests/nextflow.config:3`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/modules/nf-core/rseqc/innerdistance/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/subread/featurecounts/tests/nextflow.config:3`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/umitools/extract/tests/nextflow.config:3`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/modules/nf-core/umitools/extract/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`subworkflows/nf-core/fastq_align_bwaaln/nextflow.config:7`](https://github.com/nf-core/callingcards/blob/649f56c01b44fe26c174fd901a9c79be15e4be00/subworkflows/nf-core/fastq_align_bwaaln/nextflow.config#L7)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```
