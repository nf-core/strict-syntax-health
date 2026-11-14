# Nextflow lint results

- Generated: 2026-11-14T00:15:48.084741+00:00
- Nextflow version: 26.10.6
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/savana/run/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
