# Workflow outputs migration: crisprseq

- Generated: 2026-06-16T20:20:05.043980+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 45 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/conf/modules.config#L15) — 43 references
- [`modules/local/guides_to_fasta/main.nf`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/modules/local/guides_to_fasta/main.nf#L10) — 1 reference
- [`modules/nf-core/vsearch/sort/tests/nextflow.config`](https://github.com/nf-core/crisprseq/blob/f41f53278e2ed8111db515831c1ef7456419fc99/modules/nf-core/vsearch/sort/tests/nextflow.config#L3) — 1 reference
