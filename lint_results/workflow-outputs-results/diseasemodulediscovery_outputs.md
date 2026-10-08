# Workflow outputs migration: diseasemodulediscovery

- Generated: 2026-10-08T00:23:27.209109+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 19 `publishDir` references across 1 file that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/diseasemodulediscovery/blob/89c9dc0f19b0c4c6d465a0e8ace7b02fcc648a4f/conf/modules.config#L17) — 19 references
