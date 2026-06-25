# Nextflow lint results

- Generated: 2026-06-25T00:44:56.995053+00:00
- Nextflow version: 26.05.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/mafft_align/main.nf:13:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      alignment = MAFFT_ALIGN_MODULE.out.fas      // channel: [ val(meta), *.fas ]
      ^^^^^^^^^^
  ```
