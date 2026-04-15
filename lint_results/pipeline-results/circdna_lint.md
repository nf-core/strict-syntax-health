# Nextflow lint results

- Generated: 2026-04-15T00:30:37.985074848Z
- Nextflow version: 26.03.2-edge
- Summary: 22 errors, 25 warnings

## :x: Errors

- Error: `conf/base.config:53:20`: `check_max` is not defined

  ```nextflow
          time   = { check_max( max_time, 'time'    ) }
                     ^^^^^^^^^
  ```

- Error: `conf/base.config:60:20`: `check_max` is not defined

  ```nextflow
          cpus   = { check_max( params.max_cpus, 'cpus'    ) }
                     ^^^^^^^^^
  ```

- Error: `conf/base.config:61:20`: `check_max` is not defined

  ```nextflow
          memory = { check_max( params.max_memory, 'memory'  ) }
                     ^^^^^^^^^
  ```

- Error: `conf/base.config:62:20`: `check_max` is not defined

  ```nextflow
          time   = { check_max( max_time, 'time'    ) }
                     ^^^^^^^^^
  ```

- Error: `conf/modules.config:73:1`: If statements cannot be mixed with config statements

  ```nextflow
  if(!params.skip_qc) {
  ^
  ```

- Error: `conf/modules.config:520:1`: If statements cannot be mixed with config statements

  ```nextflow
  if (!params.skip_multiqc) {
  ^
  ```

- Error: `main.nf:18:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/circdna/workflows/circdna.nf'

  ```nextflow
  include { CIRCDNA  } from './workflows/circdna'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:53:5`: `CIRCDNA` is not defined

  ```nextflow
      CIRCDNA (
      ^^^^^^^
  ```

- Error: `main.nf:57:22`: `CIRCDNA` is not defined

  ```nextflow
      multiqc_report = CIRCDNA.out.multiqc_report // channel: /path/to/multiqc_report.html
                       ^^^^^^^
  ```

- Error: `modules/local/circexplorer2/parse.nf:6:5`: Invalid process directive

  ```nextflow
      if (workflow.containerEngine == 'singularity' && !params.singularity_pull_docker_container) {
      ^
  ```

- Error: `modules/nf-core/samtools/view/main.nf:64:9`: `index` is already declared

  ```nextflow
      def index = args.contains("--write-index") ? "touch ${prefix}.csi" : ""
          ^^^^^
  ```

- Error: `nextflow.config:342:31`: `manifest` is not defined

  ```nextflow
  \033[0;35m  nf-core/circdna ${manifest.version}\033[0m
                                ^^^^^^^^
  ```

- Error: `nextflow.config:345:26`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                           ^^^^^^^^
  ```

- Error: `nextflow.config:345:69`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                      ^^^^^^^^
  ```

- Error: `nextflow.config:345:186`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                                                                           ^^^^^^^^
  ```

- Error: `nextflow.config:354:22`: `validation` is not defined

  ```nextflow
          beforeText = validation.help.beforeText
                       ^^^^^^^^^^
  ```

- Error: `nextflow.config:355:21`: `validation` is not defined

  ```nextflow
          afterText = validation.help.afterText
                      ^^^^^^^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_circdna_pipeline/main.nf:95:20`: `parseBoolean` is not defined

  ```nextflow
              return parseBoolean(value[0])
                     ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_circdna_pipeline/main.nf:105:25`: `parseBoolean` is not defined

  ```nextflow
                      if (parseBoolean(bam)) {
                          ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_circdna_pipeline/main.nf:108:41`: `parseBoolean` is not defined

  ```nextflow
                      def is_single_end = parseBoolean(single_end) != null ? parseBoolean(single_end) : !fastq_2
                                          ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_circdna_pipeline/main.nf:108:76`: `parseBoolean` is not defined

  ```nextflow
                      def is_single_end = parseBoolean(single_end) != null ? parseBoolean(single_end) : !fastq_2
                                                                             ^^^^^^^^^^^^
  ```

- Error: `workflows/circdna.nf:326:21`: Unexpected input: 'map'

  ```nextflow
                      map { meta, bam, bai -> [meta, bam, bai] },
                      ^
  ```

## :warning: Warnings

- Warning: `modules/local/ampliconsuite/ampliconsuite.nf:34:9`: Variable was declared but not used

  ```nextflow
      def cngain = params.aa_cngain
          ^^^^^^
  ```

- Warning: `modules/local/ampliconsuite/ampliconsuite.nf:65:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/ampliconsuite/ampliconsuite.nf:67:9`: Variable was declared but not used

  ```nextflow
      def cngain = params.aa_cngain
          ^^^^^^
  ```

- Warning: `modules/local/ampliconsuite/ampliconsuite.nf:68:9`: Variable was declared but not used

  ```nextflow
      def ref = params.reference_build
          ^^^
  ```

- Warning: `modules/local/bwa/mem/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/bwa/mem/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args2 = task.ext.args2 ?: ''
          ^^^^^
  ```

- Warning: `modules/local/bwa/mem/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def samtools_command = sort_bam ? 'sort' : 'view'
          ^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/circlefinder.nf:16:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/circlemap/readextractor.nf:18:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/getcircularreads.nf:15:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/samtools/flagstat/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/samtools/idxstats/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/custom/dumpsoftwareversions/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:62:9`: Variable was declared but not used

  ```nextflow
      def target = reference ?: (bam_input ? error("BAM input requires reference") : reads)
          ^^^^^^
  ```

- Warning: `nextflow.config:345:129`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                  ^^
  ```

- Warning: `subworkflows/local/input_check.nf:16:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { create_fastq_channels(it) }
                                           ^^
  ```

- Warning: `subworkflows/local/input_check.nf:22:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { create_bam_channels(it) }
                                         ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_circdna_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_circdna_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_circdna_pipeline/main.nf:38:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_circdna_pipeline/main.nf:81:9`: Variable was declared but not used

  ```nextflow
      def parseBoolean = { value ->
          ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_circdna_pipeline/main.nf:101:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel
          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_circdna_pipeline/main.nf:125:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel
          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_circdna_pipeline/main.nf:136:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { id, metas, bams ->
                     ^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```
