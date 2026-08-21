# Workflow outputs migration: pixelator

- Generated: 2026-08-21T00:13:18.767185+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 12 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.pna.config`](https://github.com/nf-core/pixelator/blob/734dfc08d9bf7e57959d8ab9042fe8e223c6b84a/conf/modules.pna.config#L30) — 8 references
- [`conf/modules.config`](https://github.com/nf-core/pixelator/blob/734dfc08d9bf7e57959d8ab9042fe8e223c6b84a/conf/modules.config#L16) — 4 references
