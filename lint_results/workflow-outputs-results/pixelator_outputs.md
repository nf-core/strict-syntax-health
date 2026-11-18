# Workflow outputs migration: pixelator

- Generated: 2026-11-18T00:14:46.713443+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 10 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.pna.config`](https://github.com/nf-core/pixelator/blob/a493ab692b5ec7ab76d0640c9558abfd107e0e46/conf/modules.pna.config#L26) — 7 references
- [`conf/modules.config`](https://github.com/nf-core/pixelator/blob/a493ab692b5ec7ab76d0640c9558abfd107e0e46/conf/modules.config#L16) — 3 references
