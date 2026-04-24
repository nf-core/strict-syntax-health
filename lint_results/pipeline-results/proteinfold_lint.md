# Nextflow lint results

- Generated: 2026-04-24T00:32:06.272879480Z
- Nextflow version: 26.03.3-edge
- Summary: 9 errors, 4 warnings

## :x: Errors

- Error: `conf/modules_alphafold2.config:94:9`: If statements cannot be mixed with config statements

  ```nextflow
          if (params.use_gpu) {
          ^
  ```

- Error: `conf/modules_alphafold2.config:154:9`: If statements cannot be mixed with config statements

  ```nextflow
          if (params.use_gpu) {
          ^
  ```

- Error: `conf/modules_alphafold3.config:95:9`: If statements cannot be mixed with config statements

  ```nextflow
          if (params.use_gpu) {
          ^
  ```

- Error: `conf/modules_boltz.config:67:9`: If statements cannot be mixed with config statements

  ```nextflow
          if (params.use_gpu) {
          ^
  ```

- Error: `conf/modules_colabfold.config:40:9`: If statements cannot be mixed with config statements

  ```nextflow
          if (params.use_gpu) {
          ^
  ```

- Error: `conf/modules_esmfold.config:22:9`: If statements cannot be mixed with config statements

  ```nextflow
          if (params.use_gpu) {
          ^
  ```

- Error: `conf/modules_helixfold3.config:100:9`: If statements cannot be mixed with config statements

  ```nextflow
          if (params.use_gpu) {
          ^
  ```

- Error: `conf/modules_rosettafold2na.config:44:9`: If statements cannot be mixed with config statements

  ```nextflow
          if (params.use_gpu) {
          ^
  ```

- Error: `conf/modules_rosettafold_all_atom.config:23:9`: If statements cannot be mixed with config statements

  ```nextflow
          if (params.use_gpu) {
          ^
  ```

## :warning: Warnings

- Warning: `modules/local/boltz_fasta/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/run_helixfold3/main.nf:109:9`: Variable was declared but not used

  ```nextflow
      def VERSION = '705c2974a833cdc3a4420f4e3379da596091c97f'
          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_proteinfold_pipeline/main.nf:324:78`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def unsupportedModes = requestedModes.findAll { !supportedModes.contains(it) }.unique().sort()
                                                                               ^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```
