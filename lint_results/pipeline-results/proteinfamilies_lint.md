# Nextflow lint results

- Generated: 2026-03-05T00:23:42.481004337Z
- Nextflow version: 26.02.0-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `workflows/proteinfamilies.nf:200:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_config        = channel.fromPath(
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/proteinfamilies.nf:202:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_custom_config = params.multiqc_config ?
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/proteinfamilies.nf:205:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_logo          = params.multiqc_logo ?
      ^^^^^^^^^^^^^^^
  ```
