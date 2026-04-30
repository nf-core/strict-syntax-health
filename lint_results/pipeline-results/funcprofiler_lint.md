# Nextflow lint results

- Generated: 2026-04-30T00:38:16.221130157Z
- Nextflow version: 26.04.0
- Summary: 26 errors, 42 warnings

## :x: Errors

- Error: `conf/modules.config:59:55`: `meta` is not defined

  ```nextflow
          ext.prefix = params.perform_runmerging ? { "${meta.id}_${meta.db_name}.fmhfunprofiler" } : { "${meta.id}_${meta.run_accession}_${meta.db_name}.fmhfunprofiler" }
                                                        ^^^^
  ```

- Error: `conf/modules.config:59:66`: `meta` is not defined

  ```nextflow
          ext.prefix = params.perform_runmerging ? { "${meta.id}_${meta.db_name}.fmhfunprofiler" } : { "${meta.id}_${meta.run_accession}_${meta.db_name}.fmhfunprofiler" }
                                                                   ^^^^
  ```

- Error: `conf/modules.config:59:105`: `meta` is not defined

  ```nextflow
          ext.prefix = params.perform_runmerging ? { "${meta.id}_${meta.db_name}.fmhfunprofiler" } : { "${meta.id}_${meta.run_accession}_${meta.db_name}.fmhfunprofiler" }
                                                                                                          ^^^^
  ```

- Error: `conf/modules.config:59:116`: `meta` is not defined

  ```nextflow
          ext.prefix = params.perform_runmerging ? { "${meta.id}_${meta.db_name}.fmhfunprofiler" } : { "${meta.id}_${meta.run_accession}_${meta.db_name}.fmhfunprofiler" }
                                                                                                                     ^^^^
  ```

- Error: `conf/modules.config:59:138`: `meta` is not defined

  ```nextflow
          ext.prefix = params.perform_runmerging ? { "${meta.id}_${meta.db_name}.fmhfunprofiler" } : { "${meta.id}_${meta.run_accession}_${meta.db_name}.fmhfunprofiler" }
                                                                                                                                           ^^^^
  ```

- Error: `modules/local/humann/humann/main.nf:14:15`: `meta` is already declared

  ```nextflow
      tuple val(meta), path(profile)
                ^^^^
  ```

- Error: `modules/local/humann4/humann/main.nf:11:15`: `meta` is already declared

  ```nextflow
      tuple val(meta), path(profile)
                ^^^^
  ```

- Error: `nextflow.config:314:36`: `manifest` is not defined

  ```nextflow
  \033[0;35m  nf-core/funcprofiler ${manifest.version}\033[0m
                                     ^^^^^^^^
  ```

- Error: `nextflow.config:317:26`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                           ^^^^^^^^
  ```

- Error: `nextflow.config:317:69`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                      ^^^^^^^^
  ```

