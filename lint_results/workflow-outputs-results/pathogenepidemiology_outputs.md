# Workflow outputs migration: pathogenepidemiology

- Generated: 2026-08-05T00:30:00.334746+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 15 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`nextflow.custom.config`](https://github.com/nf-core/pathogenepidemiology/blob/13621e99c2baa915276f94820023ff697a304dae/nextflow.custom.config#L20) — 11 references
- [`conf/modules.config`](https://github.com/nf-core/pathogenepidemiology/blob/13621e99c2baa915276f94820023ff697a304dae/conf/modules.config#L15) — 2 references
- [`modules/nf-core/gatk4/variantrecalibrator/tests/AS.config`](https://github.com/nf-core/pathogenepidemiology/blob/13621e99c2baa915276f94820023ff697a304dae/modules/nf-core/gatk4/variantrecalibrator/tests/AS.config#L3) — 1 reference
- [`modules/nf-core/gatk4/variantrecalibrator/tests/noAS.config`](https://github.com/nf-core/pathogenepidemiology/blob/13621e99c2baa915276f94820023ff697a304dae/modules/nf-core/gatk4/variantrecalibrator/tests/noAS.config#L3) — 1 reference
