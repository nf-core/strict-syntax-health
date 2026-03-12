# Nextflow lint results

- Generated: 2026-03-12T00:18:13.012691246Z
- Nextflow version: 26.02.0-edge
- Summary: 9 errors, 2 warnings

## :x: Errors

- Error: `conf/modules_alphafold2.config:96:9`: If statements cannot be mixed with config statements

  ```nextflow
          if (params.use_gpu) {
          ^
  ```

- Error: `conf/modules_alphafold2.config:158:9`: If statements cannot be mixed with config statements

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
