# Nextflow lint results

- Generated: 2026-05-29T00:45:51.874850+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/fastq_sanitise_seqkit/main.nf:53:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      reads    = ch_reads    // channel: [ val(meta), [ fastq ] ]
      ^^^^^^^^^^
  ```
