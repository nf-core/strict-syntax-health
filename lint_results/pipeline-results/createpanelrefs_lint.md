# Nextflow lint results

- Generated: 2026-06-16T19:20:30.833201181Z
- Nextflow version: 26.04.3
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/local/prepare_alignment/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      reads_index = ch_reads_index // [ val(meta), path(bam|cram), path(bai|crai) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_createpanelrefs_pipeline/main.nf:171:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      samplesheet = ch_samplesheet
      ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
