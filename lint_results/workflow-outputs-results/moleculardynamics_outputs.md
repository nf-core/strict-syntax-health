# Workflow outputs migration: moleculardynamics

- Generated: 2026-10-13T00:26:53.885957+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 10 `publishDir` references across 10 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/moleculardynamics/blob/c94861ceb7665b22ac1789bb3257ae8da6b6643f/conf/modules.config#L15) — 1 reference
- [`modules/local/analysis_rmsd.nf`](https://github.com/nf-core/moleculardynamics/blob/c94861ceb7665b22ac1789bb3257ae8da6b6643f/modules/local/analysis_rmsd.nf#L21) — 1 reference
- [`modules/local/post_processing.nf`](https://github.com/nf-core/moleculardynamics/blob/c94861ceb7665b22ac1789bb3257ae8da6b6643f/modules/local/post_processing.nf#L21) — 1 reference
- [`modules/local/pre_pos_clean_pdb.nf`](https://github.com/nf-core/moleculardynamics/blob/c94861ceb7665b22ac1789bb3257ae8da6b6643f/modules/local/pre_pos_clean_pdb.nf#L21) — 1 reference
- [`modules/local/run_energy_min.nf`](https://github.com/nf-core/moleculardynamics/blob/c94861ceb7665b22ac1789bb3257ae8da6b6643f/modules/local/run_energy_min.nf#L20) — 1 reference
- [`modules/local/run_npt_equilibration.nf`](https://github.com/nf-core/moleculardynamics/blob/c94861ceb7665b22ac1789bb3257ae8da6b6643f/modules/local/run_npt_equilibration.nf#L20) — 1 reference
- [`modules/local/run_nvt_equilibration.nf`](https://github.com/nf-core/moleculardynamics/blob/c94861ceb7665b22ac1789bb3257ae8da6b6643f/modules/local/run_nvt_equilibration.nf#L20) — 1 reference
- [`modules/local/run_production.nf`](https://github.com/nf-core/moleculardynamics/blob/c94861ceb7665b22ac1789bb3257ae8da6b6643f/modules/local/run_production.nf#L21) — 1 reference
- [`modules/local/run_solvation.nf`](https://github.com/nf-core/moleculardynamics/blob/c94861ceb7665b22ac1789bb3257ae8da6b6643f/modules/local/run_solvation.nf#L24) — 1 reference
- [`modules/local/run_topology.nf`](https://github.com/nf-core/moleculardynamics/blob/c94861ceb7665b22ac1789bb3257ae8da6b6643f/modules/local/run_topology.nf#L22) — 1 reference
