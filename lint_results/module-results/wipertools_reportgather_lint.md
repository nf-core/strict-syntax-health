# Nextflow lint results

- Generated: 2026-02-07T00:24:15.278980+00:00
- Nextflow version: 25.12.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/wipertools/reportgather/main.nf:25:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      if (report.any { it.name == "${prefix}.report" }) {
                       ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/wipertools/reportgather/main.nf:46:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      if (report.any { it.name == "${prefix}.report" }) {
                       ^^^^^^^^^^
  ```
