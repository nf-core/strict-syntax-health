# Nextflow lint results

- Generated: 2026-02-11T00:30:24.104084+00:00
- Nextflow version: 26.01.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/chewbbaca/createschema/main.nf:51:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/chewbbaca/createschema/main.nf:53:9`: Variable was declared but not used

  ```nextflow
      def schema = "--n ${prefix}"
          ^^^^^^^^^^
  ```
