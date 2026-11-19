# Nextflow lint results

- Generated: 2026-11-19T00:14:36.341913509Z
- Nextflow version: 26.11.0-edge
- Summary: 10 warnings

## :warning: Warnings

- Warning: `subworkflows/local/run_md/main.nf:37:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      md_tpr    = RUN_PRODUCTION.out.production_out.map { tuple(it[0], it[1]) }
                                                                ^^
  ```

- Warning: `subworkflows/local/run_md/main.nf:37:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      md_tpr    = RUN_PRODUCTION.out.production_out.map { tuple(it[0], it[1]) }
                                                                       ^^
  ```

- Warning: `subworkflows/local/run_md/main.nf:38:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      md_gro    = RUN_PRODUCTION.out.production_out.map { tuple(it[0], it[2]) }
                                                                ^^
  ```

- Warning: `subworkflows/local/run_md/main.nf:38:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      md_gro    = RUN_PRODUCTION.out.production_out.map { tuple(it[0], it[2]) }
                                                                       ^^
  ```

- Warning: `subworkflows/local/run_md/main.nf:39:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      md_xtc    = RUN_PRODUCTION.out.production_out.map { tuple(it[0], it[3]) }
                                                                ^^
  ```

- Warning: `subworkflows/local/run_md/main.nf:39:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      md_xtc    = RUN_PRODUCTION.out.production_out.map { tuple(it[0], it[3]) }
                                                                       ^^
  ```

- Warning: `workflows/moleculardynamics.nf:41:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_inputs.view { "📦 Parsed sample inputs: $it" }
                                                ^^
  ```

- Warning: `workflows/moleculardynamics.nf:48:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      PRE_PROCESSING.out.cleaned_pdb.view { "✅ Cleaned PDB ready: $it" }
                                                                  ^^
  ```

- Warning: `workflows/moleculardynamics.nf:56:5`: Variable was declared but not used

  ```nextflow
      ch_md_gro = RUN_MD_SIMULATION.out.md_gro    // tuple(sample, gro)
      ^^^^^^^^^
  ```

- Warning: `workflows/moleculardynamics.nf:72:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ANALYSIS_RMSD.out.rmsd_xvg.view { "✅ RMSD analysis completed: $it" }
                                                                    ^^
  ```
