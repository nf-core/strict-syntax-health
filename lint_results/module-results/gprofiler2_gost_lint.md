# Nextflow lint results

- Generated: 2026-11-12T00:20:38.248403+00:00
- Nextflow version: 26.10.5
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gprofiler2/gost/main.nf:29:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
