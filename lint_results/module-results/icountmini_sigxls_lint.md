# Nextflow lint results

- Generated: 2026-10-16T00:24:13.384829+00:00
- Nextflow version: 26.10.1
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/icountmini/sigxls/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
