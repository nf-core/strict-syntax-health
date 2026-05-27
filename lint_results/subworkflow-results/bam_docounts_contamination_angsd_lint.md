# Nextflow lint results

- Generated: 2026-05-27T00:44:41.087177+00:00
- Nextflow version: 26.04.2
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_docounts_contamination_angsd/main.nf:23:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      txt      = ANGSD_CONTAMINATION.out.txt // channel: [ val(meta), [ txt ] ]
      ^^^^^^^^^^
  ```
