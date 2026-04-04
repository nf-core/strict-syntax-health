# Nextflow lint results

- Generated: 2026-04-04T00:24:53.551427685Z
- Nextflow version: 26.03.1-edge
- Summary: 99 warnings

## :warning: Warnings

- Warning: `conf/modules.config:94:273`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && !params.perform_shortread_hostremoval && !params.perform_shortread_complexityfilter && params.perform_shortread_qc && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                                                                  ^^
  ```

- Warning: `conf/modules.config:127:273`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && !params.perform_shortread_hostremoval && !params.perform_shortread_complexityfilter && params.perform_shortread_qc && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                                                                  ^^
  ```

- Warning: `conf/modules.config:155:273`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && !params.perform_shortread_hostremoval && !params.perform_shortread_complexityfilter && params.perform_shortread_qc && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                                                                  ^^
  ```

- Warning: `conf/modules.config:185:308`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && !params.perform_shortread_hostremoval && !params.perform_shortread_complexityfilter && params.perform_shortread_qc && !params.shortread_qc_mergepairs && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                                                                                                     ^^
  ```

- Warning: `conf/modules.config:236:273`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && !params.perform_shortread_hostremoval && !params.perform_shortread_complexityfilter && params.perform_shortread_qc && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                                                                  ^^
  ```

- Warning: `conf/modules.config:260:304`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && !params.perform_longread_hostremoval && params.longread_qc_skipqualityfilter && !params.longread_qc_skipadaptertrim && params.perform_longread_qc && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                                                                                                 ^^
  ```

- Warning: `conf/modules.config:289:304`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && !params.perform_longread_hostremoval && params.longread_qc_skipqualityfilter && !params.longread_qc_skipadaptertrim && params.perform_longread_qc && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                                                                                                 ^^
  ```

- Warning: `conf/modules.config:318:266`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && !params.perform_longread_hostremoval && !params.longread_qc_skipqualityfilter && params.perform_longread_qc && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                                                           ^^
  ```

- Warning: `conf/modules.config:347:266`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && !params.perform_longread_hostremoval && !params.longread_qc_skipqualityfilter && params.perform_longread_qc && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                                                           ^^
  ```

- Warning: `conf/modules.config:376:238`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && !params.perform_shortread_hostremoval && params.shortread_complexityfilter_tool && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                               ^^
  ```

- Warning: `conf/modules.config:404:238`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && !params.perform_shortread_hostremoval && params.shortread_complexityfilter_tool && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                               ^^
  ```

- Warning: `conf/modules.config:447:195`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && params.perform_shortread_hostremoval && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                    ^^
  ```

- Warning: `conf/modules.config:507:194`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && params.perform_longread_hostremoval && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                   ^^
  ```

- Warning: `conf/modules.config:569:99`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { !params.bracken_save_intermediatekraken2 && meta.tool == "bracken" ? null : it },
                                                                                                    ^^
  ```

- Warning: `modules/nf-core/bbmap/bbduk/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/bracken/bracken/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/bracken/combinebrackenoutputs/main.nf:39:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/cat/fastq/main.nf:22:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def readList = reads instanceof List ? reads.collect { it.toString() } : [reads.toString()]
                                                             ^^
  ```

- Warning: `modules/nf-core/cat/fastq/main.nf:58:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def readList = reads instanceof List ? reads.collect { it.toString() } : [reads.toString()]
                                                             ^^
  ```

- Warning: `modules/nf-core/ganon/classify/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/ganon/classify/main.nf:50:9`: Variable was declared but not used

  ```nextflow
      def input = meta.single_end ? "--single-reads ${fastqs}" : "--paired-reads ${fastqs}"
          ^^^^^
  ```

- Warning: `modules/nf-core/ganon/report/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/ganon/table/main.nf:36:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kaiju/kaiju/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kaiju/kaiju/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def input = meta.single_end ? "-i ${reads}" : "-i ${reads[0]} -j ${reads[1]}"
          ^^^^^
  ```

