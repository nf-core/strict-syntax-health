# Nextflow lint results

- Generated: 2026-05-13T00:40:41.504733510Z
- Nextflow version: 26.04.1
- Summary: 60 warnings

## :warning: Warnings

- Warning: `conf/modules.config:162:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { (!it.endsWith('.bam') || params.save_align_intermeds) ? it : null }
                          ^^
  ```

- Warning: `conf/modules.config:162:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { (!it.endsWith('.bam') || params.save_align_intermeds) ? it : null }
                                                                                ^^
  ```

- Warning: `subworkflows/local/align_cellranger.nf:45:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  if ( it.toString().contains("raw_feature_bc_matrix") ) { desired_files.add( it ) }
                       ^^
  ```

- Warning: `subworkflows/local/align_cellranger.nf:45:93`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  if ( it.toString().contains("raw_feature_bc_matrix") ) { desired_files.add( it ) }
                                                                                              ^^
  ```

- Warning: `subworkflows/local/align_cellranger.nf:54:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  if ( it.toString().contains("filtered_feature_bc_matrix") ) { desired_files.add( it ) }
                       ^^
  ```

- Warning: `subworkflows/local/align_cellranger.nf:54:98`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  if ( it.toString().contains("filtered_feature_bc_matrix") ) { desired_files.add( it ) }
                                                                                                   ^^
  ```

- Warning: `subworkflows/local/align_cellrangerarc.nf:70:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          mtx_files.each{ if ( it.toString().contains("${pattern}") ) { desired_files.add( it ) } }
                               ^^
  ```

- Warning: `subworkflows/local/align_cellrangerarc.nf:70:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          mtx_files.each{ if ( it.toString().contains("${pattern}") ) { desired_files.add( it ) } }
                                                                                           ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:32:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def data_dict  = meta_clone.find{ it.key == "${meta_clone.feature_type}" }
                                                ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:62:9`: Variable was declared but not used

  ```nextflow
          ch_gex_barcodes           = params.gex_barcode_sample_assignment ? file(params.gex_barcode_sample_assignment) : []
          ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:93:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{ [it[0].id] }
                     ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:94:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .concat( PARSE_CELLRANGERMULTI_SAMPLESHEET.out.cmo.flatten().map { [ "${it.baseName}" - "_cmo", it ] } )
                                                                                      ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:94:109`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .concat( PARSE_CELLRANGERMULTI_SAMPLESHEET.out.cmo.flatten().map { [ "${it.baseName}" - "_cmo", it ] } )
                                                                                                              ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:96:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { if ( it.size() == 2 ) { it[1] } else { [] } } // a correct tuple from snippet will have: [ sample, cmo.csv ]
                          ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:96:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { if ( it.size() == 2 ) { it[1] } else { [] } } // a correct tuple from snippet will have: [ sample, cmo.csv ]
                                             ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:101:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{ [it[0].id] }
                     ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:102:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .concat( PARSE_CELLRANGERMULTI_SAMPLESHEET.out.ocm.flatten().map { [ "${it.baseName}" - "_ocm", it ] } )
                                                                                      ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:102:109`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .concat( PARSE_CELLRANGERMULTI_SAMPLESHEET.out.ocm.flatten().map { [ "${it.baseName}" - "_ocm", it ] } )
                                                                                                              ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:104:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { if ( it.size() == 2 ) { it[1] } else { [] } } // a correct tuple from snippet will have: [ sample, ocm.csv ]
                          ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:104:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { if ( it.size() == 2 ) { it[1] } else { [] } } // a correct tuple from snippet will have: [ sample, ocm.csv ]
                                             ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:109:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map{ [it[0].id] }
                     ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:110:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .concat( PARSE_CELLRANGERMULTI_SAMPLESHEET.out.frna.flatten().map { [ "${it.baseName}" - "_frna", it ] } )
                                                                                       ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:110:111`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .concat( PARSE_CELLRANGERMULTI_SAMPLESHEET.out.frna.flatten().map { [ "${it.baseName}" - "_frna", it ] } )
                                                                                                                ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:112:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { if ( it.size() == 2 ) { it[1] } else { [] } } // a correct tuple from snippet will have: [ sample, frna.csv ]
                          ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:112:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { if ( it.size() == 2 ) { it[1] } else { [] } } // a correct tuple from snippet will have: [ sample, frna.csv ]
                                             ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:200:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_grouped_fastq.gex.map{ it[0] },
                                        ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:247:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              mtx_files.each{ if ( it.toString().contains("${pattern}") ) { desired_files.add( it ) } }
                                   ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:247:94`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              mtx_files.each{ if ( it.toString().contains("${pattern}") ) { desired_files.add( it ) } }
                                                                                               ^^
  ```

- Warning: `subworkflows/local/align_cellrangermulti.nf:263:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter{ it != null } // remove nulls from previous step
                   ^^
  ```

