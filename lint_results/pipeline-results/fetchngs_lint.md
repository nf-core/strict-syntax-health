# Nextflow lint results

- Generated: 2026-04-29T00:36:16.598245563Z
- Nextflow version: 26.03.4-edge
- Summary: 9 warnings

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

- Warning: `subworkflows/local/utils_nfcore_fetchngs_pipeline/main.nf:202:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def actual_ena_metadata_fields = ena_metadata_fields ? ena_metadata_fields.split(',').collect { it.trim().toLowerCase() } : valid_ena_metadata_fields
                                                                                                      ^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/fetchngs.nf:217:17`: Variable was declared but not used

  ```nextflow
          ).set { ch_collated_versions }
                  ^^^^^^^^^^^^^^^^^^^^
  ```
