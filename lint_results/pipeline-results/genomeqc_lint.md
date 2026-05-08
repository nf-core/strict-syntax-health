# Nextflow lint results

- Generated: 2026-05-08T00:32:56.569485755Z
- Nextflow version: 26.04.0
- Summary: 10 warnings

## :warning: Warnings

- Warning: `modules/local/buscos_seqs/main.nf:17:9`: Variable was declared but not used

  ```nextflow
      def prefix         = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/shiny_app/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix           = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/shiny_app/main.nf:26:9`: Variable was declared but not used

  ```nextflow
      def results_path     = file(params.outdir).toAbsolutePath()
          ^^^^^^^^^^^^
  ```

- Warning: `modules/local/tree_summary.nf:35:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `subworkflows/local/decontamination.nf:40:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gxdb_manifest ?: Channel.empty() // If there no manifest, use empty channel (won't run)
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:24:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fasta.view { "Running ${it[0]} on genome and annotation mode"}
                                 ^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:26:5`: Variable was declared but not used

  ```nextflow
      ch_versions  = channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/genome_only.nf:15:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fasta.view { "Running ${it[0]} on genome only mode"}
                                 ^^
  ```

- Warning: `subworkflows/local/genome_only.nf:17:5`: Variable was declared but not used

  ```nextflow
      ch_versions   = channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `workflows/genomeqc.nf:221:5`: Variable was declared but not used

  ```nextflow
      ch_merqury_outputs                      = ch_merqury_qv
      ^^^^^^^^^^^^^^^^^^
  ```