- Warning: `subworkflows/local/fastqc.nf:29:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      fastqc_multiqc = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/kallisto_bustools.nf:20:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/simpleaf.nf:23:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/simpleaf.nf:63:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  txp2gene = Channel.of( txp2gene )
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/simpleaf.nf:67:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              simpleaf_index = Channel.of( [ [:], [] ] )
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/simpleaf.nf:72:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          simpleaf_index = Channel.of( [ [ id: simpleaf_index.getName() ], simpleaf_index ] )
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/simpleaf.nf:76:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              txp2gene = Channel.of( txp2gene )
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/simpleaf.nf:122:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_qcatch_report = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/starsolo.nf:72:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      for_multiqc     = STAR_ALIGN.out.log_final.map{ meta, it -> it }
                                                      ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_scrnaseq_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_scrnaseq_pipeline/main.nf:110:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel
          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_scrnaseq_pipeline/main.nf:121:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map{ id, type, meta, reads -> [ id, meta, reads ] }
                        ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_scrnaseq_pipeline/main.nf:123:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  validateInputSamplesheet(it)
                                           ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_scrnaseq_pipeline/main.nf:131:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel
          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_scrnaseq_pipeline/main.nf:145:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  cellrangerarcStructure(it)
                                         ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_scrnaseq_pipeline/main.nf:149:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel
          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_scrnaseq_pipeline/main.nf:161:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  validateInputSamplesheet(it)
                                           ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_scrnaseq_pipeline/main.nf:244:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def inputSamples = file(params.input).splitCsv(header: true).collect { it.sample }.toSet()
                                                                             ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_scrnaseq_pipeline/main.nf:271:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def errorDetails = rowsWithoutBarcodes.collect { "row ${it.row} (${it.multiplexed_sample_id})" }.join(', ')
                                                                  ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_scrnaseq_pipeline/main.nf:271:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def errorDetails = rowsWithoutBarcodes.collect { "row ${it.row} (${it.multiplexed_sample_id})" }.join(', ')
                                                                             ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_scrnaseq_pipeline/main.nf:278:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def samplesWithMixedBarcodes = sampleBarcodeTypes.findAll { multiplexed_sample_id, info -> info.types.size() > 1 }
                                                                  ^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_scrnaseq_pipeline/main.nf:324:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def sample_type_ok = metas.collect { meta -> meta.sample_type }.unique().every { it in valid_sample_types }
                                                                                       ^^
  ```

- Warning: `workflows/scrnaseq.nf:103:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_genome_fasta    = GUNZIP_FASTA ( [ [:], ch_genome_fasta ] ).gunzip.map { it[1] }
                                                                                          ^^
  ```

- Warning: `workflows/scrnaseq.nf:114:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gtf      = GUNZIP_GTF ( [ [:], ch_gtf ] ).gunzip.map { it[1] }
                                                                        ^^
  ```

- Warning: `workflows/scrnaseq.nf:199:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, outs -> outs.findAll{ it -> it.name == "web_summary.html"}
              ^^^^
  ```

- Warning: `workflows/scrnaseq.nf:257:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (!map_collection_clone.any{ it.feature_type == 'gex' })    { map_collection_clone.add( [id: sample_id, feature_type: 'gex'   , gex:    empty_file, options:[:] ] ) }
                                             ^^
  ```

- Warning: `workflows/scrnaseq.nf:258:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (!map_collection_clone.any{ it.feature_type == 'vdj' })    { map_collection_clone.add( [id: sample_id, feature_type: 'vdj'   , vdj:    empty_file, options:[:] ] ) }
                                             ^^
  ```

- Warning: `workflows/scrnaseq.nf:259:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (!map_collection_clone.any{ it.feature_type == 'ab' })     { map_collection_clone.add( [id: sample_id, feature_type: 'ab'    , ab:     empty_file, options:[:] ] ) }
                                             ^^
  ```

- Warning: `workflows/scrnaseq.nf:260:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (!map_collection_clone.any{ it.feature_type == 'beam' })   { map_collection_clone.add( [id: sample_id, feature_type: 'beam'  , beam:   empty_file, options:[:] ] ) } // currently not implemented, the input samplesheet checking will not allow it.
                                             ^^
  ```

- Warning: `workflows/scrnaseq.nf:261:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (!map_collection_clone.any{ it.feature_type == 'crispr' }) { map_collection_clone.add( [id: sample_id, feature_type: 'crispr', crispr: empty_file, options:[:] ] ) }
                                             ^^
  ```

- Warning: `workflows/scrnaseq.nf:262:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (!map_collection_clone.any{ it.feature_type == 'cmo' })    { map_collection_clone.add( [id: sample_id, feature_type: 'cmo'   , cmo:    empty_file, options:[:] ] ) }
                                             ^^
  ```
