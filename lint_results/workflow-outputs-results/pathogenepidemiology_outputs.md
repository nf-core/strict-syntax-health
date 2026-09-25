# Workflow outputs migration: pathogenepidemiology

- Generated: 2026-09-25T00:21:05.593719+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 20 `publishDir` references across 6 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/pathogenepidemiology/blob/548a5b0666870f2d33a14f3466c57e5527947b46/conf/modules.config#L15) — 14 references
- [`nextflow.custom.config`](https://github.com/nf-core/pathogenepidemiology/blob/548a5b0666870f2d33a14f3466c57e5527947b46/nextflow.custom.config#L21) — 2 references
- [`modules/local/gatk4/variantrecalibrator/tests/AS.config`](https://github.com/nf-core/pathogenepidemiology/blob/548a5b0666870f2d33a14f3466c57e5527947b46/modules/local/gatk4/variantrecalibrator/tests/AS.config#L3) — 1 reference
- [`modules/local/gatk4/variantrecalibrator/tests/noAS.config`](https://github.com/nf-core/pathogenepidemiology/blob/548a5b0666870f2d33a14f3466c57e5527947b46/modules/local/gatk4/variantrecalibrator/tests/noAS.config#L3) — 1 reference
- [`modules/nf-core/gatk4/variantrecalibrator/tests/AS.config`](https://github.com/nf-core/pathogenepidemiology/blob/548a5b0666870f2d33a14f3466c57e5527947b46/modules/nf-core/gatk4/variantrecalibrator/tests/AS.config#L3) — 1 reference
- [`modules/nf-core/gatk4/variantrecalibrator/tests/noAS.config`](https://github.com/nf-core/pathogenepidemiology/blob/548a5b0666870f2d33a14f3466c57e5527947b46/modules/nf-core/gatk4/variantrecalibrator/tests/noAS.config#L3) — 1 reference
