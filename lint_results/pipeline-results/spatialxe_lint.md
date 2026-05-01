# Nextflow lint results

- Generated: 2026-05-01T00:36:38.671760865Z
- Nextflow version: 26.04.0
- Summary: 28 warnings

## :warning: Warnings

- Warning: `modules/local/baysor/run/main.nf:44:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ].findAll { it }
                  ^^
  ```

- Warning: `subworkflows/local/baysor_run_transcripts_parquet/main.nf:75:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def sorted = patch_data.sort { it[0] }
                                                 ^^
  ```

- Warning: `subworkflows/local/baysor_run_transcripts_parquet/main.nf:76:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def patch_ids = sorted.collect { it[0] }
                                                   ^^
  ```

- Warning: `subworkflows/local/baysor_run_transcripts_parquet/main.nf:77:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def csvs = sorted.collect { it[1] }
                                              ^^
  ```

- Warning: `subworkflows/local/baysor_run_transcripts_parquet/main.nf:78:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def geojsons = sorted.collect { it[2] }
                                                  ^^
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

- Warning: `subworkflows/local/proseg_preset_proseg2baysor_tiled/main.nf:51:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def sorted = patch_data.sort { it[0] }
                                             ^^
  ```

- Warning: `subworkflows/local/proseg_preset_proseg2baysor_tiled/main.nf:52:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def patch_ids = sorted.collect { it[0] }
                                               ^^
  ```

- Warning: `subworkflows/local/proseg_preset_proseg2baysor_tiled/main.nf:53:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def csvs = sorted.collect { it[1] }
                                          ^^
  ```

- Warning: `subworkflows/local/proseg_preset_proseg2baysor_tiled/main.nf:54:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def geojsons = sorted.collect { it[2] }
                                              ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_spatialxe_pipeline/main.nf:30:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_spatialxe_pipeline/main.nf:63:144`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      after_text = """${workflow.manifest.doi ? "\n* The pipeline\n" : ""}${workflow.manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/', '')}" }.join("\n")}${workflow.manifest.doi ? "\n" : ""}
                                                                                                                                                 ^^
  ```

- Warning: `subworkflows/local/xeniumranger_resegment_morphology_ome_tif/main.nf:33:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, bundle, reseg_bundle, cells_zarr ->
                                   ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:101:98`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return ch_versions.unique().map { version -> processVersionsFromYAML(version) }.unique().mix(Channel.of(workflowVersionToYAML()))
                                                                                                   ^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:215:9`: Variable was declared but not used

  ```nextflow
          ch_cellpose_model = channel.fromPath(
          ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/spatialxe.nf:603:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files.collect().map { [it] }
                                                ^^
  ```

- Warning: `workflows/spatialxe.nf:604:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .combine(ch_multiqc_configs.map { [it] })
                                                     ^^
  ```

- Warning: `workflows/spatialxe.nf:605:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .combine(ch_multiqc_logo.toList().map { [it] })
                                                           ^^
  ```

- Warning: `workflows/spatialxe.nf:618:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files.collect().map { [it] }
                                                ^^
  ```

- Warning: `workflows/spatialxe.nf:619:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .combine(ch_multiqc_configs.map { [it] })
                                                     ^^
  ```

- Warning: `workflows/spatialxe.nf:620:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .combine(ch_multiqc_logo.toList().map { [it] })
                                                           ^^
  ```

- Warning: `workflows/spatialxe.nf:656:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files.collect().map { [it] }
                                                ^^
  ```

- Warning: `workflows/spatialxe.nf:657:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .combine(ch_multiqc_configs.map { [it] })
                                                     ^^
  ```

- Warning: `workflows/spatialxe.nf:658:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .combine(ch_multiqc_logo.toList().map { [it] })
                                                           ^^
  ```
