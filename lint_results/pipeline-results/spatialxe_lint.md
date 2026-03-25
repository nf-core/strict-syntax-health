# Nextflow lint results

- Generated: 2026-03-25T00:28:14.411997119Z
- Nextflow version: 26.03.0-edge
- Summary: 11 errors, 116 warnings

## :x: Errors

- Error: `conf/base.config:13:28`: Unexpected input: 'Math'

  ```nextflow
      cpus   = { 1    * (int)Math.pow(4, task.attempt - 1) }
                             ^
  ```

- Error: `conf/modules.config:98:57`: Unexpected input: 'Math'

  ```nextflow
          memory = { params.baysor_tiling ? 240.GB * (int)Math.pow(2, task.attempt - 1) : 720.GB }
                                                          ^
  ```

- Error: `modules/local/segger/train/main.nf:29:35`: Unexpected input: 'Math'

  ```nextflow
      def gpu_count = Math.min((int)Math.pow(2, task.attempt + 1), params.devices as int)
                                    ^
  ```

- Error: `subworkflows/local/baysor_run_transcripts_parquet/main.nf:183:14`: Unexpected input: 'i'

  ```nextflow
      for (int i = 0; i < ids.size(); i++) {
               ^
  ```

- Error: `subworkflows/local/segger_create_train_predict/main.nf:6:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/spatialxe/modules/local/segger/train/main.nf'

  ```nextflow
  include { SEGGER_TRAIN                     } from '../../../modules/local/segger/train/main'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/segger_create_train_predict/main.nf:37:9`: `SEGGER_TRAIN` is not defined

  ```nextflow
          SEGGER_TRAIN(SEGGER_CREATE_DATASET.out.datasetdir)
          ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/segger_create_train_predict/main.nf:39:19`: `SEGGER_TRAIN` is not defined

  ```nextflow
              .join(SEGGER_TRAIN.out.trained_models)
                    ^^^^^^^^^^^^
  ```

- Error: `workflows/spatialxe.nf:26:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/spatialxe/subworkflows/local/baysor_run_transcripts_parquet/main.nf'

  ```nextflow
  include { BAYSOR_RUN_TRANSCRIPTS_PARQUET                   } from '../subworkflows/local/baysor_run_transcripts_parquet/main'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/spatialxe.nf:448:13`: `BAYSOR_RUN_TRANSCRIPTS_PARQUET` is not defined

  ```nextflow
              BAYSOR_RUN_TRANSCRIPTS_PARQUET(
              ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/spatialxe.nf:455:35`: `BAYSOR_RUN_TRANSCRIPTS_PARQUET` is not defined

  ```nextflow
              ch_redefined_bundle = BAYSOR_RUN_TRANSCRIPTS_PARQUET.out.redefined_bundle
                                    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/spatialxe.nf:456:35`: `BAYSOR_RUN_TRANSCRIPTS_PARQUET` is not defined

  ```nextflow
              ch_coordinate_space = BAYSOR_RUN_TRANSCRIPTS_PARQUET.out.coordinate_space
                                    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/baysor/run/main.nf:44:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ].findAll { it }
                  ^^
  ```

- Warning: `modules/local/ficture/model/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/ficture/model/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/ficture/model/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/ficture/model/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/ficture/preprocess/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/baysor_generate_preview/main.nf:17:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/baysor_generate_preview/main.nf:18:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_preview_mqc_html = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/baysor_generate_preview/main.nf:19:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_preview_mqc_png  = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/baysor_generate_segfree/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/baysor_generate_segfree/main.nf:18:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_transcripts = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/baysor_run_prior_segmentation_mask/main.nf:19:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/baysor_run_prior_segmentation_mask/main.nf:21:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_transcripts = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/baysor_run_prior_segmentation_mask/main.nf:23:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_redefined_bundle = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/baysor_run_prior_segmentation_mask/main.nf:24:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_coordinate_space = Channel.value("pixels")
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/baysor_run_transcripts_parquet_tiled/main.nf:20:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_coordinate_space = Channel.value("microns")
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/baysor_run_transcripts_parquet_tiled/main.nf:64:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def sorted = patch_data.sort { it[0] }
                                             ^^
  ```

- Warning: `subworkflows/local/baysor_run_transcripts_parquet_tiled/main.nf:65:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def patch_ids = sorted.collect { it[0] }
                                               ^^
  ```

