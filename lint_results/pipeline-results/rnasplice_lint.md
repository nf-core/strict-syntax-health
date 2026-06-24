# Nextflow lint results

- Generated: 2026-06-24T00:38:33.757448368Z
- Nextflow version: 26.05.0-edge
- Summary: 35 warnings

## :warning: Warnings

- Warning: `conf/modules.config:305:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:314:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:323:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:332:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:354:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> null }
                        ^^^^^^^^
  ```

- Warning: `main.nf:239:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = RNASPLICE.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/misopy/index/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/misopy/index/main.nf:35:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `subworkflows/local/contrast_check/main.nf:26:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      contrasts = ch_contrasts                        // channel: [ val(contrast_map) ]
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/dexseq_deu/main.nf:55:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          DEXSEQ_COUNT.out.dexseq_clean_txt.map{ it[1] }.collect(),
                                                 ^^
  ```

- Warning: `subworkflows/local/dexseq_deu/main.nf:64:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      dexseq_clean_txt        = DEXSEQ_COUNT.out.dexseq_clean_txt.map{ it[1] }.collect()
                                                                       ^^
  ```

- Warning: `subworkflows/local/edger_deu/main.nf:42:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      featureCounts_summary = SUBREAD_FEATURECOUNTS.out.summary // path featureCounts.txt.summary
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:92:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      reads    = ch_final_reads   // channel: [ val(meta), [ files ] ]
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/tx2gene_tximport/main.nf:29:14`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          tar: it[0].tgz == true
               ^^
  ```

- Warning: `subworkflows/local/tx2gene_tximport/main.nf:30:14`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          dir: it[0].tgz == false
               ^^
  ```

- Warning: `subworkflows/local/tx2gene_tximport/main.nf:44:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      TXIMPORT ( salmon_results.collect{it[1]}, tx2gene )
                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnasplice_pipeline/main.nf:411:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, fastq -> meta.single_end }
                       ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnasplice_pipeline/main.nf:415:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (it.size() > 1) {
                  ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnasplice_pipeline/main.nf:426:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, fastq -> meta.strandedness }
                       ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnasplice_pipeline/main.nf:430:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (it.size() > 1) {
                  ^^
  ```

- Warning: `subworkflows/local/visualize_miso/main.nf:63:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_bams = ch_genome_bam.collect({it[1]})
                                       ^^
  ```

- Warning: `subworkflows/local/visualize_miso/main.nf:64:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_miso_run = MISO_RUN.out.miso.map{it[1]}.collect()
                                          ^^
  ```

- Warning: `subworkflows/local/visualize_miso/main.nf:77:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def miso_genes_list = miso_genes ? miso_genes.split(',').collect{ it.trim() } : [""]
                                                                        ^^
  ```

- Warning: `subworkflows/local/visualize_miso/main.nf:95:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it[1], it[2] ] }
                  ^^
  ```

- Warning: `subworkflows/local/visualize_miso/main.nf:95:24`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it[1], it[2] ] }
                         ^^
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

- Warning: `workflows/rnasplice.nf:71:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      multiqc_config // parameter value pass-through
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/rnasplice.nf:72:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      multiqc_logo // parameter value pass-through
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/rnasplice.nf:73:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      multiqc_methods_description // parameter value pass-through
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/rnasplice.nf:135:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .flatMap { it }
                     ^^
  ```

- Warning: `workflows/rnasplice.nf:136:16`: Variable was declared but not used

  ```nextflow
          .set { ch_contrasts }
                 ^^^^^^^^^^^^
  ```

- Warning: `workflows/rnasplice.nf:227:9`: Variable was declared but not used

  ```nextflow
          ch_transcriptome_bam_index = BAM_SORT_STATS_SAMTOOLS.out.index
          ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/rnasplice.nf:588:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = MULTIQC.out.report.map { _meta, report -> [report] }.toList()
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
