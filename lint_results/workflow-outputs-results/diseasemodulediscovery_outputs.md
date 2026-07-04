# Workflow outputs migration: diseasemodulediscovery

- Generated: 2026-07-04T00:33:04.553726+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 21 `publishDir` references across 1 file that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/diseasemodulediscovery/blob/7bd8389c99966b769bf0370f6b85aeba24eb8a44/conf/modules.config#L17) — 21 references