- Warning: `subworkflows/local/baysor_run_transcripts_parquet_tiled/main.nf:66:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def csvs = sorted.collect { it[1] }
                                          ^^
  ```

- Warning: `subworkflows/local/baysor_run_transcripts_parquet_tiled/main.nf:67:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def geojsons = sorted.collect { it[2] }
                                              ^^
  ```

- Warning: `subworkflows/local/cellpose_baysor_import_segmentation/main.nf:26:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/cellpose_baysor_import_segmentation/main.nf:27:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_transcripts = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/cellpose_baysor_import_segmentation/main.nf:28:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_imp_seg_inputs = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/cellpose_baysor_import_segmentation/main.nf:29:5`: Variable was declared but not used

  ```nextflow
      ch_filtered_transcripts = Channel.empty()
      ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/cellpose_baysor_import_segmentation/main.nf:29:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_filtered_transcripts = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/cellpose_baysor_import_segmentation/main.nf:30:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_coordinate_space = Channel.value("microns")
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/cellpose_resolift_morphology_ome_tif/main.nf:21:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/cellpose_resolift_morphology_ome_tif/main.nf:22:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_imp_seg_inputs = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/cellpose_resolift_morphology_ome_tif/main.nf:23:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_coordinate_space = Channel.value("pixels")
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/cellpose_resolift_morphology_ome_tif/main.nf:53:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_scale_info = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/ficture_preprocess_model/main.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/ficture_preprocess_model/main.nf:29:77`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_features_clean = params.features ? FICTURE_PREPROCESS.out.features : Channel.value([])
                                                                              ^^^^^^^
  ```

- Warning: `subworkflows/local/opt_flip_track_stat/main.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/opt_flip_track_stat/main.nf:15:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_summary = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/proseg_preset_proseg2baysor/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/proseg_preset_proseg2baysor/main.nf:17:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_coordinate_space = Channel.value("microns")
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/proseg_preset_proseg2baysor_tiled/main.nf:19:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/proseg_preset_proseg2baysor_tiled/main.nf:20:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_coordinate_space = Channel.value("microns")
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/proseg_preset_proseg2baysor_tiled/main.nf:52:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def sorted = patch_data.sort { it[0] }
                                             ^^
  ```

- Warning: `subworkflows/local/proseg_preset_proseg2baysor_tiled/main.nf:53:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def patch_ids = sorted.collect { it[0] }
                                               ^^
  ```

- Warning: `subworkflows/local/proseg_preset_proseg2baysor_tiled/main.nf:54:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def csvs = sorted.collect { it[1] }
                                          ^^
  ```

- Warning: `subworkflows/local/proseg_preset_proseg2baysor_tiled/main.nf:55:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def geojsons = sorted.collect { it[2] }
                                              ^^
  ```

- Warning: `subworkflows/local/segger_create_train_predict/main.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/segger_create_train_predict/main.nf:21:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_coordinate_space = Channel.value("microns")
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/spatialdata_write_meta_merge/main.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/spatialdata_write_meta_merge/main.nf:19:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_segmented_object = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/spatialdata_write_meta_merge/main.nf:25:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_segmented_object = Channel.value('cells_and_nuclei')
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/spatialdata_write_meta_merge/main.nf:28:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_segmented_object = Channel.value('nuclei')
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/spatialdata_write_meta_merge/main.nf:31:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_segmented_object = Channel.value('cells')
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/spatialdata_write_meta_merge/main.nf:34:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_segmented_object = Channel.value([])
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/spatialdata_write_meta_merge/main.nf:40:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_segmented_object = Channel.value([])
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/stardist_resolift_morphology_ome_tif/main.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/stardist_resolift_morphology_ome_tif/main.nf:19:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_imp_seg_inputs = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/stardist_resolift_morphology_ome_tif/main.nf:20:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_coordinate_space = Channel.value("pixels")
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_spatialxe_pipeline/main.nf:30:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_spatialxe_pipeline/main.nf:40:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_spatialxe_pipeline/main.nf:65:144`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      after_text = """${workflow.manifest.doi ? "\n* The pipeline\n" : ""}${workflow.manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/', '')}" }.join("\n")}${workflow.manifest.doi ? "\n" : ""}
                                                                                                                                                 ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_spatialxe_pipeline/main.nf:104:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromList(samplesheetToList(input, "${projectDir}/assets/schema_input.json"))
          ^^^^^^^
  ```

