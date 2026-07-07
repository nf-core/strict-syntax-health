# Workflow outputs migration: phaseimpute

- Generated: 2026-07-07T00:36:17.466452+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 90 `publishDir` references across 20 files that should be migrated to the workflow `output {}` block:

- [`conf/steps/panelprep.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/steps/panelprep.config#L16) — 14 references
- [`conf/steps/validation.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/steps/validation.config#L18) — 10 references
- [`conf/steps/imputation_beagle5.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/steps/imputation_beagle5.config#L18) — 8 references
- [`conf/modules.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/modules.config#L15) — 7 references
- [`conf/steps/imputation_glimpse2.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/steps/imputation_glimpse2.config#L16) — 7 references
- [`conf/steps/imputation_shared.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/steps/imputation_shared.config#L19) — 6 references
- [`conf/steps/simulation.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/steps/simulation.config#L16) — 5 references
- [`conf/steps/imputation_glimpse1.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/steps/imputation_glimpse1.config#L18) — 4 references
- [`conf/steps/chrcheck.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/steps/chrcheck.config#L16) — 3 references
- [`conf/steps/imputation_minimac4.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/steps/imputation_minimac4.config#L15) — 3 references
- [`conf/steps/imputation_quilt.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/steps/imputation_quilt.config#L16) — 3 references
- [`conf/steps/imputation_quilt2.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/steps/imputation_quilt2.config#L10) — 3 references
- [`conf/steps/imputation_stitch.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/steps/imputation_stitch.config#L16) — 3 references
- [`conf/steps/initialisation.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/steps/initialisation.config#L15) — 3 references
- [`tests/nextflow.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/tests/nextflow.config#L44) — 3 references
- [`conf/test_all.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/test_all.config#L53) — 2 references
- [`conf/test_dog.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/test_dog.config#L51) — 2 references
- [`conf/test_panelprep.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/test_panelprep.config#L48) — 2 references
- [`conf/test_full.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/conf/test_full.config#L46) — 1 reference
- [`subworkflows/nf-core/bam_impute_quilt/tests/nextflow.config`](https://github.com/nf-core/phaseimpute/blob/903ec4481327346004c52f4eaa646f49b2581e06/subworkflows/nf-core/bam_impute_quilt/tests/nextflow.config#L14) — 1 reference
