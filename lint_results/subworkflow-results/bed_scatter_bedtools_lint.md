# Nextflow lint results

- Generated: 2026-05-27T00:44:41.090401+00:00
- Nextflow version: 26.04.2
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bed_scatter_bedtools/main.nf:19:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      scattered_beds = ch_scattered_beds // channel: [ val(meta), path(bed), val(scatter_count) ]
      ^^^^^^^^^^
  ```
