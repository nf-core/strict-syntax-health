# Workflow outputs migration: taxmarker

- Generated: 2026-09-22T00:25:05.896091+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 4 `publishDir` references across 1 file that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/taxmarker/blob/f3aaaf90b6e91dda88f4a33b4ce3a51e12d75366/conf/modules.config#L15) — 4 references
