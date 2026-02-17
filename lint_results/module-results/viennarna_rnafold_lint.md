# Nextflow lint results

- Generated: 2026-02-17T00:24:27.816741+00:00
- Nextflow version: 26.01.1-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/viennarna/rnafold/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = meta.id ?: "${fasta.getName()}"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/viennarna/rnafold/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
