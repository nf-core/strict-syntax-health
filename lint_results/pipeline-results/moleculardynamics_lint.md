# Nextflow lint results

- Generated: 2026-10-20T00:20:07.167239746Z
- Nextflow version: 26.10.2
- Summary: 28 errors, 6 warnings

## :x: Errors

- Error: `modules/local/pre_pos_check_missing_atoms.nf:30:32`: Unexpected input: '\n'

  ```nextflow
                emit: checked_pdb
                                 ^
  ```

- Error: `modules/local/pre_pos_clean_pdb.nf:27:170`: Unexpected input: 'into'

  ```nextflow
          tuple val(sample), path("${sample}_cleaned.pdb"), val(forcefield), val(box_type), val(distance_to_box), path(em_mdp), path(nvt_mdp), path(npt_mdp), path(md_mdp) into cleaned_pdb
                                                                                                                                                                           ^
  ```

- Error: `modules/local/run_energy_min.nf:34:30`: Unexpected input: '\n'

  ```nextflow
          emit:  energy_min_out
                               ^
  ```

- Error: `modules/local/run_npt_equilibration.nf:35:36`: Unexpected input: '\n'

  ```nextflow
          emit: npt_equilibration_out
                                     ^
  ```

- Error: `modules/local/run_nvt_equilibration.nf:34:36`: Unexpected input: '\n'

  ```nextflow
          emit: nvt_equilibration_out
                                     ^
  ```

- Error: `modules/local/run_production.nf:35:25`: Unexpected input: '\n'

  ```nextflow
      emit: production_out
                          ^
  ```

- Error: `modules/local/run_solvation.nf:39:28`: Unexpected input: '\n'

  ```nextflow
          emit: solvation_out
                             ^
  ```

- Error: `modules/local/run_topology.nf:25:154`: Unexpected input: 'into'

  ```nextflow
      tuple val(sample), path(checked_pdb), val(forcefield), val(box_type), val(distance_to_box), path(em_mdp), path(nvt_mdp), path(npt_mdp), path(md_mdp) into checked_pdb
                                                                                                                                                           ^
  ```

- Error: `subworkflows/local/pre_processing/main.nf:3:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/moleculardynamics/modules/local/pre_pos_clean_pdb.nf'

  ```nextflow
  include { PRE_POS_CLEAN_PDB }         from '../../../modules/local/pre_pos_clean_pdb.nf'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/pre_processing/main.nf:4:1`: Included name 'PRE_POS_CHECK_MISSING_ATOMS' is not defined in module '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/moleculardynamics/modules/local/pre_pos_check_missing_atoms.nf'

  ```nextflow
  include { PRE_POS_CHECK_MISSING_ATOMS } from '../../../modules/local/pre_pos_check_missing_atoms.nf'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/pre_processing/main.nf:12:16`: `PRE_POS_CLEAN_PDB` is not defined

  ```nextflow
      ch_clean = PRE_POS_CLEAN_PDB(ch_inputs, outdir)
                 ^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/pre_processing/main.nf:13:16`: `PRE_POS_CHECK_MISSING_ATOMS` is not defined

  ```nextflow
      ch_check = PRE_POS_CHECK_MISSING_ATOMS(ch_clean.cleaned)
                 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/run_md/main.nf:4:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/moleculardynamics/modules/local/run_topology.nf'

  ```nextflow
  include { RUN_TOPOLOGY } from '../../../modules/local/run_topology.nf'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/run_md/main.nf:5:1`: Included name 'RUN_SOLVATION' is not defined in module '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/moleculardynamics/modules/local/run_solvation.nf'

  ```nextflow
  include { RUN_SOLVATION } from '../../../modules/local/run_solvation.nf'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/run_md/main.nf:6:1`: Included name 'RUN_ENERGY_MINIMISATION' is not defined in module '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/moleculardynamics/modules/local/run_energy_min.nf'

  ```nextflow
  include { RUN_ENERGY_MINIMISATION } from '../../../modules/local/run_energy_min.nf'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/run_md/main.nf:7:1`: Included name 'RUN_NVT_EQUILIBRATION' is not defined in module '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/moleculardynamics/modules/local/run_nvt_equilibration.nf'

  ```nextflow
  include { RUN_NVT_EQUILIBRATION } from '../../../modules/local/run_nvt_equilibration.nf'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/run_md/main.nf:8:1`: Included name 'RUN_NPT_EQUILIBRATION' is not defined in module '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/moleculardynamics/modules/local/run_npt_equilibration.nf'

  ```nextflow
  include { RUN_NPT_EQUILIBRATION } from '../../../modules/local/run_npt_equilibration.nf'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/run_md/main.nf:9:1`: Included name 'RUN_PRODUCTION' is not defined in module '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/moleculardynamics/modules/local/run_production.nf'

  ```nextflow
  include { RUN_PRODUCTION } from '../../../modules/local/run_production.nf'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/run_md/main.nf:19:27`: `RUN_TOPOLOGY` is not defined

  ```nextflow
      topology_out        = RUN_TOPOLOGY(ch_preprocessing, force_field, outdir)
                            ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/run_md/main.nf:19:58`: `force_field` is not defined

  ```nextflow
      topology_out        = RUN_TOPOLOGY(ch_preprocessing, force_field, outdir)
                                                           ^^^^^^^^^^^
  ```

