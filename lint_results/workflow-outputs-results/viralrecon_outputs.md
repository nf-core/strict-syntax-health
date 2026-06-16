# Workflow outputs migration: viralrecon

- Generated: 2026-06-16T20:45:51.665738+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 173 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/modules_illumina.config`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L19) — 117 references
- [`conf/modules_nanopore.config`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L19) — 53 references
- [`conf/modules.config`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules.config#L18) — 2 references
- [`modules/nf-core/pycoqc/tests/nextflow.config`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/modules/nf-core/pycoqc/tests/nextflow.config#L3) — 1 reference
