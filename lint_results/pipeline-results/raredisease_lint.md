# Nextflow lint results

- Generated: 2026-05-08T00:34:05.477940682Z
- Nextflow version: 26.04.0
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/local/call_sv_MT/main.nf:140:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .filter{ !it.isEmpty() }
                            ^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```
