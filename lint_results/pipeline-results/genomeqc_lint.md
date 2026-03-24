# Nextflow lint results

- Generated: 2026-03-24T00:21:37.042826685Z
- Nextflow version: 26.03.0-edge
- Summary: 26 errors, 102 warnings

## :x: Errors

- Error: `modules/local/extract_seqs.nf:10:16`: `meta` is already declared

  ```nextflow
      tuple val (meta),  path(gff)
                 ^^^^
  ```

- Error: `modules/local/shiny_app/main.nf:12:15`: `meta` is already declared

  ```nextflow
      tuple val(meta), path(tree)
                ^^^^
  ```

- Error: `modules/nf-core/agat/spkeeplongestisoform/main.nf:24:35`: `gff` is not defined

  ```nextflow
      def prefix       = meta.id ?: gff.getBaseName()
                                    ^^^
  ```

- Error: `modules/nf-core/agat/spkeeplongestisoform/main.nf:40:29`: `gff` is not defined

  ```nextflow
      def prefix = meta.id ?: gff.getBaseName()
                              ^^^
  ```

- Error: `modules/nf-core/fcsgx/fetchdb/main.nf:38:41`: `basename` is not defined

  ```nextflow
      prefix = task.ext.prefix ?: "gxdb_${basename}"
                                          ^^^^^^^^
  ```

- Error: `workflows/genomeqc.nf:97:41`: `fasta` is already declared

  ```nextflow
      gz_fasta     = fasta.filter { meta, fasta -> fasta.name.endsWith(".gz") }
                                          ^^^^^
  ```

- Error: `workflows/genomeqc.nf:98:41`: `fasta` is already declared

  ```nextflow
      non_gz_fasta = fasta.filter { meta, fasta -> !fasta.name.endsWith(".gz") }
                                          ^^^^^
  ```

- Error: `workflows/genomeqc.nf:113:31`: `fasta` is already declared

  ```nextflow
                  | map { meta, fasta, gxf, fq ->  tuple( meta,  gxf) }
                                ^^^^^
  ```

- Error: `workflows/genomeqc.nf:117:38`: `gxf` is already declared

  ```nextflow
      gz_gxf      = gxf.filter { meta, gxf -> gxf  && gxf.name.endsWith(".gz")  } // Filter non empty and compressed gxf (channel to be uncompressed)
                                       ^^^
  ```

- Error: `workflows/genomeqc.nf:118:38`: `gxf` is already declared

  ```nextflow
      non_gz_gxf  = gxf.filter { meta, gxf -> !gxf || !gxf.name.endsWith(".gz") } // Filter empty and uncompressed gxf (not uncompressed)
                                       ^^^
  ```

- Error: `workflows/genomeqc.nf:135:51`: `fasta` is already declared

  ```nextflow
                  | mix( ch_input.local.map { meta, fasta, gxf, fq -> tuple( meta, fq ) } )
                                                    ^^^^^
  ```

- Error: `workflows/genomeqc.nf:135:58`: `gxf` is already declared

  ```nextflow
                  | mix( ch_input.local.map { meta, fasta, gxf, fq -> tuple( meta, fq ) } )
                                                           ^^^
  ```

- Error: `workflows/genomeqc.nf:151:46`: `fasta` is already declared

  ```nextflow
      ch_input_anno  = ch_input.filter { meta, fasta, gxf, fastq ->  gxf } // gxf is present. Channel will run on genome and annotation
                                               ^^^^^
  ```

- Error: `workflows/genomeqc.nf:151:53`: `gxf` is already declared

  ```nextflow
      ch_input_anno  = ch_input.filter { meta, fasta, gxf, fastq ->  gxf } // gxf is present. Channel will run on genome and annotation
                                                      ^^^
  ```

- Error: `workflows/genomeqc.nf:152:22`: `multimapChannel` is not defined

  ```nextflow
                     | multimapChannel // Notice only fasta channel and gxf are necessary here
                       ^^^^^^^^^^^^^^^
  ```

- Error: `workflows/genomeqc.nf:153:46`: `fasta` is already declared

  ```nextflow
      ch_input_geno  = ch_input.filter { meta, fasta, gxf, fastq ->  !gxf }// gxf is missing. Channel will run on genome only
                                               ^^^^^
  ```

