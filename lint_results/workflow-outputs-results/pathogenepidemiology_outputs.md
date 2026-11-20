# Workflow outputs migration: pathogenepidemiology

- Generated: 2026-11-20T00:13:24.334439+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 25 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/pathogenepidemiology/blob/1eefa4618ea815227f1a90973ff4dc16dc19b638/conf/modules.config#L15) — 23 references
- [`modules/nf-core/gatk4/variantrecalibrator/tests/AS.config`](https://github.com/nf-core/pathogenepidemiology/blob/1eefa4618ea815227f1a90973ff4dc16dc19b638/modules/nf-core/gatk4/variantrecalibrator/tests/AS.config#L3) — 1 reference
- [`modules/nf-core/gatk4/variantrecalibrator/tests/noAS.config`](https://github.com/nf-core/pathogenepidemiology/blob/1eefa4618ea815227f1a90973ff4dc16dc19b638/modules/nf-core/gatk4/variantrecalibrator/tests/noAS.config#L3) — 1 reference
