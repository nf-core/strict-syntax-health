# Nextflow lint results

- Generated: 2026-07-08T00:30:24.973179311Z
- Nextflow version: 26.06.0-edge
- Summary: 18 warnings

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

- Warning: `main.nf:101:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = ch_multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/create_reads_manifest/main.nf:25:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def fastq_args   = fastq_list.collect { "--fastq ${it.name}" }.join(' \\\n        ')
                                                         ^^
  ```

- Warning: `modules/local/generate_assembly_manifest/main.nf:26:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/generate_assembly_manifest/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/generate_assembly_manifest/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `subworkflows/local/fasta_validation/main.nf:27:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      fasta_split = input_fasta.branch { meta, fasta ->
                                         ^^^^
  ```

- Warning: `subworkflows/local/fasta_validation/main.nf:66:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      valid_fastas    = valid_fastas
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/genome_evaluation/main.nf:30:5`: Variable was declared but not used

  ```nextflow
      ch_versions = channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_classify_catpack/main.nf:39:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, db ->
                    ^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      valid_config = valid_config
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:76:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
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

- Warning: `workflows/genomesubmit.nf:372:78`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(CONCAT_METADATA.out.file_out.map{meta, file -> file})
                                                                               ^^^^
  ```

- Warning: `workflows/genomesubmit.nf:374:80`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(CONCAT_ACCESSIONS.out.file_out.map{meta, file -> file})
                                                                                 ^^^^
  ```
