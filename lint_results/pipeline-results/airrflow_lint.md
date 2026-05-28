# Nextflow lint results

- Generated: 2026-05-28T00:35:30.945894364Z
- Nextflow version: 26.04.2
- Summary: 40 warnings

## :warning: Warnings

- Warning: `main.nf:237:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_custom_methods_description = params.multiqc_methods_description ? file(params.multiqc_methods_description, checkIfExists: true) : file("$projectDir/assets/methods_description_template.yml", checkIfExists: true)
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `main.nf:332:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = AIRRFLOW.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/cat/fastq/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/cat/fastq/main.nf:23:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def readList = reads instanceof List ? reads.collect{ it.toString() } : [reads.toString()]
                                                            ^^
  ```

- Warning: `modules/nf-core/cat/fastq/main.nf:54:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def readList = reads instanceof List ? reads.collect{ it.toString() } : [reads.toString()]
                                                            ^^
  ```

- Warning: `modules/nf-core/cellranger/vdj/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/trust4/main.nf:91:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/assembled_input_check.nf:32:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { get_meta(it) }
                          ^^
  ```

- Warning: `subworkflows/local/clonal_analysis.nf:50:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .splitText( limit:1 ) { it.trim().toString() }
                                      ^^
  ```

- Warning: `subworkflows/local/clonal_analysis.nf:62:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def valid = list.findAll { it != '' && it != 'NA' && it != 'NaN' }
                                             ^^
  ```

- Warning: `subworkflows/local/clonal_analysis.nf:62:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def valid = list.findAll { it != '' && it != 'NA' && it != 'NaN' }
                                                         ^^
  ```

- Warning: `subworkflows/local/clonal_analysis.nf:62:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def valid = list.findAll { it != '' && it != 'NA' && it != 'NaN' }
                                                                       ^^
  ```

- Warning: `subworkflows/local/clonal_analysis.nf:107:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map{ get_meta_tabs(it, genotypeby, cloneby) }
                                      ^^
  ```

- Warning: `subworkflows/local/fastq_input_check.nf:19:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/fastq_input_check.nf:24:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { create_fastq_channels(it, collapseby, cloneby, index_file) }
                                       ^^
  ```

- Warning: `subworkflows/local/novel_alleles_and_genotyping.nf:11:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_validated_samplesheet
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/novel_alleles_and_genotyping.nf:12:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_logo
      ^^^^^^^
  ```

- Warning: `subworkflows/local/novel_alleles_and_genotyping.nf:42:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .map{ get_meta_tabs(it) }
                                          ^^
  ```

- Warning: `subworkflows/local/presto_sans_umi.nf:229:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      fastp_reads_json = FASTP.out.json.collect{ meta,json -> json }
                                                 ^^^^
  ```

- Warning: `subworkflows/local/presto_sans_umi.nf:230:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      fastp_reads_html = FASTP.out.html.collect{ meta,html -> html }
                                                 ^^^^
  ```

- Warning: `subworkflows/local/presto_umi.nf:113:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                              .map{ id, meta1, R1, R2, meta2, index -> [ meta1, R1, R2, index ] }
                                                    ^^
  ```

- Warning: `subworkflows/local/presto_umi.nf:113:70`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                              .map{ id, meta1, R1, R2, meta2, index -> [ meta1, R1, R2, index ] }
                                                                       ^^^^^
  ```

- Warning: `subworkflows/local/presto_umi.nf:641:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      fastp_reads_json = FASTP.out.json.collect{ meta,json -> json }
                                                 ^^^^
  ```

- Warning: `subworkflows/local/presto_umi.nf:642:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      fastp_reads_html = FASTP.out.html.collect{ meta,html -> html }
                                                 ^^^^
  ```

- Warning: `subworkflows/local/repertoire_analysis_reporting.nf:88:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions = ch_versions
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/rnaseq_input.nf:33:5`: Variable was declared but not used

  ```nextflow
      ch_logs = channel.empty()
      ^^^^^^^
  ```

- Warning: `subworkflows/local/rnaseq_input.nf:113:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      return [ meta, out_files.find { it.endsWith("${meta.id}_airr.tsv") } ]
                                                      ^^
  ```

- Warning: `subworkflows/local/rnaseq_input.nf:115:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      return [ meta, out_files.find { it.endsWith("${meta.id}_barcode_airr.tsv") } ]
                                                      ^^
  ```

- Warning: `subworkflows/local/rnaseq_input.nf:138:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      fastp_reads_json = FASTP.out.json.collect{ meta,json -> json }
                                                 ^^^^
  ```

- Warning: `subworkflows/local/rnaseq_input.nf:139:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      fastp_reads_html = FASTP.out.html.collect{ meta,html -> html }
                                                 ^^^^
  ```

- Warning: `subworkflows/local/sc_raw_input.nf:25:5`: Variable was declared but not used

  ```nextflow
      ch_logs = channel.empty()
      ^^^^^^^
  ```

- Warning: `subworkflows/local/sc_raw_input.nf:79:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  [ meta, out_files.find { it.endsWith("airr_rearrangement.tsv") } ]
                                           ^^
  ```

- Warning: `subworkflows/local/sc_raw_input.nf:90:16`: Variable was declared but not used

  ```nextflow
          .set { ch_renamed_tsv }
                 ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/translate_embed.nf:56:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions = ch_versions
      ^^^^^^^^^^^^^^^^^^^^
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

- Warning: `workflows/airrflow.nf:171:17`: Variable was declared but not used

  ```nextflow
                  ch_cellranger_airr                      = SC_RAW_INPUT.out.airr
                  ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/airrflow.nf:172:17`: Variable was declared but not used

  ```nextflow
                  ch_cellranger_out                       = SC_RAW_INPUT.out.outs
                  ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/airrflow.nf:513:88`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(ch_fastqc_postassembly_mqc.collect{it[1]}.ifEmpty([]))
                                                                                         ^^
  ```
