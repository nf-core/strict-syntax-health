# Nextflow lint results

- Generated: 2026-07-07T00:36:54.981645705Z
- Nextflow version: 26.06.0-edge
- Summary: 19 warnings

## :warning: Warnings

- Warning: `subworkflows/local/annotate_mobile_elements/main.nf:74:9`: Emit name should be omitted when there is only one emit

  ```nextflow
          vcf_ann  = BCFTOOLS_VIEW_FILTER.out.vcf     // channel: [ val(meta), path(vcf) ]
          ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/call_snv_sentieon/main.nf:67:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def sorted = [vcfs, idxs].transpose().sort { it[0].name }
                                                               ^^
  ```

- Warning: `subworkflows/local/call_snv_sentieon/main.nf:68:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  return [meta, sorted.collect { it[0] }, sorted.collect { it[1] }]
                                                 ^^
  ```

- Warning: `subworkflows/local/call_snv_sentieon/main.nf:68:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  return [meta, sorted.collect { it[0] }, sorted.collect { it[1] }]
                                                                           ^^
  ```

- Warning: `subworkflows/local/call_sv_MT/main.nf:145:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .filter { !it.isEmpty() }
                             ^^
  ```

- Warning: `subworkflows/local/call_sv_cnvnator/main.nf:44:9`: Emit name should be omitted when there is only one emit

  ```nextflow
          vcf        = SVDB_MERGE_CNVNATOR.out.vcf  // channel: [ val(meta), path(*.tar.gz) ]
          ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/call_sv_tiddit/main.nf:35:9`: Emit name should be omitted when there is only one emit

  ```nextflow
          vcf      = SVDB_MERGE_TIDDIT.out.vcf // channel: [ val(meta), path(vcf) ]
          ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/contamination_check/main.nf:32:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { vcf, tbi -> vcf }
                      ^^^
  ```

- Warning: `subworkflows/local/contamination_check/main.nf:36:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { vcf, tbi -> tbi }
                 ^^^
  ```

- Warning: `subworkflows/local/generate_cytosure_files/main.nf:91:9`: Emit name should be omitted when there is only one emit

  ```nextflow
          cgh = VCF2CYTOSURE.out.cgh // channel: [ val(meta), path(cgh) ]
          ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      valid_config = valid_config
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/raredisease.nf:433:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_contamination_mqc    = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `workflows/raredisease.nf:434:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_contamination_table  = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `workflows/raredisease.nf:435:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_contamination_pileup = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `workflows/raredisease.nf:1069:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_config        = channel.fromPath(
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/raredisease.nf:1071:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_custom_config = val_multiqc_config ?
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/raredisease.nf:1074:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_logo          = val_multiqc_logo ?
      ^^^^^^^^^^^^^^^
  ```
