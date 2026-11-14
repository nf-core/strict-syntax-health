# Nextflow lint results

- Generated: 2026-11-14T00:15:47.829949+00:00
- Nextflow version: 26.10.6
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/cellrangeratac/count/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
