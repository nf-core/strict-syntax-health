# Nextflow lint results

- Generated: 2026-07-17T00:32:33.022471694Z
- Nextflow version: 26.07.0-edge
- Summary: 303 warnings

## :warning: Warnings

- Warning: `conf/modules/aligner.config:51:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      ) { "mapped/${meta.id}/${it}" }
                                               ^^
  ```

- Warning: `conf/modules/aligner.config:81:178`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { (params.save_output_as_bam && (params.save_mapped || params.skip_tools && params.skip_tools.split(',').contains('markduplicates'))) ? "mapped/${meta.id}/${it}" : null }
                                                                                                                                                                                   ^^
  ```

- Warning: `conf/modules/aligner_parabricks.config:31:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_mapped ? it : null }
                                             ^^
  ```

- Warning: `conf/modules/aligner_parabricks.config:41:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_mapped ? it : null }
                                             ^^
  ```

- Warning: `conf/modules/aligner_parabricks.config:50:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_mapped ? it : null }
                                             ^^
  ```

- Warning: `conf/modules/aligner_parabricks.config:59:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_output_as_bam ? it : null }
                                                    ^^
  ```

- Warning: `conf/modules/annotate.config:27:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      saveAs: { params.tools.split(',').contains('snpeff') ? it : null }
                                                                             ^^
  ```

- Warning: `conf/modules/annotate.config:88:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_reference ? it : null }
                                                    ^^
  ```

- Warning: `conf/modules/annotate.config:126:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.tools.split(',').contains('snpeff') ? it : null }
                                                                         ^^
  ```

- Warning: `conf/modules/contamination.config:17:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_bbsplit_reads ? it : null }
                                                        ^^
  ```

- Warning: `conf/modules/deepvariant.config:29:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "deepvariant/${meta.id}/${it}" }
                                                                                  ^^
  ```

- Warning: `conf/modules/freebayes.config:43:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "freebayes/${meta.id}/${it}" }
                                                                                ^^
  ```

- Warning: `conf/modules/haplotypecaller.config:29:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "haplotypecaller/${meta.id}/${it}" }
                                                                                      ^^
  ```

- Warning: `conf/modules/lofreq.config:26:80`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { meta.num_intervals > 1 ? null : "lofreq/${meta.id}/${it}" }
                                                                                 ^^
  ```

- Warning: `conf/modules/markduplicates.config:42:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { !params.save_output_as_bam ? it : null }
                                                     ^^
  ```

- Warning: `conf/modules/markduplicates.config:74:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { !params.save_output_as_bam ? it : null }
                                                         ^^
  ```

- Warning: `conf/modules/markduplicates.config:82:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_output_as_bam ? (it.endsWith('.md.bai') ? it.replace('.md.bai', '.md.bam.bai') : it) : null }
                                                         ^^
  ```

- Warning: `conf/modules/markduplicates.config:82:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_output_as_bam ? (it.endsWith('.md.bai') ? it.replace('.md.bai', '.md.bam.bai') : it) : null }
                                                                                  ^^
  ```

- Warning: `conf/modules/markduplicates.config:82:120`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_output_as_bam ? (it.endsWith('.md.bai') ? it.replace('.md.bai', '.md.bam.bai') : it) : null }
                                                                                                                         ^^
  ```

- Warning: `conf/modules/markduplicates.config:88:145`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { !(params.skip_tools && params.skip_tools.split(',').contains('markduplicates_report')) ? "markduplicates/${meta.id}/${it}" : null}
                                                                                                                                                  ^^
  ```

- Warning: `conf/modules/markduplicates.config:102:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { !params.save_output_as_bam ? it : null }
                                                         ^^
  ```

- Warning: `conf/modules/markduplicates.config:108:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_output_as_bam ? it : null }
                                                        ^^
  ```

