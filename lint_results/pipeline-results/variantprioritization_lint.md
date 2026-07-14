# Nextflow lint results

- Generated: 2026-07-14T00:28:23.023914025Z
- Nextflow version: 26.06.0-edge
- Summary: 11 warnings

## :warning: Warnings

- Warning: `main.nf:49:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = VARIANTPRIORITIZATION.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/input_preprocessing/main.nf:26:5`: Variable was declared but not used

  ```nextflow
      ch_cna_files = ch_samplesheet
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/input_preprocessing/main.nf:68:5`: Variable was declared but not used

  ```nextflow
      normalised_germline = ch_filtered.filter { meta, _vcf, _tbi -> meta.status == 'germline' }
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/input_preprocessing/main.nf:69:5`: Variable was declared but not used

  ```nextflow
      normalised_somatic = ch_filtered.filter { meta, _vcf, _tbi -> meta.status == 'somatic' }
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_somatic/main.nf:72:5`: Variable was declared but not used

  ```nextflow
      pcgr_ready_vcf = PCGR_PREPAREVCF.out.vcf
      ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_somatic/main.nf:79:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      pcgr_ready_vcf
      ^^^^^^^^^^^^^^
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

- Warning: `workflows/variantprioritization/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      multiqc_methods_description
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/variantprioritization/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      outdir
      ^^^^^^
  ```
