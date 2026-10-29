# Nextflow lint results

- Generated: 2026-10-29T00:21:43.224893+00:00
- Nextflow version: 26.10.4
- Summary: 3 warnings

## :warning: Warnings

- Warning: `modules/nf-core/dds/createproject/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```

- Warning: `modules/nf-core/dds/createproject/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/dds/createproject/main.nf:31:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
