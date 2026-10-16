# Nextflow lint results

- Generated: 2026-10-16T00:24:13.340896+00:00
- Nextflow version: 26.10.1
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gcta/makegrmpart/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
