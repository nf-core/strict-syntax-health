# Nextflow lint results

- Generated: 2026-02-10T00:27:01.520614+00:00
- Nextflow version: 26.01.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/ribocode/metaplots/main.nf:34:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
