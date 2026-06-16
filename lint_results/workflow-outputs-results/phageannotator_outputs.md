# Workflow outputs migration: phageannotator

- Generated: 2026-06-16T14:26:43.541642+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 39 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`modules/local/anicluster/anicalc/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/anicluster/anicalc/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/anicluster/aniclust/nextflow.config:8`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/anicluster/aniclust/nextflow.config#L8)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/anicluster/extractreps/nextflow.config:4`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/anicluster/extractreps/nextflow.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/appendscreenhits/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/appendscreenhits/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/coverm/contig/nextflow.config:9`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/coverm/contig/nextflow.config#L9)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/extractviralassemblies/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/extractviralassemblies/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/instrain/stb/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/instrain/stb/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/mash/paste/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/mash/paste/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/qualityfilterviruses/nextflow.config:9`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/qualityfilterviruses/nextflow.config#L9)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/seqkit/seq/nextflow.config:4`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/seqkit/seq/nextflow.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/viromeqc/install/nextflow.config:4`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/viromeqc/install/nextflow.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/viromeqc/viromeqc/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/viromeqc/viromeqc/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/bacphlip/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/bacphlip/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/blast/blastn/nextflow.config:8`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/blast/blastn/nextflow.config#L8)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/blast/makeblastdb/nextflow.config:4`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/blast/makeblastdb/nextflow.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/bowtie2/align/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/bowtie2/align/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/bowtie2/build/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/bowtie2/build/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/cat/cat/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/cat/cat/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/checkv/downloaddatabase/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/checkv/downloaddatabase/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/checkv/endtoend/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/checkv/endtoend/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/cobrameta/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/cobrameta/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/fastqc/nextflow.config:4`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/fastqc/nextflow.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/genomad/download/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/genomad/download/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/genomad/endtoend/nextflow.config:10`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/genomad/endtoend/nextflow.config#L10)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/gunzip/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/gunzip/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/instrain/compare/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/instrain/compare/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/instrain/profile/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/instrain/profile/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/iphop/download/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/iphop/download/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/iphop/predict/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/iphop/predict/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/mash/screen/nextflow.config:7`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/mash/screen/nextflow.config#L7)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/mash/sketch/nextflow.config:4`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/mash/sketch/nextflow.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/mash/sketch/nextflow.config:11`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/mash/sketch/nextflow.config#L11)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/multiqc/nextflow.config:4`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/multiqc/nextflow.config#L4)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/pharokka/pharokka/nextflow.config:6`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/pharokka/pharokka/nextflow.config#L6)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/samtools/flagstat/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/samtools/flagstat/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/samtools/idxstats/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/samtools/idxstats/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/samtools/index/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/samtools/index/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/samtools/stats/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/samtools/stats/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/untar/nextflow.config:3`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/untar/nextflow.config#L3)

  ```nextflow
  publishDir = [
  ```
