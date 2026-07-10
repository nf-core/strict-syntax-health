# Workflow outputs migration: createtaxdb

- Generated: 2026-07-10T00:34:18.915519+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 17 `publishDir` references across 3 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/createtaxdb/blob/336763b0e0567be070b17a92ff71286d5574e2db/conf/modules.config#L15) — 15 references
- [`subworkflows/local/sourmash_create/tests/dna.config`](https://github.com/nf-core/createtaxdb/blob/336763b0e0567be070b17a92ff71286d5574e2db/subworkflows/local/sourmash_create/tests/dna.config#L4) — 1 reference
- [`subworkflows/local/sourmash_create/tests/protein.config`](https://github.com/nf-core/createtaxdb/blob/336763b0e0567be070b17a92ff71286d5574e2db/subworkflows/local/sourmash_create/tests/protein.config#L4) — 1 reference
