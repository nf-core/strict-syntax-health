# Nextflow lint results

- Generated: 2026-02-13T00:21:54.528341502Z
- Nextflow version: 26.01.1-edge
- Summary: 8 errors, 81 warnings

## :x: Errors

- Error: `modules/local/create_anndata_mudata/main.nf:34:9`: `prefix` is already declared

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Error: `modules/local/extract_hashes/main.nf:33:9`: `prefix` is already declared

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Error: `modules/local/gene_summary/main.nf:34:9`: `prefix` is already declared

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Error: `modules/local/hash_summary/main.nf:39:9`: `prefix` is already declared

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Error: `modules/local/htodemux_visualization/main.nf:59:9`: `prefix` is already declared

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Error: `modules/local/preprocessing_for_htodemux_multiseq/main.nf:38:9`: `prefix` is already declared

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Error: `modules/nf-core/demuxem/main.nf:51:9`: `prefix` is already declared

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Error: `subworkflows/local/hash_demultiplexing/main.nf:115:57`: `gmmdemux_estimated_n_cells` is not defined

  ```nextflow
                      params.gmmdemux_estimated_n_cells ? gmmdemux_estimated_n_cells : [],
                                                          ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/create_anndata_mudata/main.nf:29:5`: Variable was declared but not used

  ```nextflow
      prefix = task.ext.prefix ?: "${meta.id}"
      ^^^^^^
  ```

- Warning: `modules/local/gene_summary/main.nf:29:5`: Variable was declared but not used

  ```nextflow
      prefix = task.ext.prefix ?: "${meta.id}"
      ^^^^^^
  ```

- Warning: `modules/local/hash_summary/main.nf:33:5`: Variable was declared but not used

  ```nextflow
      prefix         = task.ext.prefix         ?: "${meta.id}"
      ^^^^^^
  ```

- Warning: `modules/local/hash_summary/main.nf:34:5`: Variable was declared but not used

  ```nextflow
      hash_list      = "${meta.hto_names}".split(",")
      ^^^^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:27:5`: Variable was declared but not used

  ```nextflow
      ridgePlot      = task.ext.ridgePlot      ?: true         // Generate ridge plot
      ^^^^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:28:5`: Variable was declared but not used

  ```nextflow
      ridgeNCol      = task.ext.ridgeNCol      ?: 2            // Number of columns for ridge plot
      ^^^^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:31:5`: Variable was declared but not used

  ```nextflow
      featureScatter = task.ext.featureScatter ?: true         // Generate feature scatter plot
      ^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:32:5`: Variable was declared but not used

  ```nextflow
      scatterFeat1   = task.ext.scatterFeat1   ?: null         // Feature 1 for scatter plot
      ^^^^^^^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:33:5`: Variable was declared but not used

  ```nextflow
      scatterFeat2   = task.ext.scatterFeat2   ?: null         // Feature 2 for scatter plot
      ^^^^^^^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:36:5`: Variable was declared but not used

  ```nextflow
      vlnPlot        = task.ext.vlnPlot        ?: true         // Generate violin plot
      ^^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:37:5`: Variable was declared but not used

  ```nextflow
      vlnFeatures    = task.ext.vlnFeatures    ?: "nCount_RNA" // Features to plot (gene expression, metrics, PC scores, anything that can be retreived by FetchData)
      ^^^^^^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:38:5`: Variable was declared but not used

  ```nextflow
      vlnLog         = task.ext.vlnLog         ?: true         // Plot the feature axis on log scale
      ^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:41:5`: Variable was declared but not used

  ```nextflow
      tSNE           = task.ext.tSNE           ?: true         // Generate a two dimensional tSNE embedding for HTOs
      ^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:42:5`: Variable was declared but not used

  ```nextflow
      tSNEIdents     = task.ext.tSNEIdents     ?: "Negative"   // What should we remove from the object (we have Singlet,Doublet and Negative)
      ^^^^^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:43:5`: Variable was declared but not used

  ```nextflow
      tSNEInvert     = task.ext.tSNEInvert     ?: true         // Invert tSNE selection
      ^^^^^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:44:5`: Variable was declared but not used

  ```nextflow
      tSNEVerbose    = task.ext.tSNEVerbose    ?: false        // Verbose tSNE
      ^^^^^^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:45:5`: Variable was declared but not used

  ```nextflow
      tSNEApprox     = task.ext.tSNEApprox     ?: false        // Approximate tSNE
      ^^^^^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:46:5`: Variable was declared but not used

  ```nextflow
      tSNEDimMax     = task.ext.tSNEDimMax     ?: 2            // Max number of donors
      ^^^^^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:47:5`: Variable was declared but not used

  ```nextflow
      tSNEPerplexity = task.ext.tSNEPerplexity ?: 100          // Value for perplexity
      ^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:50:5`: Variable was declared but not used

  ```nextflow
      heatMap        = task.ext.heatMap        ?: true         // Generate heatmap
      ^^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:51:5`: Variable was declared but not used

  ```nextflow
      heatMapNcells  = task.ext.heatMapNcells  ?: 500          // Number of cells for heatmap
      ^^^^^^^^^^^^^
  ```

