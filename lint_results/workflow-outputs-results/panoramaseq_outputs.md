# Workflow outputs migration: panoramaseq

- Generated: 2026-06-16T19:35:09.419536+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 15 `publishDir` references across 6 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/conf/modules.config#L15) — 10 references
- [`modules/local/featurecounts/custom/tests/nextflow.config`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/modules/local/featurecounts/custom/tests/nextflow.config#L2) — 1 reference
- [`modules/local/quik/tests/nextflow.config`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/modules/local/quik/tests/nextflow.config#L2) — 1 reference
- [`modules/local/umicount/custom/tests/nextflow.config`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/modules/local/umicount/custom/tests/nextflow.config#L2) — 1 reference
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/panoramaseq/blob/6ae42ff41da173277612264afb4482667ff91cde/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
