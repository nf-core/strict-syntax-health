# Nextflow lint results

- Generated: 2026-02-03T00:25:25.810665+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/custom/dumpsoftwareversions/main.nf:31:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
