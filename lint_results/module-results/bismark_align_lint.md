# Nextflow lint results

- Generated: 2026-02-01T00:22:15.872414+00:00
- Nextflow version: 25.12.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/bismark/align/main.nf:51:18`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          } catch (all) {
                   ^^^^^^
  ```

- Warning: `modules/nf-core/bismark/align/main.nf:67:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
