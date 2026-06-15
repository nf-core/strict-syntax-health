# Nextflow lint results

- Generated: 2026-06-15T00:46:19.976550+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/fastq_download_prefetch_fasterqdump_sratools/main.nf:32:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      reads    = SRATOOLS_FASTERQDUMP.out.reads // channel: [ val(meta), [ reads ] ]
      ^^^^^^^^^^
  ```
