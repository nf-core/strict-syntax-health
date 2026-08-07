# Nextflow lint results

- Generated: 2026-08-07T01:18:22.034050+00:00
- Nextflow version: 26.07.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/civicpy/annotate/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args   ?: ''
          ^^^^^^^^^^
  ```
