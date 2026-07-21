# Nextflow lint results

- Generated: 2026-07-21T00:30:56.339686648Z
- Nextflow version: 26.07.0-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `modules/local/boltz_fasta/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/run_helixfold3/main.nf:114:9`: Variable was declared but not used

  ```nextflow
      def VERSION = '705c2974a833cdc3a4420f4e3379da596091c97f'
          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_proteinfold_pipeline/main.nf:327:78`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def unsupportedModes = requestedModes.findAll { !supportedModes.contains(it) }.unique().sort()
                                                                               ^^
  ```
