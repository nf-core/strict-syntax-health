# Nextflow lint results

- Generated: 2026-03-14T00:21:53.136095777Z
- Nextflow version: 26.02.0-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `workflows/proteinfamilies.nf:215:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_config        = channel.fromPath(
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/proteinfamilies.nf:217:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_custom_config = params.multiqc_config ?
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/proteinfamilies.nf:220:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_logo          = params.multiqc_logo ?
      ^^^^^^^^^^^^^^^
  ```