- Warning: `conf/modules/markduplicates.config:119:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { !params.save_output_as_bam ? it : null }
                                                         ^^
  ```

- Warning: `conf/modules/markduplicates.config:125:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_output_as_bam ? it : null }
                                                        ^^
  ```

- Warning: `conf/modules/mpileup.config:33:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : it }
                                                        ^^
  ```

- Warning: `conf/modules/mutect2.config:26:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { meta.num_intervals > 1 ? null : "mutect2/${meta.id}/${it}" }
                                                                                  ^^
  ```

- Warning: `conf/modules/mutect2.config:98:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { meta.num_intervals > 1 ? null : "mutect2/${meta.id}/${it}" }
                                                                                  ^^
  ```

- Warning: `conf/modules/prepare_genome.config:21:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:31:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:40:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:50:84`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? "cnvkit/${it}" : null }
                                                                                     ^^
  ```

- Warning: `conf/modules/prepare_genome.config:61:84`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? "cnvkit/${it}" : null }
                                                                                     ^^
  ```

- Warning: `conf/modules/prepare_genome.config:70:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:79:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:88:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:97:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:106:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:115:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:124:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:133:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:142:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:151:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:160:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:175:78`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { (params.save_reference || params.build_only_index) && !it.equals('versions.yml') ? it : null }
                                                                               ^^
  ```

- Warning: `conf/modules/prepare_genome.config:175:106`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { (params.save_reference || params.build_only_index) && !it.equals('versions.yml') ? it : null }
                                                                                                           ^^
  ```

- Warning: `conf/modules/prepare_genome.config:186:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? it : null }
                                                                           ^^
  ```

- Warning: `conf/modules/prepare_intervals.config:28:87`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? "intervals/${it}" : null }
                                                                                        ^^
  ```

- Warning: `conf/modules/prepare_intervals.config:37:87`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? "intervals/${it}" : null }
                                                                                        ^^
  ```

- Warning: `conf/modules/prepare_intervals.config:47:87`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_reference || params.build_only_index ? "intervals/${it}" : null }
                                                                                        ^^
  ```

- Warning: `conf/modules/prepare_recalibration.config:25:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "recal_table/${meta.id}/${it}" }
                                                                                  ^^
  ```

- Warning: `conf/modules/recalibrate.config:28:111`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { !params.save_output_as_bam ? meta.num_intervals > 1 ? null : "recalibrated/${meta.id}/${it}" : null }
                                                                                                                ^^
  ```

- Warning: `conf/modules/recalibrate.config:34:110`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_output_as_bam ? meta.num_intervals > 1 ? null : "recalibrated/${meta.id}/${it}" : null }
                                                                                                               ^^
  ```

- Warning: `conf/modules/recalibrate.config:40:110`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_output_as_bam ? meta.num_intervals > 1 ? null : "recalibrated/${meta.id}/${it.replace('.bai', '.bam.bai')}" : null }
                                                                                                               ^^
  ```

- Warning: `conf/modules/recalibrate.config:50:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { !params.save_output_as_bam ? it : null }
                                                     ^^
  ```

- Warning: `conf/modules/recalibrate.config:59:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { !params.save_output_as_bam ? it : null }
                                                     ^^
  ```

- Warning: `conf/modules/recalibrate.config:69:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { params.save_output_as_bam ? it : null }
                                                    ^^
  ```

- Warning: `conf/modules/recalibrate.config:79:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { (params.save_output_as_bam && meta.num_intervals > 1) ? it : null }
                                                                                ^^
  ```

- Warning: `conf/modules/sentieon_dedup.config:35:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { !params.save_output_as_bam ? it : null }
                                                         ^^
  ```

- Warning: `conf/modules/sentieon_dedup.config:41:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { params.save_output_as_bam ? it : null }
                                                        ^^
  ```