- Error: `workflows/genomeqc.nf:153:53`: `gxf` is already declared

  ```nextflow
      ch_input_geno  = ch_input.filter { meta, fasta, gxf, fastq ->  !gxf }// gxf is missing. Channel will run on genome only
                                                      ^^^
  ```

- Error: `workflows/genomeqc.nf:154:22`: `multimapChannel` is not defined

  ```nextflow
                     | multimapChannel // Notice only fasta channel is necessary here
                       ^^^^^^^^^^^^^^^
  ```

- Error: `workflows/genomeqc.nf:157:46`: `fasta` is already declared

  ```nextflow
      ch_input_merq  = ch_input.filter { meta, fasta, gxf, fastq -> fastq } // filter rows where fastq is present
                                               ^^^^^
  ```

- Error: `workflows/genomeqc.nf:157:53`: `gxf` is already declared

  ```nextflow
      ch_input_merq  = ch_input.filter { meta, fasta, gxf, fastq -> fastq } // filter rows where fastq is present
                                                      ^^^
  ```

- Error: `workflows/genomeqc.nf:158:22`: `multimapChannel` is not defined

  ```nextflow
                     | multimapChannel // Notice only fasta and fastq channels are necessary here
                       ^^^^^^^^^^^^^^^
  ```

- Error: `workflows/genomeqc.nf:161:46`: `fasta` is already declared

  ```nextflow
      ch_input_decon = ch_fasta.filter { meta, fasta -> meta.taxid } // filter rows where taxid is present. Run decon on those
                                               ^^^^^
  ```

- Error: `workflows/genomeqc.nf:186:54`: `fasta` is already declared

  ```nextflow
      ch_repeat = params.repeat ? ch_fasta.map { meta, fasta -> [ meta, params.repeat ] } : Channel.empty()
                                                       ^^^^^
  ```

- Error: `workflows/genomeqc.nf:441:4`: `multi_ch` was assigned but not declared

  ```nextflow
     multi_ch = input
     ^^^^^^^^
  ```

- Error: `workflows/genomeqc.nf:442:15`: `multiMap` is not defined

  ```nextflow
              | multiMap {
                ^^^^^^^^
  ```

- Error: `workflows/genomeqc.nf:448:12`: `multi_ch` is not defined

  ```nextflow
      return multi_ch
             ^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/buscos_seqs/main.nf:17:9`: Variable was declared but not used

  ```nextflow
      def prefix         = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/extract_seqs.nf:9:16`: Variable was declared but not used

  ```nextflow
      tuple val (meta),  path(fasta)
                 ^^^^
  ```

- Warning: `modules/local/famdb.py/main.nf:20:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/shiny_app/main.nf:11:15`: Variable was declared but not used

  ```nextflow
      tuple val(meta), path(tables)
                ^^^^
  ```

- Warning: `modules/local/shiny_app/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def prefix           = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/shiny_app/main.nf:27:9`: Variable was declared but not used

  ```nextflow
      def results_path     = file(params.outdir).toAbsolutePath()
          ^^^^^^^^^^^^
  ```

- Warning: `modules/local/tree_summary.nf:26:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/agat/convertspgxf2gxf/main.nf:37:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/agat/spstatistics/main.nf:36:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/cat/cat/main.nf:23:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def file_list = files_in.collect { it.toString() }
                                         ^^
  ```

- Warning: `modules/nf-core/cat/cat/main.nf:58:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def file_list   = files_in.collect { it.toString() }
                                           ^^
  ```

- Warning: `modules/nf-core/cdhit/cdhitest/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/cdhit/cdhitest/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:26:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      suffix    = task.ext.suffix ?: "${input.collect{ it.getExtension()}.get(0)}" // use the first extension of the input files
                                                       ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:29:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      lst_gz     = input.findResults{ it.getExtension().endsWith("gz") ? it.toString() : null }
                                      ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:29:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      lst_gz     = input.findResults{ it.getExtension().endsWith("gz") ? it.toString() : null }
                                                                         ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:31:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      input_cmd  = input.collect { it.toString() - ~/\.gz$/ }.join(" ")
                                   ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:34:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      cleanup    = lst_gz ? "rm ${lst_gz.collect{ it - ~/\.gz$/ }.join(" ")}" : ""
                                                  ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:37:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          assert it.name != "${prefix}.${suffix}" : "Input and output names are the same, set prefix in module configuration to disambiguate!"
                 ^^
  ```

