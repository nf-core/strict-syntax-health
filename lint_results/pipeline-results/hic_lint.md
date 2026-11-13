# Nextflow lint results

- Generated: 2026-11-13T00:15:20.816804472Z
- Nextflow version: 26.10.5
- Summary: 50 warnings

## :warning: Warnings

- Warning: `modules/local/fithichip/cool2matrix/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/fithichip/main.nf:35:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/hicexplorer/hicPlotDistVsCounts.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/pairs2bed/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pairtools/pairtools_parse.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/split_cooler_dump/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/split_cooler_dump/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/bowtie2/align/main.nf:32:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bowtie2/build/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bwa/index/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bwa/mem/main.nf:28:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/calder2/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/cooler/balance/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/cooler/cload/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/cooler/dump/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/cooler/makebins/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/cooler/zoomify/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fastqc/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/macs3/callpeak/main.nf:26:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pairix/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pairtools/dedup/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pairtools/merge/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pairtools/parse/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pairtools/restrict/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pairtools/select/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pairtools/sort/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pairtools/stats/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/faidx/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/flagstat/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/index/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/sort/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/trimgalore/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/local/compartments/main.nf:26:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              cool.map { meta, cool_file, res -> [meta, cool_file] },
                                          ^^^
  ```

- Warning: `subworkflows/local/cooler/main.nf:66:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_cool.map{[it[0], it[1], ""]}
                       ^^
  ```

- Warning: `subworkflows/local/cooler/main.nf:66:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_cool.map{[it[0], it[1], ""]}
                              ^^
  ```

- Warning: `subworkflows/local/cooler/main.nf:71:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter{ meta, cool, zoom_res -> meta.resolution == zoom_res }
                         ^^^^
  ```

- Warning: `subworkflows/local/cooler/main.nf:84:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          COOLER_BALANCE.out.cool.map{[it[0], it[1], ""]}
                                       ^^
  ```

- Warning: `subworkflows/local/cooler/main.nf:84:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          COOLER_BALANCE.out.cool.map{[it[0], it[1], ""]}
                                              ^^
  ```

- Warning: `subworkflows/local/pairtools/main.nf:66:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              single: it[0].part <=1
                      ^^
  ```

- Warning: `subworkflows/local/pairtools/main.nf:67:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              multiple: it[0].part > 1
                        ^^
  ```

- Warning: `workflows/hic.nf:39:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_restriction_site
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/hic.nf:114:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def paired = files.findAll { it.name =~ /_val_[12]\.fq\.gz$/ }
                                           ^^
  ```

- Warning: `workflows/hic.nf:128:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQC.out.zip.collect{it[1]})
                                                                         ^^
  ```

- Warning: `workflows/hic.nf:175:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter{ it[0].resolution == it[2] }
                       ^^
  ```

- Warning: `workflows/hic.nf:175:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter{ it[0].resolution == it[2] }
                                           ^^
  ```

- Warning: `workflows/hic.nf:190:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter{ it[0].resolution == it[2] }
                       ^^
  ```

- Warning: `workflows/hic.nf:190:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter{ it[0].resolution == it[2] }
                                           ^^
  ```

- Warning: `workflows/hic.nf:207:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter{ it[0].resolution == it[2] }
                       ^^
  ```

- Warning: `workflows/hic.nf:207:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter{ it[0].resolution == it[2] }
                                           ^^
  ```
