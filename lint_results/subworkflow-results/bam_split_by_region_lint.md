# Nextflow lint results

- Generated: 2026-07-16T00:33:22.643456+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_split_by_region/main.nf:65:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      bam_bai     = ch_output                         // channel: [ val(meta), path(bam), path(bai) ]
      ^^^^^^^^^^
  ```
