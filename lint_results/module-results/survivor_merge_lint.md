# Nextflow lint results

- Generated: 2026-01-30T00:23:50.054651+00:00
- Nextflow version: 25.12.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/survivor/merge/main.nf:30:13`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          if (it.getExtension() == "gz"){
              ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/survivor/merge/main.nf:57:13`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          if (it.getExtension() == "gz"){
              ^^^^^^^^^^
  ```
