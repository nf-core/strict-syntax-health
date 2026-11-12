# Nextflow lint results

- Generated: 2026-11-12T00:20:38.493696+00:00
- Nextflow version: 26.10.5
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/starfusion/build/main.nf:30:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
