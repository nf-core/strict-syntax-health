# Nextflow lint results

- Generated: 2026-11-07T00:15:17.073528+00:00
- Nextflow version: 26.10.5
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/humann3/renorm/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
