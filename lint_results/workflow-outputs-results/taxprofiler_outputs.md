# Workflow outputs migration: taxprofiler

- Generated: 2026-10-04T01:01:57.498439+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 90 `publishDir` references across 9 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/taxprofiler/blob/3b8595987edec10bd4aff0d9dcecfb93c850871e/conf/modules.config#L15) — 72 references
- [`conf/test.config`](https://github.com/nf-core/taxprofiler/blob/3b8595987edec10bd4aff0d9dcecfb93c850871e/conf/test.config#L69) — 3 references
- [`conf/test_fastpnonpareilkrakenuniq.config`](https://github.com/nf-core/taxprofiler/blob/3b8595987edec10bd4aff0d9dcecfb93c850871e/conf/test_fastpnonpareilkrakenuniq.config#L76) — 3 references
- [`conf/test_alternativepreprocessing.config`](https://github.com/nf-core/taxprofiler/blob/3b8595987edec10bd4aff0d9dcecfb93c850871e/conf/test_alternativepreprocessing.config#L65) — 2 references
- [`conf/test_falcobbduk.config`](https://github.com/nf-core/taxprofiler/blob/3b8595987edec10bd4aff0d9dcecfb93c850871e/conf/test_falcobbduk.config#L64) — 2 references
- [`conf/test_malt.config`](https://github.com/nf-core/taxprofiler/blob/3b8595987edec10bd4aff0d9dcecfb93c850871e/conf/test_malt.config#L64) — 2 references
- [`conf/test_minimal.config`](https://github.com/nf-core/taxprofiler/blob/3b8595987edec10bd4aff0d9dcecfb93c850871e/conf/test_minimal.config#L60) — 2 references
- [`conf/test_motus.config`](https://github.com/nf-core/taxprofiler/blob/3b8595987edec10bd4aff0d9dcecfb93c850871e/conf/test_motus.config#L69) — 2 references
- [`conf/test_nopreprocessing.config`](https://github.com/nf-core/taxprofiler/blob/3b8595987edec10bd4aff0d9dcecfb93c850871e/conf/test_nopreprocessing.config#L63) — 2 references
