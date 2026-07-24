# Nextflow lint results

- Generated: 2026-07-24T00:27:09.374716074Z
- Nextflow version: 26.07.0-edge
- Summary: 19 warnings

## :warning: Warnings

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

- Warning: `subworkflows/local/dataprep/main.nf:45:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { group_key, meta_list, reads_list ->
                 ^^^^^^^^^
  ```

- Warning: `subworkflows/local/dbprep/main.nf:10:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_dbs_for_untar = databases.branch { db_meta, db_path ->
                                            ^^^^^^^
  ```

- Warning: `subworkflows/local/dbprep/main.nf:17:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { db_meta, db_path ->
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/profile/main.nf:63:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  	.filter { meta_db, file ->
                      ^^^^
  ```

- Warning: `subworkflows/local/profile/main.nf:157:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions             = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/profile/main.nf:158:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files        = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/profile/main.nf:159:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

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

- Warning: `workflows/funcprofiler.nf:58:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:59:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```
