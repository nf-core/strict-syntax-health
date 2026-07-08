# Nextflow lint results

- Generated: 2026-07-08T00:28:45.603879935Z
- Nextflow version: 26.06.0-edge
- Summary: 28 warnings

## :warning: Warnings

- Warning: `main.nf:51:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = FUNCPROFILER.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `main.nf:76:9`: Variable was declared but not used

  ```nextflow
      def profileUsesContainers = (workflow.containerEngine != null && workflow.containerEngine != '')
          ^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/humann4/regroup/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/humann4/renorm/main.nf:35:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/humann3/renorm/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/concatall.nf:26:5`: Variable was declared but not used

  ```nextflow
      ch_input_reads_merged = CAT_FASTQ(ch_input_singlefq.cat).reads
      ^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/concatall.nf:31:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      ch_input_reads_merged
      ^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/dataprep/main.nf:46:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { group_key, meta_list, reads_list ->
                 ^^^^^^^^^
  ```

- Warning: `subworkflows/local/dbprep/main.nf:12:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_dbs_for_untar = databases.branch { db_meta, db_path ->
                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/dbprep/main.nf:19:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { db_meta, db_path ->
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/dbprep/main.nf:61:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dbs = ch_grouped_dbs
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/profile/main.nf:64:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  	.filter { meta_db, file ->
                      ^^^^
  ```

- Warning: `subworkflows/local/profile/main.nf:158:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions             = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/profile/main.nf:159:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files        = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/profile/main.nf:160:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_raw_profiles         = Channel.empty() // These are count tables
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_funcprofiler_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_funcprofiler_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_funcprofiler_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      databases //  string: Path to databases
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_funcprofiler_pipeline/main.nf:102:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.fromList(samplesheetToList(params.input, "assets/schema_input.json"))
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_funcprofiler_pipeline/main.nf:108:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.fromList(samplesheetToList(params.databases, "assets/schema_database.json"))
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_funcprofiler_pipeline/main.nf:130:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      hook_url //  string: hook URL for notifications
      ^^^^^^^^
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

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:76:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:50:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      multiqc_config
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:51:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      multiqc_logo
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:57:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:58:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```
