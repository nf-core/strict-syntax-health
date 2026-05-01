# Nextflow lint results

- Generated: 2026-05-01T00:35:03.157111886Z
- Nextflow version: 26.04.0
- Summary: 6 warnings

## :warning: Warnings

- Warning: `modules/nf-core/ganon/buildcustom/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/ganon/buildcustom/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def taxonomy_args = taxonomy_files ? "--taxonomy-files ${taxonomy_files}" : ""
          ^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/ganon/buildcustom/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def genome_size_args = genome_size_files ? "--genome-size-files ${genome_size_files}" : ""
          ^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/malt/build/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/pigz/compress/main.nf:35:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/unzip/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```
