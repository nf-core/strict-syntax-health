# Nextflow lint results

- Generated: 2026-10-14T00:24:29.306574+00:00
- Nextflow version: 26.10.0
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gatk/realignertargetcreator/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