- Warning: `modules/local/htodemux_visualization/main.nf:54:5`: Variable was declared but not used

  ```nextflow
      prefix         = task.ext.prefix         ?: "${meta.id}"
      ^^^^^^
  ```

- Warning: `modules/local/preprocessing_for_htodemux_multiseq/main.nf:24:5`: Variable was declared but not used

  ```nextflow
      sel_method  = task.ext.sel_method  ?: "mean.var.plot" // Selection method
      ^^^^^^^^^^
  ```

- Warning: `modules/local/preprocessing_for_htodemux_multiseq/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      ndelim      = task.ext.ndelim      ?: "_"             // For the initial identity class for each cell, delimiter for the cell's column name
      ^^^^^^
  ```

- Warning: `modules/local/preprocessing_for_htodemux_multiseq/main.nf:26:5`: Variable was declared but not used

  ```nextflow
      n_features  = task.ext.n_features  ?: 2000            // Number of features to be used when finding variable features
      ^^^^^^^^^^
  ```

- Warning: `modules/local/preprocessing_for_htodemux_multiseq/main.nf:27:5`: Variable was declared but not used

  ```nextflow
      assay       = task.ext.assay       ?: "HTO"           // Assay name for hashing modality
      ^^^^^
  ```

- Warning: `modules/local/preprocessing_for_htodemux_multiseq/main.nf:28:5`: Variable was declared but not used

  ```nextflow
      margin      = task.ext.margin      ?: 2               // Margin for normalisation
      ^^^^^^
  ```

- Warning: `modules/local/preprocessing_for_htodemux_multiseq/main.nf:29:5`: Variable was declared but not used

  ```nextflow
      norm_method = task.ext.norm_method ?: "CLR"           // Normalisation method
      ^^^^^^^^^^^
  ```

- Warning: `modules/local/preprocessing_for_htodemux_multiseq/main.nf:30:5`: Variable was declared but not used

  ```nextflow
      gene_col    = task.ext.gene_col    ?: 2               // Specify which column of genes.tsv or features.tsv to use for gene names
      ^^^^^^^^
  ```

- Warning: `modules/local/preprocessing_for_htodemux_multiseq/main.nf:33:5`: Variable was declared but not used

  ```nextflow
      prefix      = task.ext.prefix      ?: "${meta.id}"
      ^^^^^^
  ```

- Warning: `modules/nf-core/gmmdemux/main.nf:62:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `subworkflows/local/bam_qc/main.nf:12:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/genetic_demultiplexing/main.nf:21:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/genetic_demultiplexing/main.nf:22:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_vireo = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/genetic_demultiplexing/main.nf:23:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_demuxlet = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/genetic_demultiplexing/main.nf:24:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_freemuxlet = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/genetic_demultiplexing/main.nf:25:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_souporcell = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/genetic_demultiplexing/main.nf:26:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gt_cells = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/genetic_demultiplexing/main.nf:27:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gt_donors =  Channel.empty()
                      ^^^^^^^
  ```

- Warning: `subworkflows/local/genetic_demultiplexing/main.nf:28:34`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_vireo_filtered_variants = Channel.empty()
                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/genetic_demultiplexing/main.nf:134:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { tuple -> tuple.collect { it == null ? [] : it } }
                                          ^^
  ```

- Warning: `subworkflows/local/genetic_demultiplexing/main.nf:134:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { tuple -> tuple.collect { it == null ? [] : it } }
                                                            ^^
  ```

