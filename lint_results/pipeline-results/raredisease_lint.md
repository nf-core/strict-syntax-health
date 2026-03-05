# Nextflow lint results

- Generated: 2026-03-05T00:24:33.361122218Z
- Nextflow version: 26.02.0-edge
- Summary: 1 error

## :x: Errors

- Error: `tests/nextflow.config:28:27`: `SENTIEON_AUTH_MECH` is not defined (hint: use `env('...')` to access environment variable)

  ```nextflow
      SENTIEON_AUTH_MECH = "$SENTIEON_AUTH_MECH"
                            ^^^^^^^^^^^^^^^^^^^
  ```
