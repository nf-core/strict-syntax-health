# Nextflow lint results

- Generated: 2026-11-21T00:15:01.855316+00:00
- Nextflow version: 26.11.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/parabricks/deepsomatic/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```

- Warning: `modules/nf-core/parabricks/deepsomatic/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
