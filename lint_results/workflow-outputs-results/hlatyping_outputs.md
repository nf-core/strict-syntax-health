# Workflow outputs migration: hlatyping

- Generated: 2026-08-01T00:30:19.909853+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 20 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/hlatyping/blob/4bd547ff758474c443d7bb373ece6d4c073249bd/conf/modules.config#L15) — 19 references
- [`modules/nf-core/hlala/preparegraph/tests/nextflow.config`](https://github.com/nf-core/hlatyping/blob/4bd547ff758474c443d7bb373ece6d4c073249bd/modules/nf-core/hlala/preparegraph/tests/nextflow.config#L7) — 1 reference
