# Workflow outputs migration: stableexpression

- Generated: 2026-06-16T19:45:07.946756+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 15 `publishDir` references across 5 files that should be migrated to the workflow `output {}` block:

- [`conf/modules/public_data.config`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/public_data.config#L4) — 4 references
- [`conf/modules/id_mapping.config`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/id_mapping.config#L4) — 3 references
- [`conf/modules/normalisation.config`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/normalisation.config#L4) — 3 references
- [`conf/modules/reporting.config`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/reporting.config#L4) — 3 references
- [`conf/modules/gene_length.config`](https://github.com/nf-core/stableexpression/blob/3c5669a174e0490923b094c1a72cd0523f71acf2/conf/modules/gene_length.config#L4) — 2 references
