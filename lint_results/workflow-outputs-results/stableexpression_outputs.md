# Workflow outputs migration: stableexpression

- Generated: 2026-06-30T00:42:29.310846+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:126`](https://github.com/nf-core/stableexpression/blob/f1854a49a3f5ba6fbe297ba7496de6c5835bdb7b/main.nf#L126)

## Legacy `publishDir` references

Found 1 `publishDir` reference across 1 file that should be migrated to the workflow `output {}` block:

- [`tests/prepare_pr/.config`](https://github.com/nf-core/stableexpression/blob/f1854a49a3f5ba6fbe297ba7496de6c5835bdb7b/tests/prepare_pr/.config#L3) — 1 reference
