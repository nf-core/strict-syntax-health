# Workflow outputs migration: diseasemodulediscovery

- Generated: 2026-08-18T00:12:34.639704+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 19 `publishDir` references across 1 file that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/diseasemodulediscovery/blob/6b729f4fe6ea395a2845a45e0ce007a73e3fc001/conf/modules.config#L17) — 19 references
