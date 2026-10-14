# Nextflow lint results

- Generated: 2026-10-14T00:24:29.326436+00:00
- Nextflow version: 26.10.0
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gprofiler2/gost/main.nf:26:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