- Warning: `modules/nf-core/gffread/main.nf:26:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def extension   = args.contains("-T")       ? 'gtf' : ( ( ['-w', '-x', '-y' ].any { args.contains(it) } ) ? 'fasta' : 'gff3' )
                                                                                                        ^^
  ```

- Warning: `modules/nf-core/gffread/main.nf:30:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def args_sorted = args.replaceAll(/(.*)(-[wxy])(.*)/) { all, pre, param, post -> "$pre $post $param" }.trim()
                                                              ^^^
  ```

- Warning: `modules/nf-core/gffread/main.nf:49:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def extension   = args.contains("-T")       ? 'gtf' : ( ( ['-w', '-x', '-y' ].any { args.contains(it) } ) ? 'fasta' : 'gff3' )
                                                                                                        ^^
  ```

- Warning: `modules/nf-core/meryl/count/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/meryl/count/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/meryl/count/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/meryl/unionsum/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/ncbigenomedownload/main.nf:37:9`: Variable was declared but not used

  ```nextflow
      def prefix         = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/orthofinder/main.nf:54:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args   ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/orthofinder/main.nf:56:9`: Variable was declared but not used

  ```nextflow
      def include_command = prior_run   ? "-b $prior_run" : ''
          ^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/pigz/uncompress/main.nf:39:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/quast/main.nf:52:9`: Variable was declared but not used

  ```nextflow
      def args      = task.ext.args   ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/quast/main.nf:54:9`: Variable was declared but not used

  ```nextflow
      def features  = gff             ? "--features $gff" : ''
          ^^^^^^^^
  ```

- Warning: `modules/nf-core/quast/main.nf:55:9`: Variable was declared but not used

  ```nextflow
      def reference = fasta           ? "-r $fasta" : ''
          ^^^^^^^^^
  ```

