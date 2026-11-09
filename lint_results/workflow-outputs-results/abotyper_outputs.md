# Workflow outputs migration: abotyper

- Generated: 2026-11-09T00:12:43.764006+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 20 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/abotyper/blob/b90cc3fff3cba31f9b2973de8e065052282885a4/conf/modules.config#L14) — 19 references
- [`modules/local/abo/snps2pheno/main.nf`](https://github.com/nf-core/abotyper/blob/b90cc3fff3cba31f9b2973de8e065052282885a4/modules/local/abo/snps2pheno/main.nf#L20) — 1 reference
