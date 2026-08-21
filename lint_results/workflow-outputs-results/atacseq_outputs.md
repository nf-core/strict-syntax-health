# Workflow outputs migration: atacseq

- Generated: 2026-08-21T00:11:21.036753+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 79 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/atacseq/blob/5a4c18b3dd9a9d9484aa28903e44a58882f34b71/conf/modules.config#L18) — 78 references
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/atacseq/blob/5a4c18b3dd9a9d9484aa28903e44a58882f34b71/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
