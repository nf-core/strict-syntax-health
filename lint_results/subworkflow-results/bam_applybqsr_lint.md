# Nextflow lint results

- Generated: 2026-07-13T00:30:27.591103+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_applybqsr/main.nf:47:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      recal_out = recal_out // channel: [ meta, file, index ]
      ^^^^^^^^^^
  ```
