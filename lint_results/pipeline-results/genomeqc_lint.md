# Nextflow lint results

- Generated: 2026-07-11T00:27:37.006125030Z
- Nextflow version: 26.06.0-edge
- Summary: 24 warnings

## :warning: Warnings

- Warning: `main.nf:49:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = GENOMEQC.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/buscos_seqs/main.nf:19:9`: Variable was declared but not used

  ```nextflow
      def prefix         = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/genomeannotationbuscoideogram/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def prefix = "${genusspeci}_${lineage}"
          ^^^^^^
  ```

- Warning: `modules/local/repeatmasker_download_db/main.nf:20:9`: Variable was declared but not used

  ```nextflow
      def out_gunzip   = filename.replaceAll(/\.gz$/, '')
          ^^^^^^^^^^
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

- Warning: `modules/local/te_tbl_2_table/main.nf:18:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/treesummary/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/cat/cat/main.nf:23:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def file_list = files_in.collect { it.toString() }
                                         ^^
  ```

- Warning: `modules/nf-core/cat/cat/main.nf:59:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def file_list   = files_in.collect { it.toString() }
                                           ^^
  ```

- Warning: `subworkflows/local/decontamination.nf:39:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gxdb_manifest ?: Channel.empty() // If there no manifest, use empty channel (won't run)
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/fasta_annotate_te/main.nf:48:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      | map { meta, h5 -> h5 }
                              ^^^^
  ```

- Warning: `subworkflows/local/fasta_annotate_te/main.nf:110:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_shared_lib = CDHIT_CDHITEST.out.fasta | map { meta, fasta -> fasta }
                                                                   ^^^^
  ```

- Warning: `subworkflows/local/fasta_annotate_te/main.nf:113:81`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_shared_lib = MMSEQS_EASYLINCLUST.out.representatives | map { meta, fasta -> fasta }
                                                                                  ^^^^
  ```

- Warning: `subworkflows/local/fasta_annotate_te/main.nf:116:80`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_shared_lib = MMSEQS_EASYCLUSTER.out.representatives | map { meta, fasta -> fasta }
                                                                                 ^^^^
  ```

- Warning: `subworkflows/local/fasta_annotate_te/main.nf:121:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                               | map { meta, fasta -> meta }
                                             ^^^^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:26:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fasta.view { "Running ${it[0]} on genome and annotation mode"}
                                 ^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:259:114`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      buscos_per_seqs            = !params.skip_busco ? GENOMEANNOTATIONBUSCOIDEOGRAM.out.busco_mappings.collect { meta, table -> table}.map { tables -> tables.toSorted { a, b -> a.name <=> b.name } } : channel.empty() // channel: [ val(meta), [csv] ]
                                                                                                                   ^^^^
  ```

- Warning: `subworkflows/local/genome_only.nf:17:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fasta.view { "Running ${it[0]} on genome only mode"}
                                 ^^
  ```

- Warning: `subworkflows/local/genome_only.nf:19:5`: Variable was declared but not used

  ```nextflow
      ch_versions   = channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/genome_only.nf:129:101`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      buscos_per_seqs         = !params.skip_busco ? GENOMEBUSCOIDEOGRAM.out.busco_mappings.collect { meta, table -> table}.map { tables -> tables.toSorted { a, b -> a.name <=> b.name } } : channel.empty() // channel: [ csv ]
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

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```
