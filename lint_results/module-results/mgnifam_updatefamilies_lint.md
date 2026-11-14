# Nextflow lint results

- Generated: 2026-11-14T00:15:47.983237+00:00
- Nextflow version: 26.10.6
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/mgnifam/updatefamilies/main.nf:32:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
