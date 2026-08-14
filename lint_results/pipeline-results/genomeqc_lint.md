# Nextflow lint results

- Generated: 2026-08-14T00:21:35.761291200Z
- Nextflow version: 26.07.0-edge
- Summary: 17 warnings

## :warning: Warnings

- Warning: `modules/local/buscos_seqs/main.nf:19:9`: Variable was declared but not used

  ```nextflow
      def prefix         = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/genomeannotationbuscoideogram/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def prefix = "${meta.id}_${meta.lineage}"
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

- Warning: `modules/local/shiny_app/main.nf:29:9`: Variable was declared but not used

  ```nextflow
      def results_path     = file(params.outdir).toAbsolutePath()
          ^^^^^^^^^^^^
  ```

- Warning: `modules/local/te_tbl_2_table/main.nf:19:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/treesummary/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `subworkflows/local/fasta_annotate_te/main.nf:51:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      | map { meta, h5 -> h5 }
                              ^^^^
  ```

- Warning: `subworkflows/local/fasta_annotate_te/main.nf:113:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_shared_lib = CDHIT_CDHITEST.out.fasta | map { meta, fasta -> fasta }
                                                                   ^^^^
  ```

- Warning: `subworkflows/local/fasta_annotate_te/main.nf:116:81`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_shared_lib = MMSEQS_EASYLINCLUST.out.representatives | map { meta, fasta -> fasta }
                                                                                  ^^^^
  ```

- Warning: `subworkflows/local/fasta_annotate_te/main.nf:119:80`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ch_shared_lib = MMSEQS_EASYCLUSTER.out.representatives | map { meta, fasta -> fasta }
                                                                                 ^^^^
  ```

- Warning: `subworkflows/local/fasta_annotate_te/main.nf:124:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                               | map { meta, fasta -> meta }
                                             ^^^^^
  ```

- Warning: `subworkflows/local/genome_and_annotation/main.nf:26:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fasta.view { "Running ${it[0]} on genome and annotation mode"}
                                 ^^
  ```

- Warning: `subworkflows/local/genome_and_annotation/main.nf:259:114`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      buscos_per_seqs            = !params.skip_busco ? GENOMEANNOTATIONBUSCOIDEOGRAM.out.busco_mappings.collect { meta, table -> table}.map { tables -> tables.toSorted { a, b -> a.name <=> b.name } } : channel.empty() // channel: [ val(meta), [csv] ]
                                                                                                                   ^^^^
  ```

- Warning: `subworkflows/local/genome_only/main.nf:17:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fasta.view { "Running ${it[0]} on genome only mode"}
                                 ^^
  ```

- Warning: `subworkflows/local/genome_only/main.nf:19:5`: Variable was declared but not used

  ```nextflow
      ch_versions   = channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/genome_only/main.nf:129:101`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      buscos_per_seqs         = !params.skip_busco ? GENOMEBUSCOIDEOGRAM.out.busco_mappings.collect { meta, table -> table}.map { tables -> tables.toSorted { a, b -> a.name <=> b.name } } : channel.empty() // channel: [ csv ]
                                                                                                      ^^^^
  ```