- Warning: `subworkflows/local/hash_demultiplexing/main.nf:22:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/hash_demultiplexing/main.nf:24:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_htodemux_assignments = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/hash_demultiplexing/main.nf:25:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_htodemux_classifications = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/hash_demultiplexing/main.nf:26:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiseq = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/hash_demultiplexing/main.nf:27:14`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_bff = Channel.empty()
               ^^^^^^^
  ```

- Warning: `subworkflows/local/hash_demultiplexing/main.nf:28:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_demuxem = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/hash_demultiplexing/main.nf:29:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gmmdemux_results = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/hash_demultiplexing/main.nf:30:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gmmdemux_config = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/hash_demultiplexing/main.nf:31:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_hasheddrops_results = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/hash_demultiplexing/main.nf:32:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_hasheddrops_id_to_hash = Channel.empty()
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/hash_demultiplexing/main.nf:33:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_hashsolo = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/hash_demultiplexing/main.nf:51:13`: Variable was declared but not used

  ```nextflow
              ch_assignments = HTODEMUX.out.assignment
              ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/hash_demultiplexing/main.nf:56:13`: Variable was declared but not used

  ```nextflow
              ch_classifications = HTODEMUX.out.classification
              ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/hash_demultiplexing/main.nf:162:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_summary = ch_samplesheet.map { meta, rna, hto -> [meta,hto] }
                                              ^^^
  ```

- Warning: `subworkflows/local/hash_demultiplexing/main.nf:173:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { tuple -> tuple.collect { it == null ? [] : it } }
                                          ^^
  ```

- Warning: `subworkflows/local/hash_demultiplexing/main.nf:173:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { tuple -> tuple.collect { it == null ? [] : it } }
                                                            ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_hadge_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_hadge_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_hadge_pipeline/main.nf:41:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_hadge_pipeline/main.nf:66:144`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      after_text = """${workflow.manifest.doi ? "\n* The pipeline\n" : ""}${workflow.manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${workflow.manifest.doi ? "\n" : ""}
                                                                                                                                                 ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_hadge_pipeline/main.nf:103:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.fromList(samplesheetToList(params.input, "${projectDir}/assets/schema_input.json"))
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_hadge_pipeline/main.nf:217:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      if(meta.hto_names.split(",").any { it.contains('_') }){
                                         ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_hadge_pipeline/main.nf:218:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def bad = meta.hto_names.split(",").findAll { it.contains('_') }.join(', ')
                                                        ^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:101:98`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return ch_versions.unique().map { version -> processVersionsFromYAML(version) }.unique().mix(Channel.of(workflowVersionToYAML()))
                                                                                                   ^^^^^^^
  ```

- Warning: `workflows/hadge.nf:36:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/hadge.nf:37:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_donor_match = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `workflows/hadge.nf:38:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_find_variants = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/hadge.nf:39:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_subset_gt_donors = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `workflows/hadge.nf:40:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/hadge.nf:84:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_genetic = ch_preprocessed.map { meta, rna, _hto, bam, barcodes, vcf -> [meta, bam, barcodes, vcf] }
                                               ^^^
  ```

- Warning: `workflows/hadge.nf:194:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  if (params.mode == 'genetic'){ tuple.collect { it == null ? [] : it } }
                                                                 ^^
  ```

- Warning: `workflows/hadge.nf:194:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  if (params.mode == 'genetic'){ tuple.collect { it == null ? [] : it } }
                                                                                   ^^
  ```

- Warning: `workflows/hadge.nf:268:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_config = Channel.fromPath(
                          ^^^^^^^
  ```

- Warning: `workflows/hadge.nf:273:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.fromPath(params.multiqc_config, checkIfExists: true)
            ^^^^^^^
  ```

- Warning: `workflows/hadge.nf:274:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.empty()
            ^^^^^^^
  ```

- Warning: `workflows/hadge.nf:276:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.fromPath(params.multiqc_logo, checkIfExists: true)
            ^^^^^^^
  ```

- Warning: `workflows/hadge.nf:277:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.empty()
            ^^^^^^^
  ```

- Warning: `workflows/hadge.nf:283:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_workflow_summary = Channel.value(paramsSummaryMultiqc(summary_params))
                            ^^^^^^^
  ```

- Warning: `workflows/hadge.nf:290:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_methods_description = Channel.value(
                               ^^^^^^^
  ```