- Warning: `modules/nf-core/kaiju/kaiju2krona/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kaiju/kaiju2table/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kmcp/profile/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kmcp/search/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def input  = meta.single_end ? "${reads}": "-1 ${reads[0]} -2 ${reads[1]}"
          ^^^^^
  ```

- Warning: `modules/nf-core/kmcp/search/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:60:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:62:9`: Variable was declared but not used

  ```nextflow
      def paired       = meta.single_end ? "" : "--paired"
          ^^^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:65:9`: Variable was declared but not used

  ```nextflow
      def readclassification_option = save_reads_assignment ? "--output ${prefix}.kraken2.classifiedreads.txt" : "--output /dev/null"
          ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:66:9`: Variable was declared but not used

  ```nextflow
      def compress_reads_command = save_output_fastqs ? "pigz -p $task.cpus *.fastq" : ""
          ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/krakentools/combinekreports/main.nf:36:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/krakentools/kreport2krona/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/malt/run/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/megan/rma2info/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/megan/rma2info/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def summary = megan_summary ? "-es ${prefix}.megan" : ""
          ^^^^^^^
  ```

- Warning: `modules/nf-core/melon/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/metacache/query/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/metacache/query/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def input_file = meta.single_end ? reads : "${reads[0]} ${reads[1]} -pairfiles"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/metaphlan/mergemetaphlantables/main.nf:35:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/metaphlan/metaphlan/main.nf:58:9`: Variable was declared but not used

  ```nextflow
      def input_data = ("${input_type}".contains("fastq")) && !meta.single_end ? "${input[0]},${input[1]}" : "${input}"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/metaphlan/metaphlan/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def bowtie2_out = "${input_type}" == "--input_type bowtie2out" || "${input_type}" == "--input_type sam" ? '' : "--bowtie2out ${prefix}.bowtie2out.txt"
          ^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/metaphlan/metaphlan/main.nf:60:9`: Variable was declared but not used

  ```nextflow
      def samfile_out = save_samfile ? "-s ${prefix}.sam" : ''
          ^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:67:9`: Variable was declared but not used

  ```nextflow
      def target = reference ?: (bam_input ? error("BAM input requires reference") : reads)
          ^^^^^^
  ```

- Warning: `modules/nf-core/motus/merge/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/motus/merge/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def cmd_input = input.size() > 1 ? "-i ${input.join(',')}" : input.isDirectory() ? "-d ${input}" : "-i ${input}"
          ^^^^^^^^^
  ```

- Warning: `modules/nf-core/motus/merge/main.nf:50:9`: Variable was declared but not used

  ```nextflow
      def suffix = task.ext.args?.contains("-B") ? "biom" : "txt"
          ^^^^^^
  ```

- Warning: `modules/nf-core/motus/preplong/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def refdb = db ? "-db ${db}" : ""
          ^^^^^
  ```

- Warning: `modules/nf-core/motus/profile/main.nf:58:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/motus/profile/main.nf:60:9`: Variable was declared but not used

  ```nextflow
      def inputs = reads[0].getExtension() == 'bam' ?
          ^^^^^^
  ```

- Warning: `modules/nf-core/motus/profile/main.nf:65:9`: Variable was declared but not used

  ```nextflow
      def refdb = db ? "-db ${db}" : ""
          ^^^^^
  ```

- Warning: `modules/nf-core/nanoq/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/nonpareil/curve/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/nonpareil/nonpareil/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/nonpareil/nonpareilcurvesr/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/nonpareil/set/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/porechop/abi/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/porechop/abi/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def adapters_list = custom_adapters ? "--custom_adapters ${custom_adapters}" : ""
          ^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/sylph/profile/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/sylph/profile/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def input = meta.single_end ? "${reads}" : "-1 ${reads[0]} -2 ${reads[1]}"
          ^^^^^
  ```

