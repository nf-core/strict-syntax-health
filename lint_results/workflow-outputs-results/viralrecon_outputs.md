# Workflow outputs migration: viralrecon

- Generated: 2026-11-17T00:17:30.894965+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 169 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/modules_illumina.config`](https://github.com/nf-core/viralrecon/blob/31b9515f6e166542ca60358931351aa0f9a72b8a/conf/modules_illumina.config#L19) — 114 references
- [`conf/modules_nanopore.config`](https://github.com/nf-core/viralrecon/blob/31b9515f6e166542ca60358931351aa0f9a72b8a/conf/modules_nanopore.config#L19) — 52 references
- [`conf/modules.config`](https://github.com/nf-core/viralrecon/blob/31b9515f6e166542ca60358931351aa0f9a72b8a/conf/modules.config#L18) — 2 references
- [`modules/nf-core/pycoqc/tests/nextflow.config`](https://github.com/nf-core/viralrecon/blob/31b9515f6e166542ca60358931351aa0f9a72b8a/modules/nf-core/pycoqc/tests/nextflow.config#L3) — 1 reference
