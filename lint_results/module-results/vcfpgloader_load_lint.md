# Nextflow lint results

- Generated: 2026-02-07T00:24:15.275723+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 error

## :x: Errors

- Error: `modules/nf-core/vcfpgloader/load/main.nf:28:26`: `ROWS_LOADED` is not defined

  ```nextflow
      tuple val(meta), env(ROWS_LOADED), emit: row_count
                           ^^^^^^^^^^
  ```
