# Nextflow lint results

- Generated: 2026-06-24T00:40:31.565689+00:00
- Nextflow version: 26.05.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/opt_flip_track_stat/main.nf:28:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      summary  = ch_summary  // channel: [ val(meta), ["collapsed_summary.tsv"]]
      ^^^^^^^^^^
  ```
