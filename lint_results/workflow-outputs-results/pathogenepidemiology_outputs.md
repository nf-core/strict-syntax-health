# Workflow outputs migration: pathogenepidemiology

- Generated: 2026-07-29T00:29:39.811677+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 11 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`nextflow.custom.config`](https://github.com/nf-core/pathogenepidemiology/blob/d9dcfaee606f3fe33ddcfadedccd7011fe586ddb/nextflow.custom.config#L16) — 7 references
- [`conf/modules.config`](https://github.com/nf-core/pathogenepidemiology/blob/d9dcfaee606f3fe33ddcfadedccd7011fe586ddb/conf/modules.config#L15) — 2 references
- [`modules/nf-core/gatk4/variantrecalibrator/tests/AS.config`](https://github.com/nf-core/pathogenepidemiology/blob/d9dcfaee606f3fe33ddcfadedccd7011fe586ddb/modules/nf-core/gatk4/variantrecalibrator/tests/AS.config#L3) — 1 reference
- [`modules/nf-core/gatk4/variantrecalibrator/tests/noAS.config`](https://github.com/nf-core/pathogenepidemiology/blob/d9dcfaee606f3fe33ddcfadedccd7011fe586ddb/modules/nf-core/gatk4/variantrecalibrator/tests/noAS.config#L3) — 1 reference
