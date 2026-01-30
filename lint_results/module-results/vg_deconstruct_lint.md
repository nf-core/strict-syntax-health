# Nextflow lint results

- Generated: 2026-01-30T00:23:50.062595+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 error

## :x: Errors

- Error: `modules/nf-core/vg/deconstruct/main.nf:26:37`: `gwbt` is not defined

  ```nextflow
      def gbwt_arg = gbwt ? "--gbwt ${gwbt}" : ""
                                      ^^^^^^^^^^
  ```
