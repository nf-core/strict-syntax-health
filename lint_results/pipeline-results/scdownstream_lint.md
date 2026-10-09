# Nextflow lint results

- Generated: 2026-10-09T00:30:51.331754489Z
- Nextflow version: 26.09.2-edge
- Summary: 4 warnings

## :warning: Warnings

- Warning: `modules/local/cell2cell/tensor/main.nf:30:5`: Variable was declared but not used

  ```nextflow
      integration = meta.integration ?: 'integration'
      ^^^^^^^^^^^
  ```

- Warning: `modules/local/liana/rankaggregate/main.nf:28:5`: Variable was declared but not used

  ```nextflow
      obs_key = meta.obs_key ?: "leiden"
      ^^^^^^^
  ```

- Warning: `modules/local/scanpy/paga/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      obs_key = meta.obs_key ?: "leiden"
      ^^^^^^^
  ```

- Warning: `modules/local/scarches/expimap/main.nf:26:5`: Variable was declared but not used

  ```nextflow
      args   = task.ext.args ?: ''
      ^^^^
  ```
