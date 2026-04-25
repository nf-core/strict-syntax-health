# Nextflow lint results

- Generated: 2026-04-25T00:29:10.053292100Z
- Nextflow version: 26.03.3-edge
- Summary: 22 errors, 57 warnings

## :x: Errors

- Error: `modules/local/shiny_app/main.nf:12:15`: `meta` is already declared

  ```nextflow
      tuple val(meta), path(tree)
                ^^^^
  ```

- Error: `workflows/genomeqc.nf:96:41`: `fasta` is already declared

  ```nextflow
      gz_fasta     = fasta.filter { meta, fasta -> fasta.name.endsWith(".gz") }
                                          ^^^^^
  ```

- Error: `workflows/genomeqc.nf:97:41`: `fasta` is already declared

  ```nextflow
      non_gz_fasta = fasta.filter { meta, fasta -> !fasta.name.endsWith(".gz") }
                                          ^^^^^
  ```

- Error: `workflows/genomeqc.nf:111:31`: `fasta` is already declared

  ```nextflow
                  | map { meta, fasta, gxf, fq ->  tuple( meta,  gxf) }
                                ^^^^^
  ```

- Error: `workflows/genomeqc.nf:115:38`: `gxf` is already declared

  ```nextflow
      gz_gxf      = gxf.filter { meta, gxf -> gxf  && gxf.name.endsWith(".gz")  } // Filter non empty and compressed gxf (channel to be uncompressed)
                                       ^^^
  ```

- Error: `workflows/genomeqc.nf:116:38`: `gxf` is already declared

  ```nextflow
      non_gz_gxf  = gxf.filter { meta, gxf -> !gxf || !gxf.name.endsWith(".gz") } // Filter empty and uncompressed gxf (not uncompressed)
                                       ^^^
  ```

- Error: `workflows/genomeqc.nf:132:51`: `fasta` is already declared

  ```nextflow
                  | mix( ch_input.local.map { meta, fasta, gxf, fq -> tuple( meta, fq ) } )
                                                    ^^^^^
  ```

- Error: `workflows/genomeqc.nf:132:58`: `gxf` is already declared

  ```nextflow
                  | mix( ch_input.local.map { meta, fasta, gxf, fq -> tuple( meta, fq ) } )
                                                           ^^^
  ```

- Error: `workflows/genomeqc.nf:148:46`: `fasta` is already declared

  ```nextflow
      ch_input_anno  = ch_input.filter { meta, fasta, gxf, fastq ->  gxf } // gxf is present. Channel will run on genome and annotation
                                               ^^^^^
  ```

- Error: `workflows/genomeqc.nf:148:53`: `gxf` is already declared

  ```nextflow
      ch_input_anno  = ch_input.filter { meta, fasta, gxf, fastq ->  gxf } // gxf is present. Channel will run on genome and annotation
                                                      ^^^
  ```

- Error: `workflows/genomeqc.nf:149:22`: `multimapChannel` is not defined

  ```nextflow
                     | multimapChannel // Notice only fasta channel and gxf are necessary here
                       ^^^^^^^^^^^^^^^
  ```

- Error: `workflows/genomeqc.nf:150:46`: `fasta` is already declared

  ```nextflow
      ch_input_geno  = ch_input.filter { meta, fasta, gxf, fastq ->  !gxf }// gxf is missing. Channel will run on genome only
                                               ^^^^^
  ```

- Error: `workflows/genomeqc.nf:150:53`: `gxf` is already declared

  ```nextflow
      ch_input_geno  = ch_input.filter { meta, fasta, gxf, fastq ->  !gxf }// gxf is missing. Channel will run on genome only
                                                      ^^^
  ```

- Error: `workflows/genomeqc.nf:151:22`: `multimapChannel` is not defined

  ```nextflow
                     | multimapChannel // Notice only fasta channel is necessary here
                       ^^^^^^^^^^^^^^^
  ```

- Error: `workflows/genomeqc.nf:154:46`: `fasta` is already declared

  ```nextflow
      ch_input_merq  = ch_input.filter { meta, fasta, gxf, fastq -> fastq } // filter rows where fastq is present
                                               ^^^^^
  ```

- Error: `workflows/genomeqc.nf:154:53`: `gxf` is already declared

  ```nextflow
      ch_input_merq  = ch_input.filter { meta, fasta, gxf, fastq -> fastq } // filter rows where fastq is present
                                                      ^^^
  ```

