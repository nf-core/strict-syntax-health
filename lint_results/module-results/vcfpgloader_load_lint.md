# Nextflow lint results

- Generated: 2026-02-10T00:27:01.543848+00:00
- Nextflow version: 26.01.0-edge
- Summary: 1 error

## :x: Errors

- Error: `modules/nf-core/vcfpgloader/load/main.nf:28:26`: `ROWS_LOADED` is not defined

  ```nextflow
      tuple val(meta), env(ROWS_LOADED), emit: row_count
                           ^^^^^^^^^^
  ```
