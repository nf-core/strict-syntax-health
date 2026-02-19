# Nextflow lint results

- Generated: 2026-02-19T00:24:59.439541+00:00
- Nextflow version: 26.01.1-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/sratools/prefetch/main.nf:22:5`: The `shell` block is deprecated, use `script` instead

  ```nextflow
      shell:
      ^^^^^^
  ```

- Warning: `modules/nf-core/sratools/prefetch/main.nf:24:5`: Variable was declared but not used

  ```nextflow
      args2 = task.ext.args2 ?: '5 1 100'  // <num retries> <base delay in seconds> <max delay in seconds>
      ^^^^^^^^^^
  ```
