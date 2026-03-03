# Nextflow lint results

- Generated: 2026-03-03T00:23:10.511409157Z
- Nextflow version: 26.02.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/local/boltz_fasta/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/run_helixfold3/main.nf:107:9`: Variable was declared but not used

  ```nextflow
      def VERSION = '705c2974a833cdc3a4420f4e3379da596091c97f'
          ^^^^^^^
  ```
