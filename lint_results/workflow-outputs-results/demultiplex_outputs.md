# Workflow outputs migration: demultiplex

- Generated: 2026-06-16T19:22:38.522924+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:128`](https://github.com/nf-core/demultiplex/blob/257df49988d242fabb42b6d87fb1e3a69c39789f/main.nf#L128)

## Legacy `publishDir` references

Found 6 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/test.config`](https://github.com/nf-core/demultiplex/blob/257df49988d242fabb42b6d87fb1e3a69c39789f/conf/test.config#L38) — 2 references
- [`conf/test_uncompressed.config`](https://github.com/nf-core/demultiplex/blob/257df49988d242fabb42b6d87fb1e3a69c39789f/conf/test_uncompressed.config#L39) — 2 references
- [`conf/test_flowcell.config`](https://github.com/nf-core/demultiplex/blob/257df49988d242fabb42b6d87fb1e3a69c39789f/conf/test_flowcell.config#L39) — 1 reference
- [`modules/nf-core/bcl2fastq/tests/nextflow.config`](https://github.com/nf-core/demultiplex/blob/257df49988d242fabb42b6d87fb1e3a69c39789f/modules/nf-core/bcl2fastq/tests/nextflow.config#L3) — 1 reference
