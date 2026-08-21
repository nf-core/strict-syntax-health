# Nextflow lint results

- Generated: 2026-08-21T00:12:32.159208960Z
- Nextflow version: 26.08.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/local/shiny_app/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def prefix                    = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/treesummary/main.nf:39:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```
