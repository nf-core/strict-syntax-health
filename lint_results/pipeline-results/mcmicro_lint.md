# Nextflow lint results

- Generated: 2026-07-10T00:36:00.990555158Z
- Nextflow version: 26.06.0-edge
- Summary: 74 warnings

## :warning: Warnings

- Warning: `main.nf:51:5`: Emit name should be omitted when there is only one emit

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

- Warning: `subworkflows/local/update_from_ome/main.nf:27:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          meta, image_tiles, dfp, ffp -> [meta.cycle_number, meta.channel_count]
                                ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:27:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          meta, image_tiles, dfp, ffp -> [meta.cycle_number, meta.channel_count]
                                             ^^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:27:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                          meta, image_tiles, dfp, ffp -> [meta.cycle_number, meta.channel_count]
                                                  ^^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:42:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, xml_meta, marker_meta -> marker_meta.collect{ it -> meta.subMap('id') + it }
                    ^^^^^^^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:50:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              key, meta, counter ->
              ^^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:70:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .combine(samplesheet_meta.map{ it[0].subMap('id') }.unique())
                                         ^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:73:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map{ e -> [e.subMap('id', 'channel_number', 'cycle_number'), e.findAll{ it.value != null }] }
                                                                                   ^^
  ```

- Warning: `subworkflows/local/update_from_ome/main.nf:80:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter{ e -> !e.any{it == null}} // ignore errors, will be caught in PRELUDE
                               ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:36:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      marker_sheet      //  string: Path to marker_sheet
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:116:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .flatMap { expandSampleRow(it) }
                                         ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:122:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .collect({ it[0] }, flat: false)
                     ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:123:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map{ validateInputMarkersheet(it) }
                                         ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:198:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      if (params.cellpose_model && !params.segmentation.split(',').any{ it.equalsIgnoreCase("cellpose") }) {
                                                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:240:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def dups = test_tuples.countBy{ it }.findAll{ unused, count -> count > 1 }*.key
                                      ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:240:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def dups = test_tuples.countBy{ it }.findAll{ unused, count -> count > 1 }*.key
                                                    ^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:248:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          if (markersheet_data*.subMap(backsub_columns)*.collect{ c, v -> v != null }.flatten().any()) {
                                                                  ^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:252:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def markers_used_as_background = markersheet_data.findResults{ it.background }.toSet()
                                                                         ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:275:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def sample_cycles = samples.collect{ meta, image_tiles, dfp, ffp -> meta.cycle_number }
                                                 ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:275:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def sample_cycles = samples.collect{ meta, image_tiles, dfp, ffp -> meta.cycle_number }
                                                              ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:275:66`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def sample_cycles = samples.collect{ meta, image_tiles, dfp, ffp -> meta.cycle_number }
                                                                   ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:285:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def channel_cycle_map = samples.collect{ meta, image_tiles, dfp, ffp -> [meta.id,meta.cycle_number] }.groupBy{ it[0] }
                                                     ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:285:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def channel_cycle_map = samples.collect{ meta, image_tiles, dfp, ffp -> [meta.id,meta.cycle_number] }.groupBy{ it[0] }
                                                                  ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:285:70`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def channel_cycle_map = samples.collect{ meta, image_tiles, dfp, ffp -> [meta.id,meta.cycle_number] }.groupBy{ it[0] }
                                                                       ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:285:116`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def channel_cycle_map = samples.collect{ meta, image_tiles, dfp, ffp -> [meta.id,meta.cycle_number] }.groupBy{ it[0] }
                                                                                                                     ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:288:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          entry.value.collect{ it[1] }.each{ curr_val ->
                               ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:305:12`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          if(it.toString().endsWith(".ome.tif")){
             ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mcmicro_pipeline/main.nf:306:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              files << file(it)
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

- Warning: `workflows/mcmicro.nf:39:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      outdir
      ^^^^^^
  ```

- Warning: `workflows/mcmicro.nf:47:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_samplesheet.map{meta, image_tiles, dfp, ffp -> [meta, image_tiles]} | BFTOOLS_SHOWINF
                                            ^^^
  ```

- Warning: `workflows/mcmicro.nf:47:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_samplesheet.map{meta, image_tiles, dfp, ffp -> [meta, image_tiles]} | BFTOOLS_SHOWINF
                                                 ^^^
  ```

- Warning: `workflows/mcmicro.nf:67:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .combine(ch_has_no_errors.map{meta, has_no_error -> has_no_error})
                                    ^^^^
  ```

- Warning: `workflows/mcmicro.nf:68:14`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter{ meta, image_tiles, dfp, ffp, has_no_error -> has_no_error && !params.prelude}
               ^^^^
  ```

- Warning: `workflows/mcmicro.nf:68:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter{ meta, image_tiles, dfp, ffp, has_no_error -> has_no_error && !params.prelude}
                     ^^^^^^^^^^^
  ```

- Warning: `workflows/mcmicro.nf:68:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter{ meta, image_tiles, dfp, ffp, has_no_error -> has_no_error && !params.prelude}
                                  ^^^
  ```

- Warning: `workflows/mcmicro.nf:68:38`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter{ meta, image_tiles, dfp, ffp, has_no_error -> has_no_error && !params.prelude}
                                       ^^^
  ```

- Warning: `workflows/mcmicro.nf:69:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .map{meta, image_tiles, dfp, ffp, error -> [meta, image_tiles, dfp, ffp]}.dump(tag:"SampleAfterFiltering")
                                        ^^^^^
  ```

- Warning: `workflows/mcmicro.nf:77:38`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map{ meta, image_tiles, dfp, ffp -> [meta, image_tiles] }
                                       ^^^
  ```

- Warning: `workflows/mcmicro.nf:77:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map{ meta, image_tiles, dfp, ffp -> [meta, image_tiles] }
                                            ^^^
  ```

- Warning: `workflows/mcmicro.nf:82:38`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map{ meta, image_tiles, dfp, ffp -> [meta, image_tiles] }
                                       ^^^
  ```

- Warning: `workflows/mcmicro.nf:82:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map{ meta, image_tiles, dfp, ffp -> [meta, image_tiles] }
                                            ^^^
  ```

- Warning: `workflows/mcmicro.nf:93:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map{ meta, cycles -> [meta] + cycles.collect{ it[1..-1] }.transpose() }
                                                         ^^
  ```

- Warning: `workflows/mcmicro.nf:108:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it.collect{ it.channel_number + "," + it.cycle_number + "," + it.marker_name + "," + it.exposure + "," + it.background + "," + it.remove}] }
                  ^^
  ```

- Warning: `workflows/mcmicro.nf:108:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it.collect{ it.channel_number + "," + it.cycle_number + "," + it.marker_name + "," + it.exposure + "," + it.background + "," + it.remove}] }
                              ^^
  ```

- Warning: `workflows/mcmicro.nf:108:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it.collect{ it.channel_number + "," + it.cycle_number + "," + it.marker_name + "," + it.exposure + "," + it.background + "," + it.remove}] }
                                                        ^^
  ```

- Warning: `workflows/mcmicro.nf:108:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it.collect{ it.channel_number + "," + it.cycle_number + "," + it.marker_name + "," + it.exposure + "," + it.background + "," + it.remove}] }
                                                                                ^^
  ```

- Warning: `workflows/mcmicro.nf:108:102`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it.collect{ it.channel_number + "," + it.cycle_number + "," + it.marker_name + "," + it.exposure + "," + it.background + "," + it.remove}] }
                                                                                                       ^^
  ```

- Warning: `workflows/mcmicro.nf:108:122`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it.collect{ it.channel_number + "," + it.cycle_number + "," + it.marker_name + "," + it.exposure + "," + it.background + "," + it.remove}] }
                                                                                                                           ^^
  ```

- Warning: `workflows/mcmicro.nf:108:144`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it.collect{ it.channel_number + "," + it.cycle_number + "," + it.marker_name + "," + it.exposure + "," + it.background + "," + it.remove}] }
                                                                                                                                                 ^^
  ```

- Warning: `workflows/mcmicro.nf:110:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { it.replaceAll('(?<=,|^)null(?=,|$)', '') }
                     ^^
  ```

- Warning: `workflows/mcmicro.nf:184:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .cross(ch_masks) { it[0]['id'] }
                             ^^
  ```

- Warning: `workflows/mcmicro.nf:256:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_has_no_errors.map{ if (!it[1]) error "QC Error found" }
                                 ^^
  ```
