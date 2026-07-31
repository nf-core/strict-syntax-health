# Workflow outputs migration: magmap

- Generated: 2026-07-31T00:32:20.230587+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 25 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/magmap/blob/dbffd1e587e5713cf101b50cc766ce1b605d27f7/conf/modules.config#L15) — 24 references
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/magmap/blob/dbffd1e587e5713cf101b50cc766ce1b605d27f7/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
