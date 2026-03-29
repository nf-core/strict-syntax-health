# Nextflow lint results

- Generated: 2026-03-29T00:25:01.025485026Z
- Nextflow version: 26.03.1-edge
- Summary: 50 errors, 51 warnings

## :x: Errors

- Error: `conf/modules.config:53:55`: `meta` is not defined

  ```nextflow
          ext.prefix = params.perform_runmerging ? { "${meta.id}_${meta.db_name}.fmhfunprofiler" } : { "${meta.id}_${meta.run_accession}_${meta.db_name}.fmhfunprofiler" }
                                                        ^^^^
  ```

- Error: `conf/modules.config:53:66`: `meta` is not defined

  ```nextflow
          ext.prefix = params.perform_runmerging ? { "${meta.id}_${meta.db_name}.fmhfunprofiler" } : { "${meta.id}_${meta.run_accession}_${meta.db_name}.fmhfunprofiler" }
                                                                   ^^^^
  ```

- Error: `conf/modules.config:53:105`: `meta` is not defined

  ```nextflow
          ext.prefix = params.perform_runmerging ? { "${meta.id}_${meta.db_name}.fmhfunprofiler" } : { "${meta.id}_${meta.run_accession}_${meta.db_name}.fmhfunprofiler" }
                                                                                                          ^^^^
  ```

- Error: `conf/modules.config:53:116`: `meta` is not defined

  ```nextflow
          ext.prefix = params.perform_runmerging ? { "${meta.id}_${meta.db_name}.fmhfunprofiler" } : { "${meta.id}_${meta.run_accession}_${meta.db_name}.fmhfunprofiler" }
                                                                                                                     ^^^^
  ```

- Error: `conf/modules.config:53:138`: `meta` is not defined

  ```nextflow
          ext.prefix = params.perform_runmerging ? { "${meta.id}_${meta.db_name}.fmhfunprofiler" } : { "${meta.id}_${meta.run_accession}_${meta.db_name}.fmhfunprofiler" }
                                                                                                                                           ^^^^
  ```

- Error: `modules/local/humann/humann/base.nf:11:5`: Invalid process directive

  ```nextflow
      if (workflow.containerEngine == 'singularity' && !params.singularity_pull_docker_container)	{
      ^
  ```

- Error: `modules/local/humann/humann/base.nf:18:15`: `meta` is already declared

  ```nextflow
      tuple val(meta), path(profile)
                ^^^^
  ```

- Error: `modules/local/humann/regroup/base.nf:10:5`: Invalid process directive

  ```nextflow
      if (workflow.containerEngine == 'singularity' && !params.singularity_pull_docker_container)	{
      ^
  ```

- Error: `modules/local/humann/renorm/main.nf:7:5`: Invalid process directive

  ```nextflow
      if (workflow.containerEngine == 'singularity' && !params.singularity_pull_docker_container) {
      ^
  ```

- Error: `nextflow.config:310:36`: `manifest` is not defined

  ```nextflow
  \033[0;35m  nf-core/funcprofiler ${manifest.version}\033[0m
                                     ^^^^^^^^
  ```

- Error: `nextflow.config:313:26`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                           ^^^^^^^^
  ```

- Error: `nextflow.config:313:69`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                      ^^^^^^^^
  ```

