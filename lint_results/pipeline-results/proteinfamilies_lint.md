# Nextflow lint results

- Generated: 2026-03-13T00:22:03.749777824Z
- Nextflow version: 26.02.0-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `workflows/proteinfamilies.nf:202:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_config        = channel.fromPath(
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/proteinfamilies.nf:204:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_custom_config = params.multiqc_config ?
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/proteinfamilies.nf:207:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_logo          = params.multiqc_logo ?
      ^^^^^^^^^^^^^^^
  ```
