# Workflow outputs migration: genomeassembler

- Generated: 2026-06-19T00:50:12.809428+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 60 `publishDir` references across 16 files that should be migrated to the workflow `output {}` block:

- [`conf/modules/QC/alignments.config`](https://github.com/nf-core/genomeassembler/blob/df11fab16c4ef0ef836e40406f56f0f099e6e353/conf/modules/QC/alignments.config#L5) — 7 references
- [`conf/modules/assembly.config`](https://github.com/nf-core/genomeassembler/blob/df11fab16c4ef0ef836e40406f56f0f099e6e353/conf/modules/assembly.config#L9) — 7 references
- [`conf/modules/QC/busco.config`](https://github.com/nf-core/genomeassembler/blob/df11fab16c4ef0ef836e40406f56f0f099e6e353/conf/modules/QC/busco.config#L4) — 6 references
- [`conf/modules/QC/merqury.config`](https://github.com/nf-core/genomeassembler/blob/df11fab16c4ef0ef836e40406f56f0f099e6e353/conf/modules/QC/merqury.config#L4) — 6 references
- [`conf/modules/QC/quast.config`](https://github.com/nf-core/genomeassembler/blob/df11fab16c4ef0ef836e40406f56f0f099e6e353/conf/modules/QC/quast.config#L4) — 6 references
- [`conf/modules/liftoff.config`](https://github.com/nf-core/genomeassembler/blob/df11fab16c4ef0ef836e40406f56f0f099e6e353/conf/modules/liftoff.config#L3) — 6 references
- [`conf/modules/QC/jellyfish-genomescope.config`](https://github.com/nf-core/genomeassembler/blob/df11fab16c4ef0ef836e40406f56f0f099e6e353/conf/modules/QC/jellyfish-genomescope.config#L3) — 5 references
- [`conf/modules/ont-prep.config`](https://github.com/nf-core/genomeassembler/blob/df11fab16c4ef0ef836e40406f56f0f099e6e353/conf/modules/ont-prep.config#L3) — 3 references
- [`conf/modules/polishing.config`](https://github.com/nf-core/genomeassembler/blob/df11fab16c4ef0ef836e40406f56f0f099e6e353/conf/modules/polishing.config#L7) — 3 references
- [`conf/modules/scaffolding.config`](https://github.com/nf-core/genomeassembler/blob/df11fab16c4ef0ef836e40406f56f0f099e6e353/conf/modules/scaffolding.config#L3) — 3 references
- [`conf/modules/QC/meryl.config`](https://github.com/nf-core/genomeassembler/blob/df11fab16c4ef0ef836e40406f56f0f099e6e353/conf/modules/QC/meryl.config#L3) — 2 references
- [`conf/modules/hifi-prep.config`](https://github.com/nf-core/genomeassembler/blob/df11fab16c4ef0ef836e40406f56f0f099e6e353/conf/modules/hifi-prep.config#L3) — 2 references
- [`conf/modules.config`](https://github.com/nf-core/genomeassembler/blob/df11fab16c4ef0ef836e40406f56f0f099e6e353/conf/modules.config#L15) — 1 reference
- [`conf/modules/report.config`](https://github.com/nf-core/genomeassembler/blob/df11fab16c4ef0ef836e40406f56f0f099e6e353/conf/modules/report.config#L3) — 1 reference
- [`conf/modules/trimgalore.config`](https://github.com/nf-core/genomeassembler/blob/df11fab16c4ef0ef836e40406f56f0f099e6e353/conf/modules/trimgalore.config#L3) — 1 reference
- [`modules/nf-core/lima/tests/nextflow.config`](https://github.com/nf-core/genomeassembler/blob/df11fab16c4ef0ef836e40406f56f0f099e6e353/modules/nf-core/lima/tests/nextflow.config#L3) — 1 reference
