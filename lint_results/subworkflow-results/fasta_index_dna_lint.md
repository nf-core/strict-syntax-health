# Nextflow lint results

- Generated: 2026-06-05T00:46:34.526895+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/fasta_index_dna/main.nf:55:9`: Emit name should be omitted when there is only one emit

  ```nextflow
          index    = ch_aligner_index // channel: [ val(meta), path(index) ]
          ^^^^^^^^^^
  ```
