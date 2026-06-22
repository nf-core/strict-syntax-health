# Workflow outputs migration: mag

- Generated: 2026-06-22T00:44:27.639596+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 39 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/mag/blob/92c0b2f6fea4dfb62bbc9cc1b80c6bd4dd52432e/conf/modules.config#L16) — 38 references
- [`modules/nf-core/dastool/dastool/tests/nextflow.config`](https://github.com/nf-core/mag/blob/92c0b2f6fea4dfb62bbc9cc1b80c6bd4dd52432e/modules/nf-core/dastool/dastool/tests/nextflow.config#L3) — 1 reference
