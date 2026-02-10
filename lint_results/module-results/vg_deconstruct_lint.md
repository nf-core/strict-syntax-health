# Nextflow lint results

- Generated: 2026-02-10T00:27:01.544737+00:00
- Nextflow version: 26.01.0-edge
- Summary: 1 error

## :x: Errors

- Error: `modules/nf-core/vg/deconstruct/main.nf:26:37`: `gwbt` is not defined

  ```nextflow
      def gbwt_arg = gbwt ? "--gbwt ${gwbt}" : ""
                                      ^^^^^^^^^^
  ```