- Error: `nextflow.config:313:186`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                                                                           ^^^^^^^^
  ```

- Error: `nextflow.config:322:22`: `validation` is not defined

  ```nextflow
          beforeText = validation.help.beforeText
                       ^^^^^^^^^^
  ```

- Error: `nextflow.config:323:21`: `validation` is not defined

  ```nextflow
          afterText = validation.help.afterText
                      ^^^^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:6:1`: Included name 'HUMANN3' is not defined in module '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/funcprofiler/modules/local/humann/humann/main.nf'

  ```nextflow
  include { HUMANN3; HUMANN4                              } from '../../modules/local/humann/humann/main'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:6:1`: Included name 'HUMANN4' is not defined in module '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/funcprofiler/modules/local/humann/humann/main.nf'

  ```nextflow
  include { HUMANN3; HUMANN4                              } from '../../modules/local/humann/humann/main'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:7:1`: Included name 'HUMANN3_REGROUP' is not defined in module '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/funcprofiler/modules/local/humann/regroup/main.nf'

  ```nextflow
  include { HUMANN3_REGROUP;HUMANN4_REGROUP              } from '../../modules/local/humann/regroup/main'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:7:1`: Included name 'HUMANN4_REGROUP' is not defined in module '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/funcprofiler/modules/local/humann/regroup/main.nf'

  ```nextflow
  include { HUMANN3_REGROUP;HUMANN4_REGROUP              } from '../../modules/local/humann/regroup/main'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:38:5`: `ch_dbs` was assigned but not declared

  ```nextflow
      ch_dbs = databases
      ^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:50:5`: `reads_with_dbs` was assigned but not declared

  ```nextflow
      reads_with_dbs = pairedreads
      ^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:55:18`: `ch_dbs` is not defined

  ```nextflow
          .combine(ch_dbs, by: 0)
                   ^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:61:16`: `reads_with_dbs` is not defined

  ```nextflow
          return reads_with_dbs
                 ^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:76:16`: `reads_with_dbs` is not defined

  ```nextflow
          return reads_with_dbs
                 ^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:171:23`: `reads` is already declared

  ```nextflow
                  meta, reads, db_meta, db ->
                        ^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:192:23`: `reads` is already declared

  ```nextflow
                  meta, reads, db_meta, db ->
                        ^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:210:9`: `reads` is already declared

  ```nextflow
  		meta, reads, db_meta, db ->
          ^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:227:13`: `HUMANN3` is not defined

  ```nextflow
              HUMANN3 ( ch_input_for_humann.reads, MPAHUMANN3.out.profile, ch_input_for_humann.nuc_db, ch_input_for_humann.prot_db, ch_input_for_humann.util_db
              ^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:229:6`: `HUMANN3_REGROUP` is not defined

  ```nextflow
  	    HUMANN3_REGROUP(HUMANN3.out.genefamilies, "uniref90_level4ec", ch_input_for_humann.util_db)
       ^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:229:22`: `HUMANN3` is not defined

  ```nextflow
  	    HUMANN3_REGROUP(HUMANN3.out.genefamilies, "uniref90_level4ec", ch_input_for_humann.util_db)
                       ^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:237:55`: `HUMANN3` is not defined

  ```nextflow
          ch_raw_profiles        = ch_raw_profiles.mix( HUMANN3.out.pathabundance )
                                                        ^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:238:12`: `HUMANN3` is not defined

  ```nextflow
  	    .mix( HUMANN3.out.genefamilies )
             ^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:239:12`: `HUMANN3` is not defined

  ```nextflow
  	    .mix( HUMANN3.out.pathcoverage )
             ^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:244:9`: `reads` is already declared

  ```nextflow
  		meta, reads, db_meta, db ->
          ^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:261:13`: `HUMANN4` is not defined

  ```nextflow
              HUMANN4 ( ch_input_for_humann4.reads, MPAHUMANN4.out.profile, ch_input_for_humann4.nuc_db, ch_input_for_humann4.prot_db, ch_input_for_humann4.util_db)
              ^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:262:6`: `HUMANN4_REGROUP` is not defined

  ```nextflow
  	    HUMANN4_REGROUP(HUMANN4.out.genefamilies, "uniclust90_level4ec", ch_input_for_humann4.util_db)
       ^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:262:22`: `HUMANN4` is not defined

  ```nextflow
  	    HUMANN4_REGROUP(HUMANN4.out.genefamilies, "uniclust90_level4ec", ch_input_for_humann4.util_db)
                       ^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:268:55`: `HUMANN4` is not defined

  ```nextflow
          ch_raw_profiles        = ch_raw_profiles.mix( HUMANN4.out.pathabundance )
                                                        ^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:269:12`: `HUMANN4` is not defined

  ```nextflow
  	    .mix( HUMANN4.out.genefamilies )
             ^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:270:12`: `HUMANN4` is not defined

  ```nextflow
  	    .mix( HUMANN4.out.reactions )
             ^^^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:276:23`: `reads` is already declared

  ```nextflow
                  meta, reads, db_meta, db ->
                        ^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:294:23`: `reads` is already declared

  ```nextflow
                  meta, reads, db_meta, db ->
                        ^^^^^
  ```

- Error: `subworkflows/local/profiling.nf:307:23`: `reads` is already declared

  ```nextflow
                  meta, reads, db_meta, db ->
                        ^^^^^
  ```

- Error: `workflows/funcprofiler.nf:14:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  def checkPathParamList = [ params.input, params.databases,
  ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/funcprofiler.nf:22:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  checkPathParamList.each{param ->
  ^
  ```

- Error: `workflows/funcprofiler.nf:27:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  if ( params.input ) {
  ^
  ```

- Error: `workflows/funcprofiler.nf:33:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  if (params.databases) { ch_databases = file(params.databases, checkIfExists: true) } else { error('Input database sheet not specified!') }
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/funcprofiler.nf:178:38`: `SHORTREAD_PREPROCESSING` is not defined

  ```nextflow
          ch_shortreads_preprocessed = SHORTREAD_PREPROCESSING ( ch_input.fastq, adapterlist ).reads
                                       ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/funcprofiler.nf:178:80`: `adapterlist` is not defined

  ```nextflow
          ch_shortreads_preprocessed = SHORTREAD_PREPROCESSING ( ch_input.fastq, adapterlist ).reads
                                                                                 ^^^^^^^^^^^
  ```

- Error: `workflows/funcprofiler.nf:179:40`: `SHORTREAD_PREPROCESSING` is not defined

  ```nextflow
          ch_versions = ch_versions.mix( SHORTREAD_PREPROCESSING.out.versions )
                                         ^^^^^^^^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/humann/humann/base.nf:17:15`: Variable was declared but not used

  ```nextflow
      tuple val(meta), path(input)
                ^^^^
  ```

- Warning: `modules/local/humann/regroup/base.nf:49:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/humann/renorm/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/humann/utils.nf:32:5`: The `shell` block is deprecated, use `script` instead

  ```nextflow
      shell: """echo x3 """
      ^^^^^
  ```

- Warning: `modules/local/humann/utils.nf:38:5`: The `shell` block is deprecated, use `script` instead

  ```nextflow
      shell: """echo x4 """
      ^^^^^
  ```

- Warning: `nextflow.config:313:129`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                  ^^
  ```

- Warning: `subworkflows/local/profiling.nf:57:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              db_type, meta, reads, db_meta, db ->
              ^^^^^^^
  ```

- Warning: `subworkflows/local/profiling.nf:62:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, reads, db_meta, db ->
                    ^^^^
  ```

- Warning: `subworkflows/local/profiling.nf:62:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, reads, db_meta, db ->
                          ^^^^^
  ```

- Warning: `subworkflows/local/profiling.nf:62:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, reads, db_meta, db ->
                                          ^^
  ```

- Warning: `subworkflows/local/profiling.nf:85:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  	    .branch { meta, reads, db_meta, db ->
                 ^^^^
  ```

- Warning: `subworkflows/local/profiling.nf:85:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  	    .branch { meta, reads, db_meta, db ->
                       ^^^^^
  ```

- Warning: `subworkflows/local/profiling.nf:85:38`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  	    .branch { meta, reads, db_meta, db ->
                                       ^^
  ```

- Warning: `subworkflows/local/profiling.nf:147:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions             = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/profiling.nf:148:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files        = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/profiling.nf:149:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_raw_profiles         = Channel.empty() // These are count tables
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/profiling.nf:219:24`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  		mpa_db: db.findAll { it.db_entity == "humann_metaphlan" }.first().db_path
                         ^^
  ```

- Warning: `subworkflows/local/profiling.nf:220:24`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  		nuc_db: db.findAll { it.db_entity == "humann_nucleotide" }.first().db_path
                         ^^
  ```

- Warning: `subworkflows/local/profiling.nf:221:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  		prot_db: db.findAll { it.db_entity == "humann_protein" }.first().db_path
                          ^^
  ```

- Warning: `subworkflows/local/profiling.nf:222:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  		util_db: db.findAll { it.db_entity == "humann_utility" }.first().db_path
                          ^^
  ```

- Warning: `subworkflows/local/profiling.nf:253:24`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  		mpa_db: db.findAll { it.db_entity == "humann_metaphlan" }.first().db_path
                         ^^
  ```

- Warning: `subworkflows/local/profiling.nf:254:24`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  		nuc_db: db.findAll { it.db_entity == "humann_nucleotide" }.first().db_path
                         ^^
  ```

- Warning: `subworkflows/local/profiling.nf:255:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  		prot_db: db.findAll { it.db_entity == "humann_protein" }.first().db_path
                          ^^
  ```

- Warning: `subworkflows/local/profiling.nf:256:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
  		util_db: db.findAll { it.db_entity == "humann_utility" }.first().db_path
                          ^^
  ```

- Warning: `subworkflows/local/profiling.nf:314:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  search_db: db.findAll { it.db_entity == "eggnogmapper_db" }.first().db_path
                                          ^^
  ```

- Warning: `subworkflows/local/profiling.nf:315:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  data_dir:  db.findAll { it.db_entity == "eggnogmapper_data_dir" }.first().db_path
                                          ^^
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
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_funcprofiler_pipeline/main.nf:108:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_funcprofiler_pipeline/main.nf:131:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      hook_url //  string: hook URL for notifications
      ^^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:28:5`: Variable was declared but not used

  ```nextflow
      ch_input              = file(params.input, checkIfExists: true)
      ^^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:33:25`: Variable was declared but not used

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

- Warning: `workflows/funcprofiler.nf:101:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, run_accession, instrument_platform, fastq_1, fastq_2, fasta ->
                          ^^^^^^^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:116:5`: Variable was declared but not used

  ```nextflow
      ch_input_for_fastqc = ch_input.fastq.mix( ch_input.nanopore )
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:130:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { db_meta, db_path ->
                             ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:183:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_longreads_preprocessed = Channel.empty()
                                  ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:240:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_config        = Channel.fromPath(
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:240:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_config        = Channel.fromPath(
                                 ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:242:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_custom_config = params.multiqc_config ?
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:243:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath(params.multiqc_config, checkIfExists: true) :
          ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:244:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.empty()
          ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:245:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_logo          = params.multiqc_logo ?
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:246:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath(params.multiqc_logo, checkIfExists: true) :
          ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:247:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.empty()
          ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:251:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_workflow_summary = Channel.value(paramsSummaryMultiqc(summary_params))
                            ^^^^^^^
  ```

- Warning: `workflows/funcprofiler.nf:257:45`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_methods_description                = Channel.value(
                                              ^^^^^^^
  ```
