# Nextflow lint results

- Generated: 2026-05-24T00:38:50.927979+00:00
- Nextflow version: 26.04.2
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_markduplicates_samtools/main.nf:31:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      bam = SAMTOOLS_MARKDUP.out.bam // channel: [ val(meta), [ bam ] ]
      ^^^^^^^^^^
  ```
