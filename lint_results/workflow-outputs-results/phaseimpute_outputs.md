# Workflow outputs migration: phaseimpute

- Generated: 2026-06-16T18:07:27.020895+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 84 `publishDir` references across 22 files that should be migrated to the workflow `output {}` block:

- [`conf/steps/panelprep.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/steps/panelprep.config#L16) — 13 references
- [`conf/steps/validation.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/steps/validation.config#L18) — 10 references
- [`conf/modules.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/modules.config#L15) — 7 references
- [`conf/steps/imputation_beagle5.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/steps/imputation_beagle5.config#L18) — 7 references
- [`conf/steps/imputation_glimpse2.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/steps/imputation_glimpse2.config#L16) — 6 references
- [`conf/steps/imputation_shared.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/steps/imputation_shared.config#L19) — 6 references
- [`conf/steps/simulation.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/steps/simulation.config#L16) — 5 references
- [`conf/steps/chrcheck.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/steps/chrcheck.config#L16) — 3 references
- [`conf/steps/imputation_glimpse1.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/steps/imputation_glimpse1.config#L18) — 3 references
- [`conf/steps/initialisation.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/steps/initialisation.config#L15) — 3 references
- [`workflows/phaseimpute/tests/nextflow.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/workflows/phaseimpute/tests/nextflow.config#L38) — 3 references
- [`conf/steps/imputation_minimac4.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/steps/imputation_minimac4.config#L15) — 2 references
- [`conf/steps/imputation_quilt.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/steps/imputation_quilt.config#L16) — 2 references
- [`conf/steps/imputation_quilt2.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/steps/imputation_quilt2.config#L10) — 2 references
- [`conf/steps/imputation_stitch.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/steps/imputation_stitch.config#L16) — 2 references
- [`conf/test_all.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/test_all.config#L53) — 2 references
- [`conf/test_dog.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/test_dog.config#L51) — 2 references
- [`conf/test_panelprep.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/test_panelprep.config#L48) — 2 references
- [`conf/test_full.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/conf/test_full.config#L46) — 1 reference
- [`nextflow.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/nextflow.config#L105) — 1 reference
- [`subworkflows/nf-core/bam_impute_quilt/tests/nextflow.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/subworkflows/nf-core/bam_impute_quilt/tests/nextflow.config#L14) — 1 reference
- [`tests/nextflow.config`](https://github.com/nf-core/phaseimpute/blob/71cb181f1254459c4fad2e185d173ab23ecd4d67/tests/nextflow.config#L19) — 1 reference
