# Nextflow lint results

- Generated: 2026-05-19T00:41:02.144112692Z
- Nextflow version: 26.04.1
- Summary: 4 warnings

## :warning: Warnings

- Warning: `subworkflows/local/call_sv_MT/main.nf:153:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .filter { !it.isEmpty() }
                             ^^
  ```

- Warning: `workflows/raredisease.nf:940:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_config        = channel.fromPath(
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/raredisease.nf:942:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_custom_config = val_multiqc_config ?
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/raredisease.nf:945:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_logo          = val_multiqc_logo ?
      ^^^^^^^^^^^^^^^
  ```
