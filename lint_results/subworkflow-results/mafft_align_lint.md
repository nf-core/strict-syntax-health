# Nextflow lint results

- Generated: 2026-07-08T00:31:27.755934+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/mafft_align/main.nf:13:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      alignment = MAFFT_ALIGN_MODULE.out.fas      // channel: [ val(meta), *.fas ]
      ^^^^^^^^^^
  ```
