# Nextflow lint results

- Generated: 2026-07-10T00:38:53.784312+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_markduplicates_samtools/main.nf:31:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      bam = SAMTOOLS_MARKDUP.out.bam // channel: [ val(meta), [ bam ] ]
      ^^^^^^^^^^
  ```
