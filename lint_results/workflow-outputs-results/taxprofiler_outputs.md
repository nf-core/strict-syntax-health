# Workflow outputs migration: taxprofiler

- Generated: 2026-06-16T19:45:29.489339+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 82 `publishDir` references across 10 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L15) — 63 references
- [`conf/test.config`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test.config#L67) — 3 references
- [`conf/test_fastpnonpareilkrakenuniq.config`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_fastpnonpareilkrakenuniq.config#L73) — 3 references
- [`conf/test_alternativepreprocessing.config`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_alternativepreprocessing.config#L62) — 2 references
- [`conf/test_falcobbduk.config`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_falcobbduk.config#L61) — 2 references
- [`conf/test_malt.config`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_malt.config#L63) — 2 references
- [`conf/test_minimal.config`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_minimal.config#L59) — 2 references
- [`conf/test_motus.config`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_motus.config#L68) — 2 references
- [`conf/test_nopreprocessing.config`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_nopreprocessing.config#L62) — 2 references
- [`modules/nf-core/nonpareil/nonpareil/tests/nextflow.config`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/modules/nf-core/nonpareil/nonpareil/tests/nextflow.config#L3) — 1 reference
