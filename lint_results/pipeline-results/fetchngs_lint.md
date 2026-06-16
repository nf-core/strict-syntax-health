# Nextflow lint results

- Generated: 2026-06-16T14:16:50.200329799Z
- Nextflow version: 26.04.3
- Summary: 15 warnings

## :warning: Warnings

- Warning: `modules/local/sra_to_samplesheet/main.nf:52:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      samplesheet  = pipeline_map.keySet().collect{ '"' + it + '"'}.join(",") + '\n'
                                                          ^^
  ```

- Warning: `modules/local/sra_to_samplesheet/main.nf:53:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      samplesheet += pipeline_map.values().collect{ '"' + it + '"'}.join(",")
                                                          ^^
  ```

- Warning: `modules/local/sra_to_samplesheet/main.nf:63:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def fields = mapping_fields ? ['sample'] + mapping_fields.split(',').collect{ it.trim().toLowerCase() } : []
                                                                                    ^^
  ```

- Warning: `modules/local/sra_to_samplesheet/main.nf:69:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      mappings  = fields.collect{ '"' + it + '"'}.join(",") + '\n'
                                        ^^
  ```

- Warning: `modules/local/sra_to_samplesheet/main.nf:70:69`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      mappings += mappings_map.subMap(fields).values().collect{ '"' + it + '"'}.join(",")
                                                                      ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_fetchngs_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_fetchngs_pipeline/main.nf:113:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      ids = ch_ids
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_fetchngs_pipeline/main.nf:202:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def actual_ena_metadata_fields = ena_metadata_fields ? ena_metadata_fields.split(',').collect { it.trim().toLowerCase() } : valid_ena_metadata_fields
                                                                                                      ^^
  ```

- Warning: `subworkflows/nf-core/fastq_download_prefetch_fasterqdump_sratools/main.nf:32:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      reads    = SRATOOLS_FASTERQDUMP.out.reads // channel: [ val(meta), [ reads ] ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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

- Warning: `workflows/fetchngs.nf:63:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it.size() > 0 }
                    ^^
  ```

- Warning: `workflows/fetchngs.nf:218:17`: Variable was declared but not used

  ```nextflow
          ).set { ch_collated_versions }
                  ^^^^^^^^^^^^^^^^^^^^
  ```
