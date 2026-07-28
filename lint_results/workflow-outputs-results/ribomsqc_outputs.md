# Workflow outputs migration: ribomsqc

- Generated: 2026-07-28T00:33:54.624308+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 1 `publishDir` reference across 1 file that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/ribomsqc/blob/021c8778dac4596075fcac52d24f328ec9ab3e5a/conf/modules.config#L15) — 1 reference
