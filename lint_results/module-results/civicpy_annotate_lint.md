# Nextflow lint results

- Generated: 2026-06-19T00:54:55.522348+00:00
- Nextflow version: 26.04.4
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/civicpy/annotate/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args   ?: ''
          ^^^^^^^^^^
  ```
