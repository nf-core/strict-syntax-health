# Nextflow lint results

- Generated: 2026-02-10T00:27:01.520944+00:00
- Nextflow version: 26.01.0-edge
- Summary: 1 error, 1 warning

## :x: Errors

- Error: `modules/nf-core/ribotish/predict/main.nf:41:12`: `para_tis` is not defined

  ```nextflow
          if (para_tis){
             ^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/nf-core/ribotish/predict/main.nf:64:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
