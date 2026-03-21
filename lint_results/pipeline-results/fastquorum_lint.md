# Nextflow lint results

- Generated: 2026-03-21T00:21:50.294680177Z
- Nextflow version: 26.03.0-edge
- Summary: 5 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_fastquorum_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_fastquorum_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_fastquorum_pipeline/main.nf:111:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              validateInputSamplesheetRow(it)
                                          ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_fastquorum_pipeline/main.nf:116:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              validateInputSamplesheet(it)
                                       ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_fastquorum_pipeline/main.nf:122:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  return [meta, it]
                                ^^
  ```
