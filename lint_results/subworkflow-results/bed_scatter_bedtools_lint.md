# Nextflow lint results

- Generated: 2026-07-16T00:33:22.645452+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bed_scatter_bedtools/main.nf:19:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      scattered_beds = ch_scattered_beds // channel: [ val(meta), path(bed), val(scatter_count) ]
      ^^^^^^^^^^
  ```