- Warning: `subworkflows/local/xeniumranger_import_segmentation_redefine_bundle/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/xeniumranger_import_segmentation_redefine_bundle/main.nf:17:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_redefined_bundle = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/xeniumranger_import_segmentation_redefine_bundle/main.nf:18:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_coordinate_space = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/xeniumranger_relabel_resegment/main.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/xeniumranger_resegment_morphology_ome_tif/main.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/xeniumranger_resegment_morphology_ome_tif/main.nf:15:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_redefined_bundle = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/xeniumranger_resegment_morphology_ome_tif/main.nf:16:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_coordinate_space = Channel.value("pixels")
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/xeniumranger_resegment_morphology_ome_tif/main.nf:34:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, bundle, reseg_bundle, cells_zarr ->
                                   ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:101:98`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return ch_versions.unique().map { version -> processVersionsFromYAML(version) }.unique().mix(Channel.of(workflowVersionToYAML()))
                                                                                                   ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:67:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:69:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_input = Channel.empty()
                 ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:70:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_config = Channel.empty()
                  ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:71:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_features = Channel.value([])
                    ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:72:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_raw_bundle = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:73:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gene_panel = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:74:21`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_qc_reports = Channel.empty()
                      ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:75:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_bundle_path = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:76:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_preview_html = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:77:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_exp_metadata = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:78:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gene_synonyms = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:79:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:80:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_report = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:81:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_qupath_polygons = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:82:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_morphology_image = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:83:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_redefined_bundle = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:84:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_coordinate_space = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:85:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_panel_probes_fasta = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:86:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_transcripts_file = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:87:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_reference_annotations = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:88:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_pre_xr_report = Channel.empty()
                                 ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:89:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_post_xr_report = Channel.empty()
                                  ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:194:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_config = Channel.fromPath(
                  ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:202:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_segmentation_mask = Channel.fromPath(
                                 ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:211:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.fromPath(params.features, checkIfExists: true).flatten()
            ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:212:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.value([])
            ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:216:9`: Variable was declared but not used

  ```nextflow
          ch_cellpose_model = Channel.fromPath(
          ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:216:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_cellpose_model = Channel.fromPath(
                              ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:225:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_panel_probes_fasta = Channel.fromPath(
                                  ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:234:36`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_reference_annotations = Channel.fromPath(
                                     ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:243:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gene_synonyms = Channel.fromPath(
                             ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:252:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_qupath_polygons = Channel.fromPath(
                               ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:446:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_prior_mask = Channel.empty()
                              ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:552:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_config = Channel.fromPath(
                          ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:558:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.fromPath(params.multiqc_config, checkIfExists: true)
            ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:559:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.empty()
            ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:562:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ? Channel.fromPath(params.multiqc_logo, checkIfExists: true)
            ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:563:11`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          : Channel.empty()
            ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:573:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_workflow_summary = Channel.value(paramsSummaryMultiqc(summary_params))
                            ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:583:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_methods_description = Channel.value(
                               ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:604:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files.collect().map { [it] }
                                                ^^
  ```

- Warning: `workflows/spatialxe.nf:605:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .combine(ch_multiqc_configs.map { [it] })
                                                     ^^
  ```

- Warning: `workflows/spatialxe.nf:606:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .combine(ch_multiqc_logo.toList().map { [it] })
                                                           ^^
  ```

- Warning: `workflows/spatialxe.nf:619:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files.collect().map { [it] }
                                                ^^
  ```

- Warning: `workflows/spatialxe.nf:620:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .combine(ch_multiqc_configs.map { [it] })
                                                     ^^
  ```

- Warning: `workflows/spatialxe.nf:621:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .combine(ch_multiqc_logo.toList().map { [it] })
                                                           ^^
  ```

- Warning: `workflows/spatialxe.nf:658:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files.collect().map { [it] }
                                                ^^
  ```

- Warning: `workflows/spatialxe.nf:659:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .combine(ch_multiqc_configs.map { [it] })
                                                     ^^
  ```

- Warning: `workflows/spatialxe.nf:660:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .combine(ch_multiqc_logo.toList().map { [it] })
                                                           ^^
  ```
