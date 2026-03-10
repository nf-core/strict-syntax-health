# Nextflow lint results

- Generated: 2026-03-10T00:22:28.182361145Z
- Nextflow version: 26.02.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_variantprioritization_pipeline/main.nf:187:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def duplicates = germlineIds.countBy { it }.findAll { _k, v -> v > 1 }.keySet()
                                             ^^
  ```
