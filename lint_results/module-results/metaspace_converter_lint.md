# Nextflow lint results

- Generated: 2026-03-17T00:30:02.410946+00:00
- Nextflow version: 26.02.0-edge
- Summary: 5 warnings

## :warning: Warnings

- Warning: `modules/nf-core/metaspace/converter/main.nf:26:5`: Variable was declared but not used

  ```nextflow
      database_name    = database_name_ ?: 'HMDB'
      ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/metaspace/converter/main.nf:27:5`: Variable was declared but not used

  ```nextflow
      database_version = database_version_ ?: 'v4'
      ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/metaspace/converter/main.nf:28:5`: Variable was declared but not used

  ```nextflow
      fdr              = fdr_ ?: '0.1'
      ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/metaspace/converter/main.nf:29:5`: Variable was declared but not used

  ```nextflow
      use_tic          = use_tic_ ?: 'true'
      ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/metaspace/converter/main.nf:30:5`: Variable was declared but not used

  ```nextflow
      metadata_as_obs  = metadata_as_obs_ ?: 'false'
      ^^^^^^^^^^
  ```
