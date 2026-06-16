# Nextflow lint results

- Generated: 2026-06-16T19:37:24.527073647Z
- Nextflow version: 26.04.3
- Summary: 6 warnings

## :warning: Warnings

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

- Warning: `workflows/provenancereport.nf:19:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_samplesheet // channel: samplesheet read in from --input
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/provenancereport.nf:46:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/provenancereport.nf:55:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions       = ch_versions                 // channel: [ path(versions.yml) ]
      ^^^^^^^^^^^^^^^^^^^^
  ```