- Warning: `conf/modules/sentieon_dedup.config:47:145`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { !(params.skip_tools && params.skip_tools.split(',').contains('sentieon_dedup_report')) ? "sentieon_dedup/${meta.id}/${it}" : null}
                                                                                                                                                  ^^
  ```

- Warning: `conf/modules/sentieon_dnascope.config:25:87`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "sentieon_dnascope/${meta.id}/${it}" }
                                                                                        ^^
  ```

- Warning: `conf/modules/sentieon_haplotyper.config:25:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "sentieon_haplotyper/${meta.id}/${it}" }
                                                                                          ^^
  ```

- Warning: `conf/modules/sentieon_tnscope.config:28:86`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "sentieon_tnscope/${meta.id}/${it}" }
                                                                                       ^^
  ```

- Warning: `conf/modules/strelka.config:26:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : "strelka/${meta.id}/${it}" }
                                                                              ^^
  ```

- Warning: `modules/local/consensus_from_sites/main.nf:27:9`: Variable was declared but not used

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

- Warning: `modules/nf-core/cnvkit/batch/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def tumor_bam = tumor_exists && tumor.Extension == "bam" ? true : false
          ^^^^^^^^^
  ```

- Warning: `modules/nf-core/cnvkit/batch/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def normal_bam = normal_exists && normal.Extension == "bam" ? true : false
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/fgbio/fastqtobam/main.nf:58:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/gatk4/baserecalibrator/main.nf:29:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def sites_command = known_sites.collect{"--known-sites $it"}.join(' ')
                                                             ^^
  ```

- Warning: `modules/nf-core/gatk4/estimatelibrarycomplexity/main.nf:26:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = input.collect(){"--INPUT $it"}.join(" ")
                                                ^^
  ```

- Warning: `modules/nf-core/gatk4/filtermutectcalls/main.nf:29:113`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def orientationbias_command = orientationbias ? orientationbias.collect{"--orientation-bias-artifact-priors $it"}.join(' ') : ''
                                                                                                                  ^^
  ```

- Warning: `modules/nf-core/gatk4/filtermutectcalls/main.nf:30:96`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def segmentation_command    = segmentation    ? segmentation.collect{"--tumor-segmentation $it"}.join(' ')                  : ''
                                                                                                 ^^
  ```

- Warning: `modules/nf-core/gatk4/filtermutectcalls/main.nf:32:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def table_command           = table           ? table.collect{"--contamination-table $it"}.join(' ')                        : ''
                                                                                           ^^
  ```

- Warning: `modules/nf-core/gatk4/filtervarianttranches/main.nf:30:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def resource_list = resources.collect{"--resource $it"}.join(' ')
                                                        ^^
  ```

- Warning: `modules/nf-core/gatk4/gatherbqsrreports/main.nf:23:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = table.collect{"--input $it"}.join(' ')
                                              ^^
  ```

- Warning: `modules/nf-core/gatk4/gatherpileupsummaries/main.nf:25:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = pileup.collect{ "--I $it" }.join(' ')
                                            ^^
  ```

- Warning: `modules/nf-core/gatk4/genomicsdbimport/main.nf:30:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      input_command = input_map ? "--sample-name-map ${vcf[0]}" : vcf.collect(){"--variant $it"}.join(' ')
                                                                                           ^^
  ```

- Warning: `modules/nf-core/gatk4/learnreadorientationmodel/main.nf:23:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = f1r2.collect{"--input $it"}.join(' ')
                                             ^^
  ```

- Warning: `modules/nf-core/gatk4/markduplicates/main.nf:33:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = bam.collect { "--INPUT ${it}" }.join(' ')
                                                ^^
  ```

- Warning: `modules/nf-core/gatk4/mergemutectstats/main.nf:23:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = stats.collect{ "--stats ${it}"}.join(' ')
                                                 ^^
  ```

- Warning: `modules/nf-core/gatk4/mutect2/main.nf:33:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def inputs = input.collect{ "--input $it"}.join(" ")
                                           ^^
  ```

- Warning: `modules/nf-core/gatk4spark/baserecalibrator/main.nf:29:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def sites_command = known_sites.collect { "--known-sites ${it}" }.join(' ')
                                                                 ^^
  ```

- Warning: `modules/nf-core/gatk4spark/markduplicates/main.nf:28:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = bam.collect { "--input ${it}" }.join(' ')
                                                ^^
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

