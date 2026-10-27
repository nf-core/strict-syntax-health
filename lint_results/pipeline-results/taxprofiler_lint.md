# Nextflow lint results

- Generated: 2026-10-27T00:23:57.337399515Z
- Nextflow version: 26.10.3
- Summary: 122 warnings

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

- Warning: `conf/modules.config:653:99`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { !params.bracken_save_intermediatekraken2 && meta.tool == "bracken" ? null : it },
                                                                                                    ^^
  ```

- Warning: `modules/local/kraken2standardreport/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/kronacleanup/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/adapterremoval/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bbmap/bbduk/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bowtie2/align/main.nf:29:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bowtie2/build/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bracken/bracken/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bracken/combinebrackenoutputs/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/cat/fastq/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/centrifuge/centrifuge/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/centrifuge/kreport/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/centrifuger/centrifuger/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/centrifuger/quantification/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/deacon/filter/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/deacon/index/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/diamond/blastx/main.nf:27:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/falco/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fastp/main.nf:26:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fastqc/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/filtlong/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/ganon/classify/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/ganon/report/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/ganon/table/main.nf:16:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hostile/clean/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hostile/fetch/main.nf:16:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/kaiju/kaiju/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/kaiju/kaiju2krona/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/kaiju/kaiju2table/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/kmcp/profile/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/kmcp/profile/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kmcp/search/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
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

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/krakentools/combinekreports/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/krakentools/kreport2krona/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/krakenuniq/preloadedkrakenuniq/main.nf:26:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/krakenuniq/preloadedkrakenuniq/main.nf:112:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def prefix_list = prefixes.collect { "'${it}'" }.join(' ')
                                               ^^
  ```

- Warning: `modules/nf-core/krona/ktimporttaxonomy/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/krona/ktimporttext/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/malt/run/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/megan/rma2info/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/melon/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/metacache/query/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/metaphlan/mergemetaphlantables/main.nf:16:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/metaphlan/metaphlan/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/minimap2/index/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/motus/merge/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/motus/preplong/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/motus/profile/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/nanoq/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/nonpareil/curve/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/nonpareil/nonpareil/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/nonpareil/nonpareilcurvesr/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/nonpareil/set/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/porechop/abi/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
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

- Warning: `modules/nf-core/porechop/porechop/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/prinseqplusplus/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/fastq/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/index/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/stats/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/view/main.nf:28:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/sylph/profile/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/sylphtax/merge/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/sylphtax/taxprof/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/taxpasta/merge/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/taxpasta/standardise/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/untar/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/local/longread_hostremoval/main.nf:26:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          DEACON_INDEX( Channel.value([[id: ch_reference.baseName], ch_reference]) )
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:248:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  if (it[0].is_fasta) {
                      ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:249:145`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      log.warn("[nf-core/taxprofiler] Centrifuge currently does not accept FASTA files as input. Skipping Centrifuge for sample ${it[0].id}.")
                                                                                                                                                  ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:251:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  !it[0].is_fasta
                   ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:293:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      if (it[0].is_fasta) {
                          ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:294:151`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          log.warn("[nf-core/taxprofiler] Centrifuger currently does not accept FASTA files as input. Skipping Centrifuger for sample ${it[0].id}.")
                                                                                                                                                        ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:296:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      !it[0].is_fasta
                       ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:381:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  if (it[0].is_fasta) {
                      ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:382:135`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      log.warn("[nf-core/taxprofiler] mOTUs currently does not accept FASTA files as input. Skipping mOTUs for sample ${it[0].id}.")
                                                                                                                                        ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:384:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  !it[0].is_fasta
                   ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:387:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  longread: it[0].instrument_platform == 'OXFORD_NANOPORE' || it[0].instrument_platform == 'PACBIO_SMRT'
                            ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:387:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  longread: it[0].instrument_platform == 'OXFORD_NANOPORE' || it[0].instrument_platform == 'PACBIO_SMRT'
                                                                              ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:388:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  shortread: it[0].instrument_platform != 'OXFORD_NANOPORE' && it[0].instrument_platform != 'PACBIO_SMRT'
                             ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:388:78`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  shortread: it[0].instrument_platform != 'OXFORD_NANOPORE' && it[0].instrument_platform != 'PACBIO_SMRT'
                                                                               ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:574:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  if (it[0].is_fasta) {
                      ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:575:135`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      log.warn("[nf-core/taxprofiler] sylph currently does not accept FASTA files as input. Skipping sylph for sample ${it[0].id}.")
                                                                                                                                        ^^
  ```

- Warning: `subworkflows/local/profiling/main.nf:577:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

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

- Warning: `subworkflows/local/shortread_hostremoval/main.nf:26:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          DEACON_INDEX( Channel.value([[id: ch_reference.baseName], ch_reference]) )
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/shortread_hostremoval/main.nf:30:46`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_hostremoval_index = BOWTIE2_BUILD(Channel.value([[id: ch_reference.baseName], ch_reference])).index
                                               ^^^^^^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:27:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          centrifuge: it[0]['tool'] == 'centrifuge'
                      ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:28:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          centrifuger: it[0]['tool'] == 'centrifuger'
                       ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:29:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          kraken2: it[0]['tool'] == 'kraken2' || it[0]['tool'] == 'kraken2-bracken'
                   ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:29:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          kraken2: it[0]['tool'] == 'kraken2' || it[0]['tool'] == 'kraken2-bracken'
                                                 ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:33:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          kaiju: it[0]['tool'] == 'kaiju'
                 ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:34:15`: Implicit closure parameter is deprecated, declare an explicit parameter instead

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

- Warning: `subworkflows/local/visualization_krona/main.nf:85:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { [[id: it[0]['db_name'], tool: it[0]['tool']], it[1]] }
                           ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:85:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { [[id: it[0]['db_name'], tool: it[0]['tool']], it[1]] }
                                                   ^^
  ```

- Warning: `subworkflows/local/visualization_krona/main.nf:85:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { [[id: it[0]['db_name'], tool: it[0]['tool']], it[1]] }
                                                                   ^^
  ```
