# Workflow outputs migration: genomeassembler

- Generated: 2026-06-30T00:39:48.412457+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 93 `publishDir` references across 13 files that should be migrated to the workflow `output {}` block:

- [`conf/modules/QC/alignments.config`](https://github.com/nf-core/genomeassembler/blob/5a1991d1390f37932ff22a123aa21a5a12ebfa92/conf/modules/QC/alignments.config#L5) — 16 references
- [`conf/modules/scaffolding.config`](https://github.com/nf-core/genomeassembler/blob/5a1991d1390f37932ff22a123aa21a5a12ebfa92/conf/modules/scaffolding.config#L3) — 14 references
- [`conf/modules/assembly.config`](https://github.com/nf-core/genomeassembler/blob/5a1991d1390f37932ff22a123aa21a5a12ebfa92/conf/modules/assembly.config#L19) — 10 references
- [`conf/modules/polishing.config`](https://github.com/nf-core/genomeassembler/blob/5a1991d1390f37932ff22a123aa21a5a12ebfa92/conf/modules/polishing.config#L7) — 9 references
- [`conf/modules/QC/busco.config`](https://github.com/nf-core/genomeassembler/blob/5a1991d1390f37932ff22a123aa21a5a12ebfa92/conf/modules/QC/busco.config#L4) — 7 references
- [`conf/modules/QC/merqury.config`](https://github.com/nf-core/genomeassembler/blob/5a1991d1390f37932ff22a123aa21a5a12ebfa92/conf/modules/QC/merqury.config#L4) — 7 references
- [`conf/modules/QC/quast.config`](https://github.com/nf-core/genomeassembler/blob/5a1991d1390f37932ff22a123aa21a5a12ebfa92/conf/modules/QC/quast.config#L13) — 7 references
- [`conf/modules/liftoff.config`](https://github.com/nf-core/genomeassembler/blob/5a1991d1390f37932ff22a123aa21a5a12ebfa92/conf/modules/liftoff.config#L3) — 7 references
- [`conf/modules/QC/jellyfish-genomescope.config`](https://github.com/nf-core/genomeassembler/blob/5a1991d1390f37932ff22a123aa21a5a12ebfa92/conf/modules/QC/jellyfish-genomescope.config#L3) — 6 references
- [`conf/modules/read-prep.config`](https://github.com/nf-core/genomeassembler/blob/5a1991d1390f37932ff22a123aa21a5a12ebfa92/conf/modules/read-prep.config#L3) — 6 references
- [`conf/modules/QC/meryl.config`](https://github.com/nf-core/genomeassembler/blob/5a1991d1390f37932ff22a123aa21a5a12ebfa92/conf/modules/QC/meryl.config#L3) — 2 references
- [`conf/modules.config`](https://github.com/nf-core/genomeassembler/blob/5a1991d1390f37932ff22a123aa21a5a12ebfa92/conf/modules.config#L15) — 1 reference
- [`conf/modules/report.config`](https://github.com/nf-core/genomeassembler/blob/5a1991d1390f37932ff22a123aa21a5a12ebfa92/conf/modules/report.config#L3) — 1 reference