- Warning: `modules/nf-core/goleft/indexcov/main.nf:31:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_files = bams.findAll{it.name.endsWith(".bam")} + indexes.findAll{it.name.endsWith(".crai")}
                                     ^^
  ```

- Warning: `modules/nf-core/goleft/indexcov/main.nf:31:80`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_files = bams.findAll{it.name.endsWith(".bam")} + indexes.findAll{it.name.endsWith(".crai")}
                                                                                 ^^
  ```

- Warning: `modules/nf-core/goleft/indexcov/main.nf:32:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def extranormalize = input_files.any{it.name.endsWith(".crai")} ? " --extranormalize " : ""
                                           ^^
  ```

- Warning: `modules/nf-core/goleft/indexcov/main.nf:52:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/lofreq/callparallel/main.nf:29:9`: Variable was declared but not used

  ```nextflow
      def alignment_bam = bam.Extension == "bam" ? true : false
          ^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/manta/germline/main.nf:33:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_files = input.collect{"--bam ${it}"}.join(' ')
                                               ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:38:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def pairs = vcfs.indices.collect { [vcfs[it], input_priority[it]] }
                                                      ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:38:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def pairs = vcfs.indices.collect { [vcfs[it], input_priority[it]] }
                                                                          ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:40:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              vcfs = pairs.collect { it[0] }
                                     ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:41:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              priority = pairs.collect { it[1] }
                                         ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:55:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          input = (vcfs.collect().size() > 1 && sort_inputs) ? vcfs.sort { it.name } : vcfs
                                                                           ^^
  ```

- Warning: `modules/nf-core/unzip/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:97:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--bed') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:98:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--exclude-bed') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:99:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--hapcount') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:100:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--positions') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:101:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--exclude-positions') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:106:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--diff') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:107:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--gzdiff') }
                           ^^
  ```

- Warning: `modules/nf-core/vcftools/main.nf:108:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      args_list.removeIf { it.contains('--diff-bcf') }
                           ^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator/main.nf:41:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          single:   it[0].num_intervals <= 1
                    ^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator/main.nf:42:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          multiple: it[0].num_intervals > 1
                    ^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator_spark/main.nf:29:60`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4SPARK_BASERECALIBRATOR(cram_intervals, fasta.map{ meta, it -> [ it ] }, fasta_fai.map{ meta, it -> [ it ] }, dict.map{ meta, it -> [ it ] }, known_sites, known_sites_tbi)
                                                             ^^^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator_spark/main.nf:29:97`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4SPARK_BASERECALIBRATOR(cram_intervals, fasta.map{ meta, it -> [ it ] }, fasta_fai.map{ meta, it -> [ it ] }, dict.map{ meta, it -> [ it ] }, known_sites, known_sites_tbi)
                                                                                                  ^^^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator_spark/main.nf:29:129`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4SPARK_BASERECALIBRATOR(cram_intervals, fasta.map{ meta, it -> [ it ] }, fasta_fai.map{ meta, it -> [ it ] }, dict.map{ meta, it -> [ it ] }, known_sites, known_sites_tbi)
                                                                                                                                  ^^^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator_spark/main.nf:34:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          single:   it[0].num_intervals <= 1
                    ^^
  ```

- Warning: `subworkflows/local/bam_baserecalibrator_spark/main.nf:35:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          multiple: it[0].num_intervals > 1
                    ^^
  ```