- Error: `workflows/genomeqc.nf:155:22`: `multimapChannel` is not defined

  ```nextflow
                     | multimapChannel // Notice only fasta and fastq channels are necessary here
                       ^^^^^^^^^^^^^^^
  ```

- Error: `workflows/genomeqc.nf:158:46`: `fasta` is already declared

  ```nextflow
      ch_input_decon = ch_fasta.filter { meta, fasta -> meta.taxid } // filter rows where taxid is present. Run decon on those
                                               ^^^^^
  ```

- Error: `workflows/genomeqc.nf:182:54`: `fasta` is already declared

  ```nextflow
      ch_repeat = params.repeat ? ch_fasta.map { meta, fasta -> [ meta, params.repeat ] } : channel.empty()
                                                       ^^^^^
  ```

- Error: `workflows/genomeqc.nf:411:4`: `multi_ch` was assigned but not declared

  ```nextflow
     multi_ch = input
     ^^^^^^^^
  ```

- Error: `workflows/genomeqc.nf:412:15`: `multiMap` is not defined

  ```nextflow
              | multiMap {
                ^^^^^^^^
  ```

- Error: `workflows/genomeqc.nf:418:12`: `multi_ch` is not defined

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

- Warning: `subworkflows/local/genome_and_annotation.nf:96:80`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_tree_data = ch_tree_data.mix(GENE_OVERLAPS.out.overlap_counts.collect { meta, file -> file })
                                                                                 ^^^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:118:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_input.fasta.map { meta, fasta -> fasta}
                               ^^^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:136:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          | map { meta, fasta ->
                  ^^^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:158:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ORTHOFINDER.out.orthofinder.map { meta, folder ->
                                            ^^^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:161:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          AGAT_SPKEEPLONGESTISOFORM.out.gff.map { meta, gff -> gff }.collect()
                                                  ^^^^
  ```

- Warning: `subworkflows/local/genome_and_annotation.nf:255:96`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      buscos_per_seqs            = GENOME_ANNOTATION_BUSCO_IDEOGRAM.out.busco_mappings.collect { meta, table -> table} // channel: [ val(meta), [csv] ]
                                                                                                 ^^^^
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

- Warning: `subworkflows/local/genome_only.nf:53:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_tree_data  = ch_tree_data.mix(GAWK.out.output.collect { meta, file -> file })
                                                                 ^^^^
  ```

- Warning: `subworkflows/local/genome_only.nf:106:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ORTHOFINDER.out.orthofinder.map { meta, folder ->
                                            ^^^^
  ```

- Warning: `subworkflows/local/genome_only.nf:109:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          BUSCO_TSV_TO_GFF.out.gff.map { meta, gff -> gff }.collect()
                                         ^^^^
  ```

- Warning: `subworkflows/local/genome_only.nf:118:87`: Parameter was not used -- prefix with `_` to suppress warning

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

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
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

- Warning: `workflows/genomeqc.nf:92:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                   | map { meta, fasta, gxf, fq -> tuple( meta, fasta) }
                                        ^^^
  ```

- Warning: `workflows/genomeqc.nf:92:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                   | map { meta, fasta, gxf, fq -> tuple( meta, fasta) }
                                             ^^
  ```

- Warning: `workflows/genomeqc.nf:96:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      gz_fasta     = fasta.filter { meta, fasta -> fasta.name.endsWith(".gz") }
                                    ^^^^
  ```

- Warning: `workflows/genomeqc.nf:97:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      non_gz_fasta = fasta.filter { meta, fasta -> !fasta.name.endsWith(".gz") }
                                    ^^^^
  ```

- Warning: `workflows/genomeqc.nf:111:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  | map { meta, fasta, gxf, fq ->  tuple( meta,  gxf) }
                                ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:111:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  | map { meta, fasta, gxf, fq ->  tuple( meta,  gxf) }
                                            ^^
  ```

- Warning: `workflows/genomeqc.nf:115:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      gz_gxf      = gxf.filter { meta, gxf -> gxf  && gxf.name.endsWith(".gz")  } // Filter non empty and compressed gxf (channel to be uncompressed)
                                 ^^^^
  ```

- Warning: `workflows/genomeqc.nf:116:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      non_gz_gxf  = gxf.filter { meta, gxf -> !gxf || !gxf.name.endsWith(".gz") } // Filter empty and uncompressed gxf (not uncompressed)
                                 ^^^^
  ```

- Warning: `workflows/genomeqc.nf:131:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  | map{ meta, refseq, fq -> tuple( meta, fq ) }
                               ^^^^^^
  ```

- Warning: `workflows/genomeqc.nf:132:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  | mix( ch_input.local.map { meta, fasta, gxf, fq -> tuple( meta, fq ) } )
                                                    ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:132:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  | mix( ch_input.local.map { meta, fasta, gxf, fq -> tuple( meta, fq ) } )
                                                           ^^^
  ```

- Warning: `workflows/genomeqc.nf:148:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_anno  = ch_input.filter { meta, fasta, gxf, fastq ->  gxf } // gxf is present. Channel will run on genome and annotation
                                         ^^^^
  ```

- Warning: `workflows/genomeqc.nf:148:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_anno  = ch_input.filter { meta, fasta, gxf, fastq ->  gxf } // gxf is present. Channel will run on genome and annotation
                                               ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:148:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_anno  = ch_input.filter { meta, fasta, gxf, fastq ->  gxf } // gxf is present. Channel will run on genome and annotation
                                                           ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:150:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_geno  = ch_input.filter { meta, fasta, gxf, fastq ->  !gxf }// gxf is missing. Channel will run on genome only
                                         ^^^^
  ```

- Warning: `workflows/genomeqc.nf:150:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_geno  = ch_input.filter { meta, fasta, gxf, fastq ->  !gxf }// gxf is missing. Channel will run on genome only
                                               ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:150:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_geno  = ch_input.filter { meta, fasta, gxf, fastq ->  !gxf }// gxf is missing. Channel will run on genome only
                                                           ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:154:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_merq  = ch_input.filter { meta, fasta, gxf, fastq -> fastq } // filter rows where fastq is present
                                         ^^^^
  ```

- Warning: `workflows/genomeqc.nf:154:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_merq  = ch_input.filter { meta, fasta, gxf, fastq -> fastq } // filter rows where fastq is present
                                               ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:154:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_merq  = ch_input.filter { meta, fasta, gxf, fastq -> fastq } // filter rows where fastq is present
                                                      ^^^
  ```

- Warning: `workflows/genomeqc.nf:158:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_input_decon = ch_fasta.filter { meta, fasta -> meta.taxid } // filter rows where taxid is present. Run decon on those
                                               ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:182:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_repeat = params.repeat ? ch_fasta.map { meta, fasta -> [ meta, params.repeat ] } : channel.empty()
                                                       ^^^^^
  ```

- Warning: `workflows/genomeqc.nf:215:5`: Variable was declared but not used

  ```nextflow
      ch_merqury_outputs                      = ch_merqury_qv
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/genomeqc.nf:220:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                              | flatMap { meta, data -> data }
                                                          ^^^^
  ```

- Warning: `workflows/genomeqc.nf:231:68`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                           | mix(GENOME_ONLY.out.quast_results.map { meta, results -> results })
                                                                     ^^^^
  ```

- Warning: `workflows/genomeqc.nf:232:76`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                           | mix(GENOME_ONLY.out.busco_short_summaries.map { meta, txt -> txt })
                                                                             ^^^^
  ```

- Warning: `workflows/genomeqc.nf:242:78`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                           | mix(GENOME_AND_ANNOTATION.out.quast_results.map { meta, results -> results })
                                                                               ^^^^
  ```

- Warning: `workflows/genomeqc.nf:243:91`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                           | mix(GENOME_AND_ANNOTATION.out.busco_short_summaries_prot.map { meta, txt -> txt })
                                                                                            ^^^^
  ```

- Warning: `workflows/genomeqc.nf:260:77`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              | concat(BUSCO_SEQS_GENOME_ANNO.out.table.map { meta, table -> table})
                                                                              ^^^^
  ```

- Warning: `workflows/genomeqc.nf:263:72`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              | concat(BUSCO_SEQS_GENOME.out.table.map { meta, table -> table})
                                                                         ^^^^
  ```

- Warning: `workflows/genomeqc.nf:272:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              | map { meta, file -> file }
                                      ^^^^
  ```

- Warning: `workflows/genomeqc.nf:277:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                              | map { meta, file -> file }
                                      ^^^^
  ```