- Warning: `modules/nf-core/tidk/explore/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/tidk/plot/main.nf:37:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/decontamination.nf:22:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions        = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/decontamination.nf:44:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gxdb_manifest ?: Channel.empty() // If there no manifest, use empty channel (won't run)
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:25:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fasta.view { "Running ${it[0]} on genome and annotation mode"}
                                 ^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:27:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions  = Channel.empty()
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:30:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_tree_data = Channel.empty()
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:114:80`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_tree_data = ch_tree_data.mix(GENE_OVERLAPS.out.overlap_counts.collect { meta, file -> file })
                                                                                 ^^^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:137:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_input.fasta.map { meta, fasta -> fasta}
                               ^^^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:157:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          | map { meta, fasta ->
                  ^^^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:180:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ORTHOFINDER.out.orthofinder.map { meta, folder ->
                                            ^^^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:183:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          AGAT_SPKEEPLONGESTISOFORM.out.gff.map { meta, gff -> gff }.collect()
                                                  ^^^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:283:96`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      buscos_per_seqs            = GENOME_ANNOTATION_BUSCO_IDEOGRAM.out.busco_mappings.collect { meta, table -> table} // channel: [ val(meta), [csv] ]
                                                                                                 ^^^^
  ```

- Warning: `subworkflows/local/genome_only.nf:15:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fasta.view { "Running ${it[0]} on genome only mode"}
                                 ^^
  ```

- Warning: `subworkflows/local/genome_only.nf:17:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions   = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/genome_only.nf:20:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_tree_data = Channel.empty()
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/genome_only.nf:56:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_tree_data  = ch_tree_data.mix(GAWK.out.output.collect { meta, file -> file })
                                                                 ^^^^
  ```

- Warning: `subworkflows/local/genome_only.nf:112:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ORTHOFINDER.out.orthofinder.map { meta, folder ->
                                            ^^^^
  ```

- Warning: `subworkflows/local/genome_only.nf:115:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          BUSCO_TSV_TO_GFF.out.gff.map { meta, gff -> gff }.collect()
                                         ^^^^
  ```

- Warning: `subworkflows/local/genome_only.nf:125:87`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      buscos_per_seqs         = GENOME_ONLY_BUSCO_IDEOGRAM.out.busco_mappings.collect { meta, table -> table} // channel: [ csv ]
                                                                                        ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomeqc_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomeqc_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_explore_search_plot_tidk/main.nf:19:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_explore_search_plot_tidk/main.nf:43:58`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                                  ( ch_apriori_sequence ?: Channel.empty() )
                                                           ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_explore_search_plot_tidk/main.nf:46:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              | map { id, meta, fasta, seq -> [ meta, fasta, seq ] }
                                      ^^
  ```

- Warning: `subworkflows/nf-core/fasta_explore_search_plot_tidk/main.nf:49:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_apriori_inputs.map { meta, fasta, seq -> [ meta, fasta ] },
                                               ^^^
  ```

- Warning: `subworkflows/nf-core/fasta_explore_search_plot_tidk/main.nf:50:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_apriori_inputs.map { meta, fasta, seq -> seq }
                                  ^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_explore_search_plot_tidk/main.nf:50:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_apriori_inputs.map { meta, fasta, seq -> seq }
                                        ^^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_explore_search_plot_tidk/main.nf:64:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_aposteriori_inputs.map { meta, fasta, seq -> [ meta, fasta ] },
                                                   ^^^
  ```

- Warning: `subworkflows/nf-core/fasta_explore_search_plot_tidk/main.nf:65:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_aposteriori_inputs.map { meta, fasta, seq -> seq }
                                      ^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_explore_search_plot_tidk/main.nf:65:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_aposteriori_inputs.map { meta, fasta, seq -> seq }
                                            ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:48:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      validateInputSamplesheet(it) // Input validation (check local subworkflow for how function works)
                                               ^^
  ```

- Warning: `workflows/genomeqc.nf:62:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          | map { meta, refseq, fq -> tuple( meta, refseq ) }
                                ^^
  ```

- Warning: `workflows/genomeqc.nf:93:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                   | map { meta, fasta, gxf, fq -> tuple( meta, fasta) }
                                        ^^^
  ```

- Warning: `workflows/genomeqc.nf:93:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                   | map { meta, fasta, gxf, fq -> tuple( meta, fasta) }
                                             ^^
  ```

- Warning: `workflows/genomeqc.nf:97:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      gz_fasta     = fasta.filter { meta, fasta -> fasta.name.endsWith(".gz") }
                                    ^^^^
  ```

- Warning: `workflows/genomeqc.nf:98:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      non_gz_fasta = fasta.filter { meta, fasta -> !fasta.name.endsWith(".gz") }
                                    ^^^^
  ```

- Warning: `workflows/genomeqc.nf:113:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  | map { meta, fasta, gxf, fq ->  tuple( meta,  gxf) }
                                ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:113:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  | map { meta, fasta, gxf, fq ->  tuple( meta,  gxf) }
                                            ^^
  ```

- Warning: `workflows/genomeqc.nf:117:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      gz_gxf      = gxf.filter { meta, gxf -> gxf  && gxf.name.endsWith(".gz")  } // Filter non empty and compressed gxf (channel to be uncompressed)
                                 ^^^^
  ```

- Warning: `workflows/genomeqc.nf:118:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      non_gz_gxf  = gxf.filter { meta, gxf -> !gxf || !gxf.name.endsWith(".gz") } // Filter empty and uncompressed gxf (not uncompressed)
                                 ^^^^
  ```

- Warning: `workflows/genomeqc.nf:134:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  | map{ meta, refseq, fq -> tuple( meta, fq ) }
                               ^^^^^^
  ```

- Warning: `workflows/genomeqc.nf:135:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  | mix( ch_input.local.map { meta, fasta, gxf, fq -> tuple( meta, fq ) } )
                                                    ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:135:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  | mix( ch_input.local.map { meta, fasta, gxf, fq -> tuple( meta, fq ) } )
                                                           ^^^
  ```

- Warning: `workflows/genomeqc.nf:151:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_anno  = ch_input.filter { meta, fasta, gxf, fastq ->  gxf } // gxf is present. Channel will run on genome and annotation
                                         ^^^^
  ```

- Warning: `workflows/genomeqc.nf:151:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_anno  = ch_input.filter { meta, fasta, gxf, fastq ->  gxf } // gxf is present. Channel will run on genome and annotation
                                               ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:151:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_anno  = ch_input.filter { meta, fasta, gxf, fastq ->  gxf } // gxf is present. Channel will run on genome and annotation
                                                           ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:153:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_geno  = ch_input.filter { meta, fasta, gxf, fastq ->  !gxf }// gxf is missing. Channel will run on genome only
                                         ^^^^
  ```

- Warning: `workflows/genomeqc.nf:153:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_geno  = ch_input.filter { meta, fasta, gxf, fastq ->  !gxf }// gxf is missing. Channel will run on genome only
                                               ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:153:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_geno  = ch_input.filter { meta, fasta, gxf, fastq ->  !gxf }// gxf is missing. Channel will run on genome only
                                                           ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:157:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_merq  = ch_input.filter { meta, fasta, gxf, fastq -> fastq } // filter rows where fastq is present
                                         ^^^^
  ```

- Warning: `workflows/genomeqc.nf:157:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_merq  = ch_input.filter { meta, fasta, gxf, fastq -> fastq } // filter rows where fastq is present
                                               ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:157:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_merq  = ch_input.filter { meta, fasta, gxf, fastq -> fastq } // filter rows where fastq is present
                                                      ^^^
  ```

- Warning: `workflows/genomeqc.nf:161:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_decon = ch_fasta.filter { meta, fasta -> meta.taxid } // filter rows where taxid is present. Run decon on those
                                               ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:186:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_repeat = params.repeat ? ch_fasta.map { meta, fasta -> [ meta, params.repeat ] } : Channel.empty()
                                                       ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:186:91`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_repeat = params.repeat ? ch_fasta.map { meta, fasta -> [ meta, params.repeat ] } : Channel.empty()
                                                                                            ^^^^^^^
  ```

- Warning: `workflows/genomeqc.nf:221:5`: Variable was declared but not used

  ```nextflow
      ch_merqury_outputs                      = ch_merqury_qv
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/genomeqc.nf:226:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                              | flatMap { meta, data -> data }
                                                          ^^^^
  ```

- Warning: `workflows/genomeqc.nf:238:68`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                           | mix(GENOME_ONLY.out.quast_results.map { meta, results -> results })
                                                                     ^^^^
  ```

- Warning: `workflows/genomeqc.nf:239:76`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                           | mix(GENOME_ONLY.out.busco_short_summaries.map { meta, txt -> txt })
                                                                             ^^^^
  ```

- Warning: `workflows/genomeqc.nf:250:78`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                           | mix(GENOME_AND_ANNOTATION.out.quast_results.map { meta, results -> results })
                                                                               ^^^^
  ```

- Warning: `workflows/genomeqc.nf:251:91`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                           | mix(GENOME_AND_ANNOTATION.out.busco_short_summaries_prot.map { meta, txt -> txt })
                                                                                            ^^^^
  ```

- Warning: `workflows/genomeqc.nf:269:77`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              | concat(BUSCO_SEQS_GENOME_ANNO.out.table.map { meta, table -> table})
                                                                              ^^^^
  ```

- Warning: `workflows/genomeqc.nf:272:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              | concat(BUSCO_SEQS_GENOME.out.table.map { meta, table -> table})
                                                                         ^^^^
  ```

- Warning: `workflows/genomeqc.nf:281:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              | map { meta, file -> file }
                                      ^^^^
  ```

- Warning: `workflows/genomeqc.nf:286:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              | map { meta, file -> file }
                                      ^^^^
  ```

- Warning: `workflows/genomeqc.nf:322:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_functions = Channel.fromPath("$projectDir/bin/tree_functions.R", checkIfExists: true)
                         ^^^^^^^
  ```

- Warning: `workflows/genomeqc.nf:323:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_app       = Channel.fromPath("$projectDir/bin/shiny_app.R", checkIfExists: true)
                         ^^^^^^^
  ```

- Warning: `workflows/genomeqc.nf:347:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