- Warning: `subworkflows/local/bam_markduplicates/main.nf:24:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4_MARKDUPLICATES(bam, fasta.map{ meta, fasta_ -> [ fasta_ ] }, fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] })
                                           ^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates/main.nf:24:87`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4_MARKDUPLICATES(bam, fasta.map{ meta, fasta_ -> [ fasta_ ] }, fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] })
                                                                                        ^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates_spark/main.nf:25:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4SPARK_MARKDUPLICATES(bam, fasta.map{ meta, fasta_ -> [ fasta_ ] }, fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] }, dict.map{ meta, dict_ -> [ dict_ ] })
                                                ^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates_spark/main.nf:25:92`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4SPARK_MARKDUPLICATES(bam, fasta.map{ meta, fasta_ -> [ fasta_ ] }, fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] }, dict.map{ meta, dict_ -> [ dict_ ] })
                                                                                             ^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates_spark/main.nf:25:140`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4SPARK_MARKDUPLICATES(bam, fasta.map{ meta, fasta_ -> [ fasta_ ] }, fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] }, dict.map{ meta, dict_ -> [ dict_ ] })
                                                                                                                                             ^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates_spark/main.nf:38:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4_ESTIMATELIBRARYCOMPLEXITY(bam, fasta.map{ meta, fasta_ -> [ fasta_ ] }, fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] }, dict.map{ meta, dict_ -> [ dict_ ] })
                                                      ^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates_spark/main.nf:38:98`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4_ESTIMATELIBRARYCOMPLEXITY(bam, fasta.map{ meta, fasta_ -> [ fasta_ ] }, fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] }, dict.map{ meta, dict_ -> [ dict_ ] })
                                                                                                   ^^^^
  ```

