# Workflow outputs migration: abotyper

- Generated: 2026-07-31T00:30:11.455706+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 14 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/abotyper/blob/3a9a73a91b798ef2c17a48dc1104c4e7e1799d08/conf/modules.config#L14) — 13 references
- [`modules/local/abo/snps2pheno/main.nf`](https://github.com/nf-core/abotyper/blob/3a9a73a91b798ef2c17a48dc1104c4e7e1799d08/modules/local/abo/snps2pheno/main.nf#L10) — 1 reference
