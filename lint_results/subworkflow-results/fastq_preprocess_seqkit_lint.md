# Nextflow lint results

- Generated: 2026-05-26T00:41:33.187196+00:00
- Nextflow version: 26.04.2
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/fastq_preprocess_seqkit/main.nf:73:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      reads    = ch_reads     // channel: [ val(meta), [ fastq ] ]
      ^^^^^^^^^^
  ```