- Warning: `subworkflows/local/bam_markduplicates_spark/main.nf:38:146`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      GATK4_ESTIMATELIBRARYCOMPLEXITY(bam, fasta.map{ meta, fasta_ -> [ fasta_ ] }, fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] }, dict.map{ meta, dict_ -> [ dict_ ] })
                                                                                                                                                   ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:32:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:33:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:39:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:40:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:53:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_deepvariant/main.nf:54:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_freebayes/main.nf:37:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_freebayes/main.nf:38:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:26:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      bam                               // channel: [mandatory] meta, bam
      ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:99:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              cram.map{ meta, cram_, crai -> [ meta, [], cram_ ] },
                                     ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:181:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      fasta.map{ meta, fasta_ -> [ fasta_ ] },
                                 ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:182:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] },
                                     ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:183:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      dict.map{ meta, dict_ -> [ dict_ ] },
                                ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:243:9`: Variable was declared but not used

  ```nextflow
          gvcf_tbi_sentieon_dnascope = BAM_VARIANT_CALLING_SENTIEON_DNASCOPE.out.gvcf_tbi
          ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:301:9`: Variable was declared but not used

  ```nextflow
          gvcf_tbi_sentieon_haplotyper = BAM_VARIANT_CALLING_SENTIEON_HAPLOTYPER.out.gvcf_tbi
          ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:330:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      fasta.map{ meta, it -> [ it ] },
                                 ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:331:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      fasta_fai.map{ meta, it -> [ it ] },
                                     ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:332:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      dict.map{ meta, dict_ -> [ dict_ ] },
                                ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:352:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              fasta.map{ meta, fasta_ -> [ fasta_ ] },
                         ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_all/main.nf:353:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              fasta_fai.map{ meta, fasta_fai_ -> [ fasta_fai_ ] },
                             ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_manta/main.nf:30:5`: Variable was declared but not used

  ```nextflow
      small_indels_vcf     = MANTA_GERMLINE.out.candidate_small_indels_vcf
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_germline_manta/main.nf:31:5`: Variable was declared but not used

  ```nextflow
      sv_vcf               = MANTA_GERMLINE.out.candidate_sv_vcf
      ^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:45:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, gvcf, tbi, _cram, _crai, intervals_, dragstr_model -> [ meta, gvcf, tbi, intervals_ ] }
                                                           ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:53:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:54:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:62:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:63:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:71:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_haplotypecaller/main.nf:72:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_indexcov/main.nf:30:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      indexcov_input_ch = reindex_ch.output.map{[[id:"indexcov"], it[1], it[2]]}.groupTuple()
                                                                  ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_indexcov/main.nf:30:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      indexcov_input_ch = reindex_ch.output.map{[[id:"indexcov"], it[1], it[2]]}.groupTuple()
                                                                         ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_mpileup/main.nf:42:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_mpileup/main.nf:43:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_mpileup/main.nf:48:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_mpileup/main.nf:49:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_mpileup/main.nf:54:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_mpileup/main.nf:55:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:19:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      dbsnp_vqsr                        // channel: [optional]
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:60:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          emit_mode_items.any{ it.equals('gvcf') })
                               ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:76:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:77:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:84:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:85:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:92:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:93:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:100:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_dnascope/main.nf:101:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:19:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      dbsnp_vqsr                     // channel: [optional]
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:56:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          emit_mode_items.any{ it.equals('gvcf') })
                               ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:72:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:73:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:80:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:81:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:88:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:89:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:96:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              intervals:    it[0].num_intervals > 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sentieon_haplotyper/main.nf:97:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_intervals: it[0].num_intervals <= 1
                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:32:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:33:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:39:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:40:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:46:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_strelka/main.nf:47:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_tiddit/main.nf:24:62`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      vcf = TABIX_BGZIP_TIDDIT_SV.out.gz_index.map { meta, gz, tbi -> [meta + [variantcaller: 'tiddit'], gz] }
                                                               ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_single_tiddit/main.nf:25:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      tbi = TABIX_BGZIP_TIDDIT_SV.out.gz_index.map { meta, gz, tbi -> [meta + [variantcaller: 'tiddit'], tbi] }
                                                           ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_controlfreec/main.nf:32:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def tumor_file = cnv instanceof List ? cnv.find { it.toString().endsWith("gz_CNVs") } : cnv //only find if its a list, else it returns only the filename without the path
                                                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_controlfreec/main.nf:41:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def tumor_file = ratio instanceof List ? ratio.find { it.toString().endsWith("gz_ratio.txt") } : ratio //same here as cnv
                                                                ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_manta/main.nf:31:5`: Variable was declared but not used

  ```nextflow
      candidate_sv_vcf = MANTA_SOMATIC.out.candidate_sv_vcf
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:35:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      germline_resource_pileup = germline_resource.filter { it != [] }
                                                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:36:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      germline_resource_pileup_tbi = germline_resource_tbi.filter { it != [] }
                                                                    ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:72:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:73:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:78:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:79:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:84:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:85:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:90:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:91:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:145:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:146:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:151:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:152:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:223:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .unique { it[0] }
                    ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_mutect2/main.nf:228:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .unique { it[0] }
                    ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:32:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:33:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:39:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:40:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:53:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:54:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:60:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_strelka/main.nf:61:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_tnscope/main.nf:43:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_tnscope/main.nf:44:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_tnscope/main.nf:49:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_somatic_tnscope/main.nf:50:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_all/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      intervals_bed_gz_tbi          // channel: [mandatory] [ interval.bed.gz, interval.bed.gz.tbi, num_intervals ] or [ [], [], 0 ] if no intervals
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_lofreq/main.nf:25:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_lofreq/main.nf:26:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_lofreq/main.nf:32:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_lofreq/main.nf:33:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_manta/main.nf:30:5`: Variable was declared but not used

  ```nextflow
      small_indels_vcf = MANTA_TUMORONLY.out.candidate_small_indels_vcf
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_manta/main.nf:31:5`: Variable was declared but not used

  ```nextflow
      candidate_sv_vcf = MANTA_TUMORONLY.out.candidate_sv_vcf
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:34:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      germline_resource_pileup = germline_resource.filter { it != [] }
                                                            ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:35:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      germline_resource_pileup_tbi = germline_resource_tbi.filter { it != [] }
                                                                    ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:62:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:63:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:68:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:69:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:74:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:75:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:80:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:81:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:109:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals: it[0].num_intervals > 1
                     ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:110:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:160:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .unique { it[0] }
                    ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_mutect2/main.nf:165:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .unique { it[0] }
                    ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_tnscope/main.nf:43:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_tnscope/main.nf:44:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_tnscope/main.nf:49:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          intervals:    it[0].num_intervals > 1
                        ^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_tumor_only_tnscope/main.nf:50:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          no_intervals: it[0].num_intervals <= 1
                        ^^
  ```

