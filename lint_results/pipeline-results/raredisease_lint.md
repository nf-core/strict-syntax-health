# Nextflow lint results

- Generated: 2026-06-30T00:40:58.776411966Z
- Nextflow version: 26.05.0-edge
- Summary: 13 warnings

## :warning: Warnings

- Warning: `subworkflows/local/annotate_mobile_elements/main.nf:74:9`: Emit name should be omitted when there is only one emit

  ```nextflow
          vcf_ann  = BCFTOOLS_VIEW_FILTER.out.vcf     // channel: [ val(meta), path(vcf) ]
          ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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

- Warning: `subworkflows/local/generate_cytosure_files/main.nf:94:9`: Emit name should be omitted when there is only one emit

  ```nextflow
          publish = ch_publish // channel: [ val(destination), val(value) ]
          ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/variant_evaluation/main.nf:59:9`: Emit name should be omitted when there is only one emit

  ```nextflow
          publish = ch_publish // channel: [ val(destination), val(value) ]
          ^^^^^^^^^^^^^^^^^^
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

- Warning: `workflows/raredisease.nf:245:5`: Variable was declared but not used

  ```nextflow
      ch_call_snv_publish                 = channel.empty()
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/raredisease.nf:997:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_config        = channel.fromPath(
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/raredisease.nf:999:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_custom_config = val_multiqc_config ?
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/raredisease.nf:1002:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_logo          = val_multiqc_logo ?
      ^^^^^^^^^^^^^^^
  ```
