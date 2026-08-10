# Workflow outputs migration: stableexpression

- Generated: 2026-08-10T00:16:43.812643+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:123`](https://github.com/nf-core/stableexpression/blob/dfde809bd04f328e8421b044eec67a554cc9b220/main.nf#L123)

## Legacy `publishDir` references

Found 1 `publishDir` reference across 1 file that should be migrated to the workflow `output {}` block:

- [`tests/prepare_pr/.config`](https://github.com/nf-core/stableexpression/blob/dfde809bd04f328e8421b044eec67a554cc9b220/tests/prepare_pr/.config#L3) — 1 reference
