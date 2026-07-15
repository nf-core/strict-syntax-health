# Nextflow lint results

- Generated: 2026-07-15T00:27:50.433158+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/fastq_find_mirna_mirdeep2/main.nf:24:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      outputs  = MIRDEEP2_MIRDEEP2.out.outputs // channel: [ val(meta), [ bed, csv, html ] ]
      ^^^^^^^^^^
  ```
