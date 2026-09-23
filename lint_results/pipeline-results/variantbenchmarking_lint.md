# Nextflow lint results

- Generated: 2026-09-23T00:27:18.693355470Z
- Nextflow version: 26.08.0-edge
- Summary: 5 warnings

## :warning: Warnings

- Warning: `subworkflows/local/intersect_statistics/main.nf:18:13`: Variable was declared but not used

  ```nextflow
          def meta         = input[0]
              ^^^^
  ```

- Warning: `subworkflows/local/report_benchmark_statistics/main.nf:73:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def clean_meta = meta.findAll { it.key != 'csv' }
                                              ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_variantbenchmarking_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:231:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def _meta = it[0]
                      ^^
  ```

- Warning: `workflows/variantbenchmarking.nf:232:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def regions_file = it[2]
                             ^^
  ```