- Error: `subworkflows/local/run_md/main.nf:22:30`: `RUN_SOLVATION` is not defined

  ```nextflow
      solvation_out          = RUN_SOLVATION(topology_out, outdir)
                               ^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/run_md/main.nf:26:27`: `RUN_ENERGY_MINIMISATION` is not defined

  ```nextflow
      energy_min_out      = RUN_ENERGY_MINIMISATION(solvation_out, outdir)
                            ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/run_md/main.nf:29:30`: `RUN_NVT_EQUILIBRATION` is not defined

  ```nextflow
      nvt_equilibration_out  = RUN_NVT_EQUILIBRATION(energy_min_out, outdir)
                               ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/run_md/main.nf:32:29`: `RUN_NPT_EQUILIBRATION` is not defined

  ```nextflow
      npt_equilibration_out = RUN_NPT_EQUILIBRATION(nvt_equilibration_out, outdir)
                              ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/run_md/main.nf:35:27`: `RUN_PRODUCTION` is not defined

  ```nextflow
      production_run_out  = RUN_PRODUCTION(npt_equilibration_out, outdir)
                            ^^^^^^^^^^^^^^
  ```

- Error: `workflows/moleculardynamics.nf:77:41`: `ch_postprocessed_gro` is not defined

  ```nextflow
      ANALYSIS_RMSD(ch_postprocessed_xtc, ch_postprocessed_gro, ch_postprocessed_tpr, params.outdir)
                                          ^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/moleculardynamics.nf:77:63`: `ch_postprocessed_tpr` is not defined

  ```nextflow
      ANALYSIS_RMSD(ch_postprocessed_xtc, ch_postprocessed_gro, ch_postprocessed_tpr, params.outdir)
                                                                ^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/moleculardynamics.nf:113:31`: `ch_cleaned_pdb` is not defined

  ```nextflow
      cleaned_pdb             = ch_cleaned_pdb              // channel: [ tuple(sample_id, path(cleaned_pdb)) ]
                                ^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `workflows/moleculardynamics.nf:30:94`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      paramsSummaryMap(params, methodsDescriptionText(params)).view { "📝 Pipeline parameters:\n$it" }
                                                                                               ^^
  ```

- Warning: `workflows/moleculardynamics.nf:49:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_inputs.view { "📦 Parsed sample inputs: $it" }
                                                ^^
  ```

- Warning: `workflows/moleculardynamics.nf:56:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      PRE_PROCESSING.out.cleaned_pdb.view { "✅ Cleaned PDB ready: $it" }
                                                                  ^^
  ```

- Warning: `workflows/moleculardynamics.nf:62:102`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      RUN_MD_SIMULATION.out.md_report.view { "✅ Production run completed! You can see the report here: $it" }
                                                                                                       ^^
  ```

- Warning: `workflows/moleculardynamics.nf:71:112`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      POST_PROCESSING.out.postprocessed_report.view { "✅ Post-processing completed! You can see the report here: $it" }
                                                                                                                 ^^
  ```

- Warning: `workflows/moleculardynamics.nf:78:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ANALYSIS_RMSD.out.rmsd_xvg.view { "✅ RMSD analysis completed: $it" }
                                                                    ^^
  ```
