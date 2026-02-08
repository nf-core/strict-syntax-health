# Nextflow lint results

- Generated: 2026-02-08T00:29:10.275063+00:00
- Nextflow version: 25.12.0-edge
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
