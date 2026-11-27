# Workflow outputs migration: moleculardynamics

- Generated: 2026-11-27T00:13:09.152979+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 11 `publishDir` references across 11 files that should be migrated to the workflow `output {}` block:

- [`conf/modules.config`](https://github.com/nf-core/moleculardynamics/blob/a10294901c3f87ded7229c1c7656e27e6ccc39c9/conf/modules.config#L19) — 1 reference
- [`modules/local/analysis_rmsd.nf`](https://github.com/nf-core/moleculardynamics/blob/a10294901c3f87ded7229c1c7656e27e6ccc39c9/modules/local/analysis_rmsd.nf#L23) — 1 reference
- [`modules/local/post_processing.nf`](https://github.com/nf-core/moleculardynamics/blob/a10294901c3f87ded7229c1c7656e27e6ccc39c9/modules/local/post_processing.nf#L22) — 1 reference
- [`modules/local/pre_pos_check_missing_atoms.nf`](https://github.com/nf-core/moleculardynamics/blob/a10294901c3f87ded7229c1c7656e27e6ccc39c9/modules/local/pre_pos_check_missing_atoms.nf#L23) — 1 reference
- [`modules/local/pre_pos_clean_pdb.nf`](https://github.com/nf-core/moleculardynamics/blob/a10294901c3f87ded7229c1c7656e27e6ccc39c9/modules/local/pre_pos_clean_pdb.nf#L23) — 1 reference
- [`modules/local/run_energy_min.nf`](https://github.com/nf-core/moleculardynamics/blob/a10294901c3f87ded7229c1c7656e27e6ccc39c9/modules/local/run_energy_min.nf#L21) — 1 reference
- [`modules/local/run_npt_equilibration.nf`](https://github.com/nf-core/moleculardynamics/blob/a10294901c3f87ded7229c1c7656e27e6ccc39c9/modules/local/run_npt_equilibration.nf#L21) — 1 reference
- [`modules/local/run_nvt_equilibration.nf`](https://github.com/nf-core/moleculardynamics/blob/a10294901c3f87ded7229c1c7656e27e6ccc39c9/modules/local/run_nvt_equilibration.nf#L21) — 1 reference
- [`modules/local/run_production.nf`](https://github.com/nf-core/moleculardynamics/blob/a10294901c3f87ded7229c1c7656e27e6ccc39c9/modules/local/run_production.nf#L23) — 1 reference
- [`modules/local/run_solvation.nf`](https://github.com/nf-core/moleculardynamics/blob/a10294901c3f87ded7229c1c7656e27e6ccc39c9/modules/local/run_solvation.nf#L25) — 1 reference
- [`modules/local/run_topology.nf`](https://github.com/nf-core/moleculardynamics/blob/a10294901c3f87ded7229c1c7656e27e6ccc39c9/modules/local/run_topology.nf#L23) — 1 reference
