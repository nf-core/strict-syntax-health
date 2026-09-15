# Workflow outputs migration: abotyper

- Generated: 2026-09-15T00:19:37.499363+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 12 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/abotyper/blob/427b3356bb2b7f308ff7bbee59f99240f715dcd3/conf/modules.config#L14) — 11 references
- [`modules/local/abo/snps2pheno/main.nf`](https://github.com/nf-core/abotyper/blob/427b3356bb2b7f308ff7bbee59f99240f715dcd3/modules/local/abo/snps2pheno/main.nf#L10) — 1 reference
