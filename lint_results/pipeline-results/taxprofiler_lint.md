# Nextflow lint results

- Generated: 2026-11-20T00:14:34.783589202Z
- Nextflow version: 26.11.0-edge
- Summary: 90 warnings

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

- Warning: `conf/modules.config:553:195`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && params.perform_shortread_hostremoval && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                    ^^
  ```

- Warning: `conf/modules.config:590:194`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && params.perform_longread_hostremoval && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                   ^^
  ```

- Warning: `conf/modules.config:621:236`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && (params.perform_shortread_hostremoval || params.perform_longread_hostremoval) && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                             ^^
  ```

- Warning: `conf/modules.config:675:99`: Implicit closure parameter is deprecated, declare an explicit parameter instead

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
