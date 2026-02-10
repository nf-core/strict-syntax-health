# Nextflow lint results

- Generated: 2026-02-10T00:27:01.522807+00:00
- Nextflow version: 26.01.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/rundbcan/database/main.nf:17:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/rundbcan/database/main.nf:30:9`: Variable was declared but not used

  ```nextflow
      def args        = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
