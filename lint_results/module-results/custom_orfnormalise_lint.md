# Nextflow lint results

- Generated: 2026-09-27T00:24:18.674002+00:00
- Nextflow version: 26.09.1-edge
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
