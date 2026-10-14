# Nextflow lint results

- Generated: 2026-10-14T00:24:29.397176+00:00
- Nextflow version: 26.10.0
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/opt/stat/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
