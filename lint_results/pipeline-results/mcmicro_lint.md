# Nextflow lint results

- Generated: 2026-06-16T20:29:08.612818922Z
- Nextflow version: 26.04.3
- Summary: 13 errors, 55 warnings

## :x: Errors

- Error: `main.nf:18:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/mcmicro/workflows/mcmicro.nf'

  ```nextflow
  include { MCMICRO  } from './workflows/mcmicro'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:42:5`: `MCMICRO` is not defined

  ```nextflow
      MCMICRO (
      ^^^^^^^
  ```

- Error: `main.nf:47:22`: `MCMICRO` is not defined

  ```nextflow
      multiqc_report = MCMICRO.out.multiqc_report // channel: /path/to/multiqc_report.html
                       ^^^^^^^
  ```

- Error: `modules/local/omevalidation/main.nf:28:53`: Unexpected character: '@'

  ```nextflow
              node -> node.name() == 'Pixels' && node.@SizeX != '' && node.@SizeY != ''
                                                      ^
  ```

- Error: `subworkflows/local/update_from_ome/main.nf:1:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/mcmicro/modules/local/omevalidation/main.nf'

  ```nextflow
  include { OMEVALIDATION   } from '../../../modules/local/omevalidation/main'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/update_from_ome/main.nf:15:48`: `OMEVALIDATION` is not defined

  ```nextflow
      val_data = xml.map{meta, x -> [meta, x]} | OMEVALIDATION
                                                 ^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/update_from_ome/main.nf:36:13`: Variables in a closure should be declared with `def`

  ```nextflow
              temp = [cn, c_sum]
              ^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:10:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import groovy.io.FileType
  ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:196:35`: `segmentation_list` is not defined

  ```nextflow
      if (params.cellpose_model && !segmentation_list.contains('cellpose')) {
                                    ^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:238:51`: `_` is not allowed as an identifier because it is reserved for future use

  ```nextflow
      def dups = test_tuples.countBy{ it }.findAll{ _, count -> count > 1 }*.key
                                                    ^
  ```

- Error: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:302:44`: `FileType` is not defined

  ```nextflow
      file(image_directory).eachFileRecurse (FileType.FILES) {
                                             ^^^^^^^^
  ```

- Error: `tests/lib/utils.nf:15:5`: Unrecognized process output qualifier `publishDir`

  ```nextflow
      publishDir enabled: false
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/mcmicro.nf:89:38`: Unexpected input: '\*'

  ```nextflow
          .map{ meta, cycles -> [meta, *cycles.collect{ it[1..-1] }.transpose()]}
                                       ^
  ```

## :warning: Warnings

- Warning: `main.nf:47:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = MCMICRO.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/summary_markersheet/main.nf:20:9`: Variable was declared but not used

  ```nextflow
      def args        = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/bftools/showinf/main.nf:37:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args   ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/cellpose/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/cellpose/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/mcquant/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/scimap/mcmicro/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/scimap/mcmicro/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/scimap/mcmicro/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/scimap/mcmicro/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `subworkflows/local/prelude/main.nf:26:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                      meta, image_tiles, dfp, ffp ->
                                            ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prelude/main.nf:26:56`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                      meta, image_tiles, dfp, ffp ->
                                                         ^^^
  ```

- Warning: `subworkflows/local/prelude/main.nf:26:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                      meta, image_tiles, dfp, ffp ->
                                                              ^^^
  ```

- Warning: `subworkflows/local/prelude/main.nf:33:57`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                                          meta, file -> file
                                                          ^^^^
  ```

- Warning: `subworkflows/local/prelude/main.nf:40:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                      meta, files -> files
                                      ^^^^
  ```

- Warning: `subworkflows/local/prelude/main.nf:43:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                                      meta, files -> files
                                      ^^^^
  ```

- Warning: `subworkflows/local/prelude/main.nf:50:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      output_file_xml                  = ch_output_xml.output.map{ meta, files -> files}
                                                                   ^^^^
  ```

- Warning: `subworkflows/local/prelude/main.nf:51:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      output_file_samplesheet          = ch_output_samplesheet.map{ meta, files -> files}
                                                                    ^^^^
  ```

- Warning: `subworkflows/local/prelude/main.nf:52:67`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      output_file_markersheet          = ch_output_markersheet.map{ meta, files -> files}
                                                                    ^^^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:18:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
           .map { original_meta, image_tiles, dfp, ffp, xml_meta, marker_data ->
                                                                  ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:29:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, image_tiles, dfp, ffp -> [meta.cycle_number, meta.channel_count]
                    ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:29:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, image_tiles, dfp, ffp -> [meta.cycle_number, meta.channel_count]
                                 ^^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:29:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, image_tiles, dfp, ffp -> [meta.cycle_number, meta.channel_count]
                                      ^^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:45:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, xml_meta, marker_meta -> marker_meta.collect{ meta.subMap('id') + it }
                    ^^^^^^^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:45:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              meta, xml_meta, marker_meta -> marker_meta.collect{ meta.subMap('id') + it }
                                                                                      ^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:53:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              key, meta, counter ->
              ^^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:71:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .combine(samplesheet_meta.map{ it[0].subMap('id') }.unique())
                                         ^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:72:15`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map{ it[0] + it[1] }
                ^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:72:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map{ it[0] + it[1] }
                        ^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:74:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map{ e -> [e.subMap('id', 'channel_number', 'cycle_number'), e.findAll{ it.value != null }] }
                                                                                   ^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:79:15`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map{ it.drop(1) }
                ^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:81:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter{ e -> !e.any{it == null}} // ignore errors, will be caught in PRELUDE
                               ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:38:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      marker_sheet      //  string: Path to marker_sheet
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:111:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .flatMap { expandSampleRow(it) }
                                         ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:117:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .collect({ it[0] }, flat: false)
                     ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:118:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map{ validateInputMarkersheet(it) }
                                         ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:238:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def dups = test_tuples.countBy{ it }.findAll{ _, count -> count > 1 }*.key
                                      ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:246:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          if (markersheet_data*.subMap(backsub_columns)*.collect{ c, v -> v != null }.flatten().any()) {
                                                                  ^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:250:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def markers_used_as_background = markersheet_data.findResults{ it.background }.toSet()
                                                                         ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:273:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def sample_cycles = samples.collect{ meta, image_tiles, dfp, ffp -> meta.cycle_number }
                                                 ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:273:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def sample_cycles = samples.collect{ meta, image_tiles, dfp, ffp -> meta.cycle_number }
                                                              ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:273:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def sample_cycles = samples.collect{ meta, image_tiles, dfp, ffp -> meta.cycle_number }
                                                                   ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:283:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def channel_cycle_map = samples.collect{ meta, image_tiles, dfp, ffp -> [meta.id,meta.cycle_number] }.groupBy{ it[0] }
                                                     ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:283:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def channel_cycle_map = samples.collect{ meta, image_tiles, dfp, ffp -> [meta.id,meta.cycle_number] }.groupBy{ it[0] }
                                                                  ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:283:70`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def channel_cycle_map = samples.collect{ meta, image_tiles, dfp, ffp -> [meta.id,meta.cycle_number] }.groupBy{ it[0] }
                                                                       ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:283:116`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def channel_cycle_map = samples.collect{ meta, image_tiles, dfp, ffp -> [meta.id,meta.cycle_number] }.groupBy{ it[0] }
                                                                                                                     ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:286:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          entry.value.collect{ it[1] }.each{ curr_val ->
                               ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:303:12`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          if(it.toString().endsWith(".ome.tif")){
             ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:304:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              files << file(it)
                            ^^
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

- Warning: `tests/lib/utils.nf:18:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def relPaths = f.collect{ "'../$it'" }.join(' ')
                                     ^^
  ```
