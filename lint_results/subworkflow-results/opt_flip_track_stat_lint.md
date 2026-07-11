# Nextflow lint results

- Generated: 2026-07-11T00:30:43.499009+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/opt_flip_track_stat/main.nf:28:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      summary  = ch_summary  // channel: [ val(meta), ["collapsed_summary.tsv"]]
      ^^^^^^^^^^
  ```
