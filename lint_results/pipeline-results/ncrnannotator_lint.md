# Nextflow lint results

- Generated: 2026-06-16T14:25:01.020436798Z
- Nextflow version: 26.04.3
- Summary: 10 warnings

## :warning: Warnings

- Warning: `main.nf:37:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = NCRNANNOTATOR.out.multiqc_report
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ncrnannotator_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ncrnannotator_pipeline/main.nf:99:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions = ch_versions
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ncrnannotator_pipeline/main.nf:180:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              errors.collect { "    * ${it}" }.join("\n") + "\n" +
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

- Warning: `workflows/ncrnannotator.nf:90:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          CMSEARCH.out.tblout.collect { it[1] },
                                        ^^
  ```

- Warning: `workflows/ncrnannotator.nf:105:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
