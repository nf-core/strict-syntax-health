# Nextflow lint results

- Generated: 2026-07-10T00:38:53.795552+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/opt_flip_track_stat/main.nf:28:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      summary  = ch_summary  // channel: [ val(meta), ["collapsed_summary.tsv"]]
      ^^^^^^^^^^
  ```
