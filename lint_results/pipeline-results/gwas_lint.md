# Nextflow lint results

- Generated: 2026-03-17T00:23:40.307802209Z
- Nextflow version: 26.02.0-edge
- Summary: 7 warnings

## :warning: Warnings

- Warning: `modules/nf-core/plink/gwas/main.nf:33:9`: Variable was declared but not used

  ```nextflow
      def outmeta = ""
          ^^^^^^^
  ```

- Warning: `modules/nf-core/plink/gwas/main.nf:64:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/plink/gwas/main.nf:69:9`: Variable was declared but not used

  ```nextflow
      def outmeta = ""
          ^^^^^^^
  ```

- Warning: `modules/nf-core/plink/vcf/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_gwas_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_gwas_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `workflows/gwas.nf:67:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
