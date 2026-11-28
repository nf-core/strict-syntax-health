# Nextflow lint results

- Generated: 2026-11-28T00:16:00.868230+00:00
- Nextflow version: 26.11.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/pairtools/parse/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
