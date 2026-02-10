# Nextflow lint results

- Generated: 2026-02-10T00:27:01.531627+00:00
- Nextflow version: 26.01.0-edge
- Summary: 1 error, 1 warning

## :x: Errors

- Error: `modules/nf-core/shinyngs/app/tests/nextflow.config:6:32`: Unexpected input: ':'

  ```nextflow
      withName: test_shinyngs_app:SHINYNGS_APP {
                                 ^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/nf-core/shinyngs/app/main.nf:56:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
