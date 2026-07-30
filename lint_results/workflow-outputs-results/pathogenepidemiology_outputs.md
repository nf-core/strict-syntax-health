# Workflow outputs migration: pathogenepidemiology

- Generated: 2026-07-30T00:29:50.200513+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 15 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`nextflow.custom.config`](https://github.com/nf-core/pathogenepidemiology/blob/380535d43c7fff0d1f5e0b571a1a638d794c6671/nextflow.custom.config#L18) — 11 references
- [`conf/modules.config`](https://github.com/nf-core/pathogenepidemiology/blob/380535d43c7fff0d1f5e0b571a1a638d794c6671/conf/modules.config#L15) — 2 references
- [`modules/nf-core/gatk4/variantrecalibrator/tests/AS.config`](https://github.com/nf-core/pathogenepidemiology/blob/380535d43c7fff0d1f5e0b571a1a638d794c6671/modules/nf-core/gatk4/variantrecalibrator/tests/AS.config#L3) — 1 reference
- [`modules/nf-core/gatk4/variantrecalibrator/tests/noAS.config`](https://github.com/nf-core/pathogenepidemiology/blob/380535d43c7fff0d1f5e0b571a1a638d794c6671/modules/nf-core/gatk4/variantrecalibrator/tests/noAS.config#L3) — 1 reference
