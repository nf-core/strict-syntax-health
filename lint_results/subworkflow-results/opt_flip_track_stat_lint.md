# Nextflow lint results

- Generated: 2026-06-15T00:46:19.978287+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/opt_flip_track_stat/main.nf:28:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      summary  = ch_summary  // channel: [ val(meta), ["collapsed_summary.tsv"]]
      ^^^^^^^^^^
  ```
