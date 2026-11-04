# Workflow outputs migration: viralrecon

- Generated: 2026-11-04T00:15:44.190320+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 169 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/modules_illumina.config`](https://github.com/nf-core/viralrecon/blob/7cbb764e38012eb72a24c1a7a2d5db1e3251633a/conf/modules_illumina.config#L19) — 114 references
- [`conf/modules_nanopore.config`](https://github.com/nf-core/viralrecon/blob/7cbb764e38012eb72a24c1a7a2d5db1e3251633a/conf/modules_nanopore.config#L19) — 52 references
- [`conf/modules.config`](https://github.com/nf-core/viralrecon/blob/7cbb764e38012eb72a24c1a7a2d5db1e3251633a/conf/modules.config#L18) — 2 references
- [`modules/nf-core/pycoqc/tests/nextflow.config`](https://github.com/nf-core/viralrecon/blob/7cbb764e38012eb72a24c1a7a2d5db1e3251633a/modules/nf-core/pycoqc/tests/nextflow.config#L3) — 1 reference
