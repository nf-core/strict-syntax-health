# Nextflow lint results

- Generated: 2026-10-31T00:21:15.282082+00:00
- Nextflow version: 26.10.4
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/parabricks/deepsomatic/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```

- Warning: `modules/nf-core/parabricks/deepsomatic/main.nf:50:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
