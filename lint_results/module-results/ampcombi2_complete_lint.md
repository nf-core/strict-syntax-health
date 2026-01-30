# Nextflow lint results

- Generated: 2026-01-30T00:23:49.942195+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/ampcombi2/complete/main.nf:25:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          --summaries_files '${summaries.collect{"$it"}.join("' '")}' \\
                                                  ^^^^^^^^^^
  ```
