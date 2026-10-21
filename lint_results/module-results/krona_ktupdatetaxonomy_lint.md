# Nextflow lint results

- Generated: 2026-10-21T00:24:17.497644+00:00
- Nextflow version: 26.10.2
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/krona/ktupdatetaxonomy/main.nf:13:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
