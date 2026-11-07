# Nextflow lint results

- Generated: 2026-11-07T00:15:17.114213+00:00
- Nextflow version: 26.10.5
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/mmseqs/createindex/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
