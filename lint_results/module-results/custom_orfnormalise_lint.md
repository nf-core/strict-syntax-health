# Nextflow lint results

- Generated: 2026-06-16T14:40:24.636570+00:00
- Nextflow version: 26.04.3
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/custom/orfnormalise/main.nf:24:5`: Variable was declared but not used

  ```nextflow
      sample_id = meta.id ?: 'unknown'
      ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/custom/orfnormalise/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      args      = task.ext.args ?: ''
      ^^^^^^^^^^
  ```