- Error: `nextflow.config:317:186`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                                                                           ^^^^^^^^
  ```

- Error: `nextflow.config:326:22`: `validation` is not defined

  ```nextflow
          beforeText = validation.help.beforeText
                       ^^^^^^^^^^
  ```

- Error: `nextflow.config:327:21`: `validation` is not defined

  ```nextflow
          afterText = validation.help.afterText
                      ^^^^^^^^^^
  ```

- Error: `subworkflows/local/profile/main.nf:202:42`: `reads` is already declared

  ```nextflow
              ch_humann3_input.map { meta, reads, profile -> [meta, reads] },  // Extract reads
                                           ^^^^^
  ```

- Error: `subworkflows/local/profile/main.nf:203:42`: `reads` is already declared

  ```nextflow
              ch_humann3_input.map { meta, reads, profile -> [meta, profile] }, // Extract profile
                                           ^^^^^
  ```

- Error: `subworkflows/local/profile/main.nf:223:42`: `reads` is already declared

  ```nextflow
              ch_humann4_input.map { meta, reads, profile -> [meta, reads] },  // Extract reads
                                           ^^^^^
  ```

- Error: `subworkflows/local/profile/main.nf:224:42`: `reads` is already declared

  ```nextflow
              ch_humann4_input.map { meta, reads, profile -> [meta, profile] }, // Extract profile
                                           ^^^^^
  ```

- Error: `subworkflows/local/profile/main.nf:241:18`: `ch_input_for_rgi` is not defined

  ```nextflow
          RGI_BWT( ch_input_for_rgi.reads, getDbPath(ch_input_for_rgi.db, "main"), [] )
                   ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/profile/main.nf:241:52`: `ch_input_for_rgi` is not defined

  ```nextflow
          RGI_BWT( ch_input_for_rgi.reads, getDbPath(ch_input_for_rgi.db, "main"), [] )
                                                     ^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/profile/main.nf:245:15`: `ch_input_for_eggnogmapper` is not defined

  ```nextflow
  	SEQKIT_FQ2FA(ch_input_for_eggnogmapper.reads)
                ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/profile/main.nf:249:16`: `ch_input_for_eggnogmapper` is not defined

  ```nextflow
  	    getDbPath(ch_input_for_eggnogmapper.db, "eggnogmapper_db"),
                 ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/profile/main.nf:250:16`: `ch_input_for_eggnogmapper` is not defined

  ```nextflow
  	    getDbPath(ch_input_for_eggnogmapper.db, "")
                 ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/funcprofiler.nf:13:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  def checkPathParamList = [ params.input, params.databases,
  ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/funcprofiler.nf:21:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  checkPathParamList.each{param ->
  ^
  ```

- Error: `workflows/funcprofiler.nf:26:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  if ( params.input ) {
  ^
  ```

- Error: `workflows/funcprofiler.nf:32:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  if (params.databases) { ch_databases = file(params.databases, checkIfExists: true) } else { error('Input database sheet not specified!') }
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/humann/humann/main.nf:13:15`: Variable was declared but not used

  ```nextflow
      tuple val(meta), path(input)
                ^^^^
  ```

- Warning: `modules/local/humann/regroup/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/humann/renorm/main.nf:35:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/humann4/humann/main.nf:10:15`: Variable was declared but not used

  ```nextflow
      tuple val(meta), path(input)
                ^^^^
  ```

- Warning: `modules/local/humann4/regroup/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/humann4/renorm/main.nf:35:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `nextflow.config:317:129`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                  ^^
  ```

- Warning: `subworkflows/local/concatall.nf:26:5`: Variable was declared but not used

  ```nextflow
      ch_input_reads_merged = CAT_FASTQ(ch_input_singlefq.cat).reads
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

- Warning: `subworkflows/local/profile/main.nf:170:5`: Variable was declared but not used

  ```nextflow
      rgi_inputs = prepareInputs(reads, databases, 'rgi', false)
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/profile/main.nf:202:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_humann3_input.map { meta, reads, profile -> [meta, reads] },  // Extract reads
                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/profile/main.nf:203:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_humann3_input.map { meta, reads, profile -> [meta, profile] }, // Extract profile
                                           ^^^^^
  ```

- Warning: `subworkflows/local/profile/main.nf:223:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_humann4_input.map { meta, reads, profile -> [meta, reads] },  // Extract reads
                                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/profile/main.nf:224:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_humann4_input.map { meta, reads, profile -> [meta, profile] }, // Extract profile
                                           ^^^^^
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

- Warning: `subworkflows/local/utils_nfcore_funcprofiler_pipeline/main.nf:42:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_funcprofiler_pipeline/main.nf:101:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.fromList(samplesheetToList(params.input, "assets/schema_input.json"))
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_funcprofiler_pipeline/main.nf:107:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.fromList(samplesheetToList(params.databases, "assets/schema_database.json"))
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_funcprofiler_pipeline/main.nf:129:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      hook_url //  string: hook URL for notifications
      ^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:27:5`: Variable was declared but not used

  ```nextflow
      ch_input              = file(params.input, checkIfExists: true)
      ^^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:32:25`: Variable was declared but not used

  ```nextflow
  if (params.databases) { ch_databases = file(params.databases, checkIfExists: true) } else { error('Input database sheet not specified!') }
                          ^^^^^^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:75:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:76:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:105:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_config        = Channel.fromPath(
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:105:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_config        = Channel.fromPath(
                                 ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:107:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_custom_config = params.multiqc_config ?
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:108:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath(params.multiqc_config, checkIfExists: true) :
          ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:109:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.empty()
          ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:110:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_logo          = params.multiqc_logo ?
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:111:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath(params.multiqc_logo, checkIfExists: true) :
          ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:112:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.empty()
          ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:116:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_workflow_summary = Channel.value(paramsSummaryMultiqc(summary_params))
                            ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:122:45`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_methods_description                = Channel.value(
                                              ^^^^^^^
  ```
