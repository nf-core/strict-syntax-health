# Nextflow lint results

- Generated: 2026-02-03T00:25:25.943480+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 error, 1 warning

## :x: Errors

- Error: `modules/nf-core/svanalyzer/svbenchmark/main.nf:36:9`: `bed` is already declared

  ```nextflow
      def bed = bed ? "-includebed $bed" : ""
          ^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/nf-core/svanalyzer/svbenchmark/main.nf:63:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
