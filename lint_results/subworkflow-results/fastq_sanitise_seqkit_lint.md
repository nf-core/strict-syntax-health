# Nextflow lint results

- Generated: 2026-06-15T00:46:19.977441+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/fastq_sanitise_seqkit/main.nf:53:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      reads    = ch_reads    // channel: [ val(meta), [ fastq ] ]
      ^^^^^^^^^^
  ```
