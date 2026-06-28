# Nextflow lint results

- Generated: 2026-06-28T00:43:03.833229+00:00
- Nextflow version: 26.05.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/fasta_index_dna/main.nf:55:9`: Emit name should be omitted when there is only one emit

  ```nextflow
          index    = ch_aligner_index // channel: [ val(meta), path(index) ]
          ^^^^^^^^^^
  ```
