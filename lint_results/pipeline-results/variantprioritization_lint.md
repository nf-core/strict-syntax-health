# Nextflow lint results

- Generated: 2026-04-11T00:29:40.847320436Z
- Nextflow version: 26.03.2-edge
- Summary: 5 warnings

## :warning: Warnings

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

- Warning: `subworkflows/local/prepare_somatic/main.nf:68:5`: Variable was declared but not used

  ```nextflow
      pcgr_ready_vcf = PCGR_PREPAREVCF.out.vcf
      ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```
