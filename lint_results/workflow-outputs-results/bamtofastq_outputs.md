# Workflow outputs migration: bamtofastq

- Generated: 2026-11-28T00:11:39.897852+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 9 `publishDir` references across 1 file that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/bamtofastq/blob/7e6822804f944b05c85519f042043974bef422bc/conf/modules.config#L15) — 9 references
