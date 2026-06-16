# Workflow outputs migration: genomeassembler

- Generated: 2026-06-16T20:25:34.134946+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 60 `publishDir` references across 16 files that should be migrated to the workflow `output {}` block:

- [`conf/modules/QC/alignments.config`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/alignments.config#L5) — 7 references
- [`conf/modules/assembly.config`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/assembly.config#L9) — 7 references
- [`conf/modules/QC/busco.config`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/busco.config#L4) — 6 references
- [`conf/modules/QC/merqury.config`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/merqury.config#L4) — 6 references
- [`conf/modules/QC/quast.config`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/quast.config#L4) — 6 references
- [`conf/modules/liftoff.config`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/liftoff.config#L3) — 6 references
- [`conf/modules/QC/jellyfish-genomescope.config`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/jellyfish-genomescope.config#L3) — 5 references
- [`conf/modules/ont-prep.config`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/ont-prep.config#L3) — 3 references
- [`conf/modules/polishing.config`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/polishing.config#L7) — 3 references
- [`conf/modules/scaffolding.config`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/scaffolding.config#L3) — 3 references
- [`conf/modules/QC/meryl.config`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/QC/meryl.config#L3) — 2 references
- [`conf/modules/hifi-prep.config`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/hifi-prep.config#L3) — 2 references
- [`conf/modules.config`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules.config#L15) — 1 reference
- [`conf/modules/report.config`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/report.config#L3) — 1 reference
- [`conf/modules/trimgalore.config`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/conf/modules/trimgalore.config#L3) — 1 reference
- [`modules/nf-core/lima/tests/nextflow.config`](https://github.com/nf-core/genomeassembler/blob/b017207723b90730c53a0c2b17a4a62170a2cfff/modules/nf-core/lima/tests/nextflow.config#L3) — 1 reference
