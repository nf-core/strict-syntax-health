# Nextflow lint results

- Generated: 2026-10-30T00:22:40.994236+00:00
- Nextflow version: 26.10.4
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gatk4/printsvevidence/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
