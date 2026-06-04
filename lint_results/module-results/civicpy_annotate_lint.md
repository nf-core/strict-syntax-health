# Nextflow lint results

- Generated: 2026-06-04T00:53:04.670938+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/civicpy/annotate/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args   ?: ''
          ^^^^^^^^^^
  ```
