# Workflow outputs migration: phageannotator

- Generated: 2026-06-16T19:35:27.874152+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 39 `publishDir` references across 38 files that should be migrated to the workflow `output {}` block:

- [`modules/nf-core/mash/sketch/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/mash/sketch/nextflow.config#L4) — 2 references
- [`modules/local/anicluster/anicalc/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/anicluster/anicalc/nextflow.config#L3) — 1 reference
- [`modules/local/anicluster/aniclust/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/anicluster/aniclust/nextflow.config#L8) — 1 reference
- [`modules/local/anicluster/extractreps/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/anicluster/extractreps/nextflow.config#L4) — 1 reference
- [`modules/local/appendscreenhits/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/appendscreenhits/nextflow.config#L3) — 1 reference
- [`modules/local/coverm/contig/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/coverm/contig/nextflow.config#L9) — 1 reference
- [`modules/local/extractviralassemblies/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/extractviralassemblies/nextflow.config#L3) — 1 reference
- [`modules/local/instrain/stb/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/instrain/stb/nextflow.config#L3) — 1 reference
- [`modules/local/mash/paste/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/mash/paste/nextflow.config#L3) — 1 reference
- [`modules/local/qualityfilterviruses/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/qualityfilterviruses/nextflow.config#L9) — 1 reference
- [`modules/local/seqkit/seq/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/seqkit/seq/nextflow.config#L4) — 1 reference
- [`modules/local/viromeqc/install/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/viromeqc/install/nextflow.config#L4) — 1 reference
- [`modules/local/viromeqc/viromeqc/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/local/viromeqc/viromeqc/nextflow.config#L3) — 1 reference
- [`modules/nf-core/bacphlip/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/bacphlip/nextflow.config#L3) — 1 reference
- [`modules/nf-core/blast/blastn/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/blast/blastn/nextflow.config#L8) — 1 reference
- [`modules/nf-core/blast/makeblastdb/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/blast/makeblastdb/nextflow.config#L4) — 1 reference
- [`modules/nf-core/bowtie2/align/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/bowtie2/align/nextflow.config#L3) — 1 reference
- [`modules/nf-core/bowtie2/build/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/bowtie2/build/nextflow.config#L3) — 1 reference
- [`modules/nf-core/cat/cat/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/cat/cat/nextflow.config#L3) — 1 reference
- [`modules/nf-core/checkv/downloaddatabase/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/checkv/downloaddatabase/nextflow.config#L3) — 1 reference
- [`modules/nf-core/checkv/endtoend/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/checkv/endtoend/nextflow.config#L3) — 1 reference
- [`modules/nf-core/cobrameta/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/cobrameta/nextflow.config#L3) — 1 reference
- [`modules/nf-core/fastqc/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/fastqc/nextflow.config#L4) — 1 reference
- [`modules/nf-core/genomad/download/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/genomad/download/nextflow.config#L3) — 1 reference
- [`modules/nf-core/genomad/endtoend/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/genomad/endtoend/nextflow.config#L10) — 1 reference
- [`modules/nf-core/gunzip/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/gunzip/nextflow.config#L3) — 1 reference
- [`modules/nf-core/instrain/compare/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/instrain/compare/nextflow.config#L3) — 1 reference
- [`modules/nf-core/instrain/profile/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/instrain/profile/nextflow.config#L3) — 1 reference
- [`modules/nf-core/iphop/download/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/iphop/download/nextflow.config#L3) — 1 reference
- [`modules/nf-core/iphop/predict/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/iphop/predict/nextflow.config#L3) — 1 reference
- [`modules/nf-core/mash/screen/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/mash/screen/nextflow.config#L7) — 1 reference
- [`modules/nf-core/multiqc/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/multiqc/nextflow.config#L4) — 1 reference
- [`modules/nf-core/pharokka/pharokka/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/pharokka/pharokka/nextflow.config#L6) — 1 reference
- [`modules/nf-core/samtools/flagstat/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/samtools/flagstat/nextflow.config#L3) — 1 reference
- [`modules/nf-core/samtools/idxstats/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/samtools/idxstats/nextflow.config#L3) — 1 reference
- [`modules/nf-core/samtools/index/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/samtools/index/nextflow.config#L3) — 1 reference
- [`modules/nf-core/samtools/stats/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/samtools/stats/nextflow.config#L3) — 1 reference
- [`modules/nf-core/untar/nextflow.config`](https://github.com/nf-core/phageannotator/blob/129a138b32e88c3e9e43a46d8146f70d2061f67f/modules/nf-core/untar/nextflow.config#L3) — 1 reference
