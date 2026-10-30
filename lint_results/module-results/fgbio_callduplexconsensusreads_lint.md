# Nextflow lint results

- Generated: 2026-10-30T00:22:40.965992+00:00
- Nextflow version: 26.10.4
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/fgbio/callduplexconsensusreads/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
