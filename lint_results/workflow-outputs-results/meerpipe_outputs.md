# Workflow outputs migration: meerpipe

- Generated: 2026-11-13T00:16:02.118600+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 9 `publishDir` references across 5 files that should be migrated to the workflow `output {}` block:

- [`modules/local/generate_image_results.nf`](https://github.com/nf-core/meerpipe/blob/c77cdd4e5d0507e0b4ce7862d0a9bc8bd9a6bfb0/modules/local/generate_image_results.nf#L7) — 3 references
- [`conf/modules.config`](https://github.com/nf-core/meerpipe/blob/c77cdd4e5d0507e0b4ce7862d0a9bc8bd9a6bfb0/conf/modules.config#L16) — 2 references
- [`modules/local/psradd_calibrate_clean.nf`](https://github.com/nf-core/meerpipe/blob/c77cdd4e5d0507e0b4ce7862d0a9bc8bd9a6bfb0/modules/local/psradd_calibrate_clean.nf#L7) — 2 references
- [`modules/local/decimate.nf`](https://github.com/nf-core/meerpipe/blob/c77cdd4e5d0507e0b4ce7862d0a9bc8bd9a6bfb0/modules/local/decimate.nf#L7) — 1 reference
- [`modules/local/generate_toas.nf`](https://github.com/nf-core/meerpipe/blob/c77cdd4e5d0507e0b4ce7862d0a9bc8bd9a6bfb0/modules/local/generate_toas.nf#L6) — 1 reference
