# Workflow outputs migration: abotyper

- Generated: 2026-10-15T00:17:43.989190+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 19 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/abotyper/blob/6d2eb3a12457050743afce31ddb520b650da0c29/conf/modules.config#L14) — 18 references
- [`modules/local/abo/snps2pheno/main.nf`](https://github.com/nf-core/abotyper/blob/6d2eb3a12457050743afce31ddb520b650da0c29/modules/local/abo/snps2pheno/main.nf#L20) — 1 reference
