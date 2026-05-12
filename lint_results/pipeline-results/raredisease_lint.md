# Nextflow lint results

- Generated: 2026-05-12T00:35:30.258977748Z
- Nextflow version: 26.04.1
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/local/call_sv_MT/main.nf:141:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .filter{ !it.isEmpty() }
                            ^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```
