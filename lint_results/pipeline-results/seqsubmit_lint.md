# Nextflow lint results

- Generated: 2026-05-15T00:37:08.694803619Z
- Nextflow version: 26.04.1
- Summary: 12 warnings

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

- Warning: `subworkflows/local/fasta_validation.nf:27:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      fasta_split = input_fasta.branch { meta, fasta ->
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

- Warning: `workflows/assemblysubmit.nf:229:80`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(CONCAT_ACCESSIONS.out.file_out.map{meta, file -> file})
                                                                                 ^^^^
  ```

- Warning: `workflows/assemblysubmit.nf:230:78`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(CONCAT_METADATA.out.file_out.map{meta, file -> file})
                                                                               ^^^^
  ```

- Warning: `workflows/genomesubmit.nf:361:78`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(CONCAT_METADATA.out.file_out.map{meta, file -> file})
                                                                               ^^^^
  ```

- Warning: `workflows/genomesubmit.nf:363:80`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(CONCAT_ACCESSIONS.out.file_out.map{meta, file -> file})
                                                                                 ^^^^
  ```
