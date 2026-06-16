# Nextflow lint results

- Generated: 2026-06-16T19:28:10.695980759Z
- Nextflow version: 26.04.3
- Summary: 12 errors, 31 warnings

## :x: Errors

- Error: `modules/local/hicpro/dnase_mapping_stats.nf:2:10`: `sample` is not defined

  ```nextflow
      tag "$sample = $bam"
           ^^^^^^^
  ```

- Error: `subworkflows/local/compartments/main.nf:26:28`: `cool` is already declared

  ```nextflow
              cool.map{meta, cool, res -> [meta, cool] },
                             ^^^^
  ```

- Error: `subworkflows/local/cooler/main.nf:43:47`: `pairs` is already declared

  ```nextflow
      cload_inputs = pairs_res.multiMap { meta, pairs, index, cool_bin ->
                                                ^^^^^
  ```

- Error: `subworkflows/local/hicpro/main.nf:18:5`: `meta` was assigned but not declared

  ```nextflow
      meta = row[0].clone()
      ^^^^
  ```

- Error: `subworkflows/local/hicpro/main.nf:19:5`: `meta` is not defined

  ```nextflow
      meta.remove('chunk')
      ^^^^
  ```

- Error: `subworkflows/local/hicpro/main.nf:20:13`: `meta` is not defined

  ```nextflow
      return [meta, row[1]]
              ^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_hic_pipeline/main.nf:140:13`: `completionEmail` is not defined

  ```nextflow
              completionEmail(
              ^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_hic_pipeline/main.nf:153:13`: `imNotification` is not defined

  ```nextflow
              imNotification(summary_params, hook_url)
              ^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_hic_pipeline/main.nf:292:9`: `meta` was assigned but not declared

  ```nextflow
          meta = row[0].clone()
          ^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_hic_pipeline/main.nf:293:9`: `meta` is not defined

  ```nextflow
          meta.chunk = i
          ^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_hic_pipeline/main.nf:294:9`: `meta` is not defined

  ```nextflow
          meta.part = row[1].size()
          ^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_hic_pipeline/main.nf:295:17`: `meta` is not defined

  ```nextflow
          map += [meta, file]
                  ^^^^
  ```

## :warning: Warnings

- Warning: `main.nf:73:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = HIC.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/hicexplorer/hicPlotDistVsCounts.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/split_cooler_dump/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/compartments/main.nf:26:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              cool.map{meta, cool, res -> [meta, cool] },
                                   ^^^
  ```

- Warning: `subworkflows/local/cooler/main.nf:60:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_cool.map{[it[0], it[1], ""]}
                       ^^
  ```

- Warning: `subworkflows/local/cooler/main.nf:60:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_cool.map{[it[0], it[1], ""]}
                              ^^
  ```

- Warning: `subworkflows/local/cooler/main.nf:72:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter{ it[2] == it[3] }
                   ^^
  ```

- Warning: `subworkflows/local/cooler/main.nf:72:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter{ it[2] == it[3] }
                            ^^
  ```

- Warning: `subworkflows/local/cooler/main.nf:85:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          COOLER_BALANCE.out.cool.map{[it[0], it[1], ""]}
                                       ^^
  ```

- Warning: `subworkflows/local/cooler/main.nf:85:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

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

- Warning: `subworkflows/local/utils_nfcore_hic_pipeline/main.nf:29:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_hic_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_hic_pipeline/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      help              // boolean: Display help message and exit
      ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_hic_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      help_full         // boolean: Show the full help message
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_hic_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      show_hidden       // boolean: Show hidden parameters in the help message
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      valid_config
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/hic.nf:38:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_restriction_site
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/hic.nf:97:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def paired = files.findAll { it.name =~ /_val_[12]\.fq\.gz$/ }
                                           ^^
  ```

- Warning: `workflows/hic.nf:110:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(FASTQC.out.zip.collect{it[1]})
                                                                     ^^
  ```

- Warning: `workflows/hic.nf:155:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter{ it[0].resolution == it[2] }
                       ^^
  ```

- Warning: `workflows/hic.nf:155:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter{ it[0].resolution == it[2] }
                                           ^^
  ```

- Warning: `workflows/hic.nf:170:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter{ it[0].resolution == it[2] }
                       ^^
  ```

- Warning: `workflows/hic.nf:170:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter{ it[0].resolution == it[2] }
                                           ^^
  ```

- Warning: `workflows/hic.nf:187:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter{ it[0].resolution == it[2] }
                       ^^
  ```

- Warning: `workflows/hic.nf:187:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter{ it[0].resolution == it[2] }
                                           ^^
  ```

- Warning: `workflows/hic.nf:254:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = MULTIQC.out.report.map { _meta, report -> [report] }.toList() // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
