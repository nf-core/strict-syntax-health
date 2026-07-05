# Nextflow lint results

- Generated: 2026-07-05T00:34:54.677594+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_subsampledepth_samtools/main.nf:93:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      bam_subsampled    = ch_bam_subsampled             // channel: [ val(meta), path(bam), path(csi) ]
      ^^^^^^^^^^
  ```