- Warning: `modules/nf-core/sylphtax/merge/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/taxpasta/merge/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/taxpasta/merge/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def taxonomy_option = taxonomy ? "--taxonomy ${taxonomy}" : ''
          ^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/taxpasta/merge/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def samplesheet_input = samplesheet ? "-s ${samplesheet}" : ''
          ^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/taxpasta/standardise/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/taxpasta/standardise/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def taxonomy_option = taxonomy ? "--taxonomy ${taxonomy}" : ''
          ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:247:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  if (it[0].is_fasta) {
                      ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:248:145`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      log.warn("[nf-core/taxprofiler] Centrifuge currently does not accept FASTA files as input. Skipping Centrifuge for sample ${it[0].id}.")
                                                                                                                                                  ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:250:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  !it[0].is_fasta
                   ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:335:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  if (it[0].is_fasta) {
                      ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:336:135`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      log.warn("[nf-core/taxprofiler] mOTUs currently does not accept FASTA files as input. Skipping mOTUs for sample ${it[0].id}.")
                                                                                                                                        ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:338:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  !it[0].is_fasta
                   ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:341:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  longread: it[0].instrument_platform == 'OXFORD_NANOPORE' || it[0].instrument_platform == 'PACBIO_SMRT'
                            ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:341:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  longread: it[0].instrument_platform == 'OXFORD_NANOPORE' || it[0].instrument_platform == 'PACBIO_SMRT'
                                                                              ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:342:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  shortread: it[0].instrument_platform != 'OXFORD_NANOPORE' && it[0].instrument_platform != 'PACBIO_SMRT'
                             ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:342:78`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  shortread: it[0].instrument_platform != 'OXFORD_NANOPORE' && it[0].instrument_platform != 'PACBIO_SMRT'
                                                                               ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:534:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  if (it[0].is_fasta) {
                      ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:535:135`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      log.warn("[nf-core/taxprofiler] sylph currently does not accept FASTA files as input. Skipping sylph for sample ${it[0].id}.")
                                                                                                                                        ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:537:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  !it[0].is_fasta
                   ^^
  ```

- Warning: `subworkflows/local/shortread_adapterremoval/main.nf:19:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          single: it[0].single_end
                  ^^
  ```

- Warning: `subworkflows/local/shortread_adapterremoval/main.nf:20:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          paired: !it[0].single_end
                   ^^
  ```

- Warning: `subworkflows/local/shortread_fastp/main.nf:18:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          single: it[0]['single_end'] == true
                  ^^
  ```

- Warning: `subworkflows/local/shortread_fastp/main.nf:19:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          paired: it[0]['single_end'] == false
                  ^^
  ```

- Warning: `subworkflows/local/standardisation_profiles/main.nf:232:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { key, meta, profile, db ->
                      ^^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:27:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          centrifuge: it[0]['tool'] == 'centrifuge'
                      ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:28:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          kraken2: it[0]['tool'] == 'kraken2' || it[0]['tool'] == 'kraken2-bracken'
                   ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:28:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          kraken2: it[0]['tool'] == 'kraken2' || it[0]['tool'] == 'kraken2-bracken'
                                                 ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:32:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          kaiju: it[0]['tool'] == 'kaiju'
                 ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:33:15`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          malt: it[0]['tool'] == 'malt'
                ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:72:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [[id: it[0]['db_name'], tool: it[0]['tool']], it[1]] }
                       ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:72:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [[id: it[0]['db_name'], tool: it[0]['tool']], it[1]] }
                                               ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:72:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [[id: it[0]['db_name'], tool: it[0]['tool']], it[1]] }
                                                               ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:86:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { [[id: it[0]['db_name'], tool: it[0]['tool']], it[1]] }
                           ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:86:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { [[id: it[0]['db_name'], tool: it[0]['tool']], it[1]] }
                                                   ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:86:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { [[id: it[0]['db_name'], tool: it[0]['tool']], it[1]] }
                                                                   ^^
  ```
