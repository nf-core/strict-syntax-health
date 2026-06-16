# Workflow outputs migration: genomeassembler

- Generated: 2026-06-16T14:18:09.181439+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 60 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/alignments.config:5`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/alignments.config#L5)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/alignments.config:17`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/alignments.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/alignments.config:28`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/alignments.config#L28)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/alignments.config:39`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/alignments.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/alignments.config:50`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/alignments.config#L50)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/alignments.config:61`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/alignments.config#L61)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/alignments.config:72`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/alignments.config#L72)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/busco.config:4`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/busco.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/busco.config:13`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/busco.config#L13)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/busco.config:22`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/busco.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/busco.config:31`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/busco.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/busco.config:40`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/busco.config#L40)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/busco.config:50`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/busco.config#L50)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/jellyfish-genomescope.config:3`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/jellyfish-genomescope.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/jellyfish-genomescope.config:10`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/jellyfish-genomescope.config#L10)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/jellyfish-genomescope.config:17`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/jellyfish-genomescope.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/jellyfish-genomescope.config:24`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/jellyfish-genomescope.config#L24)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/jellyfish-genomescope.config:31`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/jellyfish-genomescope.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/merqury.config:4`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/merqury.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/merqury.config:12`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/merqury.config#L12)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/merqury.config:20`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/merqury.config#L20)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/merqury.config:28`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/merqury.config#L28)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/merqury.config:36`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/merqury.config#L36)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/merqury.config:45`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/merqury.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/meryl.config:3`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/meryl.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/meryl.config:10`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/meryl.config#L10)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/quast.config:4`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/quast.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/quast.config:12`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/quast.config#L12)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/quast.config:20`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/quast.config#L20)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/quast.config:28`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/quast.config#L28)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/quast.config:36`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/quast.config#L36)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/QC/quast.config:45`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/quast.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/assembly.config:9`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/assembly.config#L9)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/assembly.config:17`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/assembly.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/assembly.config:25`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/assembly.config#L25)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/assembly.config:32`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/assembly.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/assembly.config:39`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/assembly.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/assembly.config:46`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/assembly.config#L46)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/assembly.config:53`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/assembly.config#L53)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/hifi-prep.config:3`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/hifi-prep.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/hifi-prep.config:10`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/hifi-prep.config#L10)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/liftoff.config:3`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/liftoff.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/liftoff.config:11`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/liftoff.config#L11)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/liftoff.config:19`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/liftoff.config#L19)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/liftoff.config:27`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/liftoff.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/liftoff.config:35`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/liftoff.config#L35)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/liftoff.config:43`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/liftoff.config#L43)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/ont-prep.config:3`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/ont-prep.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/ont-prep.config:10`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/ont-prep.config#L10)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/ont-prep.config:17`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/ont-prep.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/polishing.config:7`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/polishing.config#L7)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/polishing.config:15`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/polishing.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/polishing.config:25`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/polishing.config#L25)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/report.config:3`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/report.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/scaffolding.config:3`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/scaffolding.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/scaffolding.config:17`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/scaffolding.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/scaffolding.config:26`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/scaffolding.config#L26)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/trimgalore.config:3`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/trimgalore.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/lima/tests/nextflow.config:3`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/modules/nf-core/lima/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```