- Warning: `subworkflows/local/cram_qc_mosdepth_samtools/main.nf:23:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      MOSDEPTH(cram.combine(intervals.map { meta, bed -> [bed ?: []] }), fasta)
                                            ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:137:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .collect { [it] }
                              ^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:46:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              CREATE_INTERVALS_BED(intervals_combined.map{ meta, path -> path }, nucleotides_per_second)
                                                           ^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:87:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .flatten().collate(2).map{ duration, intervalFile -> intervalFile }.collect()
                                         ^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:93:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          TABIX_BGZIPTABIX_INTERVAL_SPLIT(intervals_bed.map{ file, num_intervals -> [ [ id:file.baseName], file ] })
                                                                   ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:95:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          intervals_bed_gz_tbi = TABIX_BGZIPTABIX_INTERVAL_SPLIT.out.gz_index.map{ meta, bed, tbi -> [ bed, tbi ] }.toList()
                                                                                   ^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:103:60`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      intervals_bed_combined        = intervals_combined.map{meta, bed -> bed }.collect()
                                                             ^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:104:89`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      intervals_bed_gz_tbi_combined = TABIX_BGZIPTABIX_INTERVAL_COMBINED.out.gz_index.map{meta, gz, tbi -> [gz, tbi] }.collect()
                                                                                          ^^^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:16:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          has_vardb: it.vardb != null
                     ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:23:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_branched.needs_vardb.map { [[id: it.vcf.baseName], it.vcf, it.tbi, it.fields ? it.fields.replace(';', ',') : ''] }
                                              ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:23:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_branched.needs_vardb.map { [[id: it.vcf.baseName], it.vcf, it.tbi, it.fields ? it.fields.replace(';', ',') : ''] }
                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:23:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_branched.needs_vardb.map { [[id: it.vcf.baseName], it.vcf, it.tbi, it.fields ? it.fields.replace(';', ',') : ''] }
                                                                        ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:23:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_branched.needs_vardb.map { [[id: it.vcf.baseName], it.vcf, it.tbi, it.fields ? it.fields.replace(';', ',') : ''] }
                                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:23:91`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_branched.needs_vardb.map { [[id: it.vcf.baseName], it.vcf, it.tbi, it.fields ? it.fields.replace(';', ',') : ''] }
                                                                                            ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:29:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .join(ch_branched.needs_vardb.map { [it.vcf.baseName, it] })
                                               ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:29:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .join(ch_branched.needs_vardb.map { [it.vcf.baseName, it] })
                                                                ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:34:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it.vcf, it.tbi, it.vardb, it.fields ? it.fields.replace(';', ',') : '', it.prefix ?: ''] }
                  ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:34:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it.vcf, it.tbi, it.vardb, it.fields ? it.fields.replace(';', ',') : '', it.prefix ?: ''] }
                          ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:34:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it.vcf, it.tbi, it.vardb, it.fields ? it.fields.replace(';', ',') : '', it.prefix ?: ''] }
                                  ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:34:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it.vcf, it.tbi, it.vardb, it.fields ? it.fields.replace(';', ',') : '', it.prefix ?: ''] }
                                            ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:34:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it.vcf, it.tbi, it.vardb, it.fields ? it.fields.replace(';', ',') : '', it.prefix ?: ''] }
                                                        ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:34:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [it.vcf, it.tbi, it.vardb, it.fields ? it.fields.replace(';', ',') : '', it.prefix ?: ''] }
                                                                                          ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:42:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  list.collect { it[0] },  // db_vcf
                                 ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:43:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  list.collect { it[1] },  // db_vcf_tbi
                                 ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:44:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  list.collect { it[2] },  // db_vardb
                                 ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:45:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  list.collect { it[3] },  // db_fields
                                 ^^
  ```

- Warning: `subworkflows/local/prepare_snpsift_databases/main.nf:46:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  list.collect { it[4] }   // db_prefixes
                                 ^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:13:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      bcftools_columns              // Path: bcftools columns
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:53:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def status0_count = samples.count { it.status == 0 }
                                                  ^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:54:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def status1_count = samples.count { it.status == 1 }
                                                  ^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:70:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { combination_key, combination_list ->
                 ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:90:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              [patient, samples.collect { it.sample }]
                                          ^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:245:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it[0].status == 1 }
                        ^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:263:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it[0].status == 0 }
                        ^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:437:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (it[0].sex == 'NA') {
                  ^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:446:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (it[0].status == 1 && !it[0].containsKey('contamination')) {
                  ^^
  ```

- Warning: `subworkflows/local/samplesheet_to_channel/main.nf:446:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              if (it[0].status == 1 && !it[0].containsKey('contamination')) {
                                        ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:18:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch{ meta, vcf, tbi ->
                         ^^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:18:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch{ meta, vcf, tbi ->
                              ^^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:53:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              def sorted_vcfs = sorted_pairs.collect { it[0] }
                                                                       ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:54:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              def callers = sorted_pairs.collect { it[1] }
                                                                   ^^
  ```

- Warning: `subworkflows/local/vcf_consensus/main.nf:65:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, dir ->
                    ^^^^
  ```

- Warning: `workflows/sarek.nf:143:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              bam: it[0].data_type == "bam"
                   ^^
  ```

- Warning: `workflows/sarek.nf:144:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              fastq_gz: it[0].data_type == "fastq_gz"
                        ^^
  ```

- Warning: `workflows/sarek.nf:145:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              one_fastq_gz_spring: it[0].data_type == "one_fastq_gz_spring"
                                   ^^
  ```

- Warning: `workflows/sarek.nf:146:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              two_fastq_gz_spring: it[0].data_type == "two_fastq_gz_spring"
                                   ^^
  ```

- Warning: `workflows/sarek.nf:292:77`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              cram_variant_calling_status_tmp = cram_variant_calling.branch { meta, file, index ->
                                                                              ^^^^
  ```

- Warning: `workflows/sarek.nf:292:89`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              cram_variant_calling_status_tmp = cram_variant_calling.branch { meta, file, index ->
                                                                                          ^^^^^
  ```

- Warning: `workflows/sarek.nf:312:75`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          cram_variant_calling_status = cram_variant_calling.branch { meta, file, index ->
                                                                            ^^^^
  ```

- Warning: `workflows/sarek.nf:312:81`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          cram_variant_calling_status = cram_variant_calling.branch { meta, file, index ->
                                                                                  ^^^^^
  ```

- Warning: `workflows/sarek.nf:318:73`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          bam_variant_calling_status = bam_variant_calling.branch { meta, file, index ->
                                                                          ^^^^
  ```

- Warning: `workflows/sarek.nf:318:79`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          bam_variant_calling_status = bam_variant_calling.branch { meta, file, index ->
                                                                                ^^^^^
  ```

- Warning: `workflows/sarek.nf:712:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def InputStream gzipStream = new java.util.zip.GZIPInputStream(it)
                                                                             ^^
  ```
