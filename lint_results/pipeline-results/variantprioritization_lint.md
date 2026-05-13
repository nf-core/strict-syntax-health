# Nextflow lint results

- Generated: 2026-05-13T00:41:25.636559246Z
- Nextflow version: 26.04.1
- Summary: 6 warnings

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
