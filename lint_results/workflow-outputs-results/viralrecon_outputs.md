# Workflow outputs migration: viralrecon

- Generated: 2026-11-28T00:15:21.671598+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 171 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/modules_illumina.config`](https://github.com/nf-core/viralrecon/blob/90316c62438fc5f22b9ec49893e6fa31982a4c16/conf/modules_illumina.config#L19) — 116 references
- [`conf/modules_nanopore.config`](https://github.com/nf-core/viralrecon/blob/90316c62438fc5f22b9ec49893e6fa31982a4c16/conf/modules_nanopore.config#L19) — 52 references
- [`conf/modules.config`](https://github.com/nf-core/viralrecon/blob/90316c62438fc5f22b9ec49893e6fa31982a4c16/conf/modules.config#L18) — 2 references
- [`modules/nf-core/pycoqc/tests/nextflow.config`](https://github.com/nf-core/viralrecon/blob/90316c62438fc5f22b9ec49893e6fa31982a4c16/modules/nf-core/pycoqc/tests/nextflow.config#L3) — 1 reference
