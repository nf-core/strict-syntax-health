# Workflow outputs migration: mspepid

- Generated: 2026-06-16T20:31:03.268846+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 9 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/mspepid/blob/6b5c623d878e520308eb0feb61d7ae36428f88d7/conf/modules.config#L15) — 6 references
- [`modules/local/cometconfig/main.nf`](https://github.com/nf-core/mspepid/blob/6b5c623d878e520308eb0feb61d7ae36428f88d7/modules/local/cometconfig/main.nf#L5) — 1 reference
- [`modules/local/ms2rescore/getmodel/main.nf`](https://github.com/nf-core/mspepid/blob/6b5c623d878e520308eb0feb61d7ae36428f88d7/modules/local/ms2rescore/getmodel/main.nf#L5) — 1 reference
- [`modules/local/psmutilsconversions/main.nf`](https://github.com/nf-core/mspepid/blob/6b5c623d878e520308eb0feb61d7ae36428f88d7/modules/local/psmutilsconversions/main.nf#L6) — 1 reference
