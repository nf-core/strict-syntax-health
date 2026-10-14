# Workflow outputs migration: atacseq

- Generated: 2026-10-14T00:18:48.126647+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 81 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/atacseq/blob/73155d2b59d37f521e3f00228d559031d2e7847f/conf/modules.config#L18) — 79 references
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/atacseq/blob/73155d2b59d37f521e3f00228d559031d2e7847f/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
- [`modules/nf-core/umitools/extract/tests/nextflow.config`](https://github.com/nf-core/atacseq/blob/73155d2b59d37f521e3f00228d559031d2e7847f/modules/nf-core/umitools/extract/tests/nextflow.config#L3) — 1 reference
