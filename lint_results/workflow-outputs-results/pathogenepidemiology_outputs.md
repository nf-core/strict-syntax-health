# Workflow outputs migration: pathogenepidemiology

- Generated: 2026-10-13T00:27:24.759142+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 27 `publishDir` references across 6 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/pathogenepidemiology/blob/5af61764aa4eadce6caa43a9fdaff1e118b40476/conf/modules.config#L15) — 21 references
- [`nextflow.custom.config`](https://github.com/nf-core/pathogenepidemiology/blob/5af61764aa4eadce6caa43a9fdaff1e118b40476/nextflow.custom.config#L21) — 2 references
- [`modules/local/gatk4/variantrecalibrator/tests/AS.config`](https://github.com/nf-core/pathogenepidemiology/blob/5af61764aa4eadce6caa43a9fdaff1e118b40476/modules/local/gatk4/variantrecalibrator/tests/AS.config#L3) — 1 reference
- [`modules/local/gatk4/variantrecalibrator/tests/noAS.config`](https://github.com/nf-core/pathogenepidemiology/blob/5af61764aa4eadce6caa43a9fdaff1e118b40476/modules/local/gatk4/variantrecalibrator/tests/noAS.config#L3) — 1 reference
- [`modules/nf-core/gatk4/variantrecalibrator/tests/AS.config`](https://github.com/nf-core/pathogenepidemiology/blob/5af61764aa4eadce6caa43a9fdaff1e118b40476/modules/nf-core/gatk4/variantrecalibrator/tests/AS.config#L3) — 1 reference
- [`modules/nf-core/gatk4/variantrecalibrator/tests/noAS.config`](https://github.com/nf-core/pathogenepidemiology/blob/5af61764aa4eadce6caa43a9fdaff1e118b40476/modules/nf-core/gatk4/variantrecalibrator/tests/noAS.config#L3) — 1 reference
