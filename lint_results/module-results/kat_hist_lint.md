# Nextflow lint results

- Generated: 2026-01-23T00:22:21.975403+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/kat/hist/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def args      = task.ext.args   ?: ''
          ^^^^^^^^^^
  ```
