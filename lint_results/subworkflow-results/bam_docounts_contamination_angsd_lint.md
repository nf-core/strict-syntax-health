# Nextflow lint results

- Generated: 2026-06-26T00:47:26.809164+00:00
- Nextflow version: 26.05.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_docounts_contamination_angsd/main.nf:23:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      txt      = ANGSD_CONTAMINATION.out.txt // channel: [ val(meta), [ txt ] ]
      ^^^^^^^^^^
  ```
