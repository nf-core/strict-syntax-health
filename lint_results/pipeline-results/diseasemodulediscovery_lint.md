# Nextflow lint results

- Generated: 2026-11-27T00:12:28.194004799Z
- Nextflow version: 26.11.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/gprofiler2/gost/main.nf:29:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```
