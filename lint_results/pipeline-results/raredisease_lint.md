# Nextflow lint results

- Generated: 2026-03-17T00:27:33.941453232Z
- Nextflow version: 26.02.0-edge
- Summary: 1 error

## :x: Errors

- Error: `tests/nextflow.config:28:27`: `SENTIEON_AUTH_MECH` is not defined (hint: use `env('...')` to access environment variable)

  ```nextflow
      SENTIEON_AUTH_MECH = "$SENTIEON_AUTH_MECH"
                            ^^^^^^^^^^^^^^^^^^^
  ```
