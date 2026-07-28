# Workflow outputs migration: panoramaseq

- Generated: 2026-07-28T00:31:17.689991+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 15 `publishDir` references across 6 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/panoramaseq/blob/4908592cbc5ccd79a7f99edc56825c5a98079aae/conf/modules.config#L15) — 10 references
- [`modules/local/featurecounts/custom/tests/nextflow.config`](https://github.com/nf-core/panoramaseq/blob/4908592cbc5ccd79a7f99edc56825c5a98079aae/modules/local/featurecounts/custom/tests/nextflow.config#L2) — 1 reference
- [`modules/local/quik/tests/nextflow.config`](https://github.com/nf-core/panoramaseq/blob/4908592cbc5ccd79a7f99edc56825c5a98079aae/modules/local/quik/tests/nextflow.config#L2) — 1 reference
- [`modules/local/umicount/custom/tests/nextflow.config`](https://github.com/nf-core/panoramaseq/blob/4908592cbc5ccd79a7f99edc56825c5a98079aae/modules/local/umicount/custom/tests/nextflow.config#L2) — 1 reference
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/panoramaseq/blob/4908592cbc5ccd79a7f99edc56825c5a98079aae/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/panoramaseq/blob/4908592cbc5ccd79a7f99edc56825c5a98079aae/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
