# Nextflow lint results

- Generated: 2026-05-12T00:36:57.920376751Z
- Nextflow version: 26.04.1
- Summary: 14 warnings

## :warning: Warnings

- Warning: `conf/modules.config:59:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  saveAs: { filename -> "db" }
                            ^^^^^^^^
  ```

- Warning: `conf/modules.config:65:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  saveAs: { filename -> "tax" }
                            ^^^^^^^^
  ```

- Warning: `modules/local/generate_assembly_manifest/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/generate_assembly_manifest/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/generate_assembly_manifest/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/barrnap/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/genome_evaluation.nf:30:5`: Variable was declared but not used

  ```nextflow
      ch_versions = channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_classify_catpack/main.nf:39:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, db ->
                    ^^^^
  ```

- Warning: `workflows/assemblysubmit.nf:41:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      webin_cli_version    // val: WebinCLI tool version to download and use for submission
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/assemblysubmit.nf:235:80`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(CONCAT_ACCESSIONS.out.file_out.map{meta, file -> file})
                                                                                 ^^^^
  ```

- Warning: `workflows/assemblysubmit.nf:236:78`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(CONCAT_METADATA.out.file_out.map{meta, file -> file})
                                                                               ^^^^
  ```

- Warning: `workflows/genomesubmit.nf:53:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      webin_cli_version        // val: WebinCLI tool version to download and use for submission
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/genomesubmit.nf:369:78`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(CONCAT_METADATA.out.file_out.map{meta, file -> file})
                                                                               ^^^^
  ```

- Warning: `workflows/genomesubmit.nf:371:80`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(CONCAT_ACCESSIONS.out.file_out.map{meta, file -> file})
                                                                                 ^^^^
  ```
