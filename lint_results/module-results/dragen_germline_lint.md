# Nextflow lint results

- Generated: 2026-02-01T00:22:15.899574+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 error

## :x: Errors

- Error: `modules/nf-core/dragen/germline/main.nf:282:22`: Unexpected input: 'i'

  ```nextflow
              for (int i = 1; i < qc_coverage_region.size() + 1; i++) {
                       ^^^^^^^^^^
  ```
