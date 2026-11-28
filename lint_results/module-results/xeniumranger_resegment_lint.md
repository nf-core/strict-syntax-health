# Nextflow lint results

- Generated: 2026-11-28T00:16:01.010674+00:00
- Nextflow version: 26.11.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/xeniumranger/resegment/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
