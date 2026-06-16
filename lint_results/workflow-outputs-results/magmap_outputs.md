# Workflow outputs migration: magmap

- Generated: 2026-06-16T20:28:48.628685+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 27 `publishDir` references across 2 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/conf/modules.config#L15) — 26 references
- [`modules/nf-core/subread/featurecounts/tests/nextflow.config`](https://github.com/nf-core/magmap/blob/ee6503ef0f1daea9a4eee02ab12ec7b21295551b/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3) — 1 reference
