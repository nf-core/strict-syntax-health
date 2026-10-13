# Workflow outputs migration: pacvar

- Generated: 2026-10-13T00:27:05.006737+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 14 `publishDir` references across 4 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/pacvar/blob/665d69635d2e99273067af5e5b69c552b44e0858/conf/modules.config#L14) — 8 references
- [`conf/modules/ensemblvep.config`](https://github.com/nf-core/pacvar/blob/665d69635d2e99273067af5e5b69c552b44e0858/conf/modules/ensemblvep.config#L18) — 4 references
- [`conf/modules/fibertools.config`](https://github.com/nf-core/pacvar/blob/665d69635d2e99273067af5e5b69c552b44e0858/conf/modules/fibertools.config#L3) — 1 reference
- [`modules/nf-core/lima/tests/nextflow.config`](https://github.com/nf-core/pacvar/blob/665d69635d2e99273067af5e5b69c552b44e0858/modules/nf-core/lima/tests/nextflow.config#L3) — 1 reference
