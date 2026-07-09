# Nextflow lint results

- Generated: 2026-07-09T00:32:33.725224746Z
- Nextflow version: 26.06.0-edge
- Summary: 9 warnings

## :warning: Warnings

- Warning: `main.nf:50:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = DATASYNC.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/comparechecksum/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/comparechecksum/main.nf:27:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
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

- Warning: `workflows/datasync.nf:95:78`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(COMPARECHECKSUM.out.report.map { meta, report -> report })
                                                                               ^^^^
  ```

- Warning: `workflows/datasync.nf:96:86`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(COMPARECHECKSUM.out.summary_report.map { meta, summary -> summary })
                                                                                       ^^^^
  ```

- Warning: `workflows/datasync.nf:138:45`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(Channel.fromPath(params.input).collectFile(name: 'samplesheet.csv'))
                                              ^^^^^^^
  ```
