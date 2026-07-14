# Nextflow lint results

- Generated: 2026-07-14T00:29:23.995301+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_docounts_contamination_angsd/main.nf:23:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      txt      = ANGSD_CONTAMINATION.out.txt // channel: [ val(meta), [ txt ] ]
      ^^^^^^^^^^
  ```
