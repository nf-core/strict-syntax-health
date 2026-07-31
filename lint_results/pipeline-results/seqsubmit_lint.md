# Nextflow lint results

- Generated: 2026-07-31T00:34:44.727507854Z
- Nextflow version: 26.07.0-edge
- Summary: 10 warnings

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

- Warning: `modules/local/generate_assembly_manifest/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/generate_assembly_manifest/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `subworkflows/local/fasta_validation/main.nf:27:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      fasta_split = input_fasta.branch { meta, fasta ->
                                         ^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_classify_catpack/main.nf:39:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, db ->
                    ^^^^
  ```

- Warning: `workflows/assemblysubmit.nf:53:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, fasta, reads_1, reads_2 ->
                              ^^^^^^^
  ```

- Warning: `workflows/assemblysubmit.nf:61:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, fasta, reads_1, reads_2 ->
                       ^^^^^
  ```
