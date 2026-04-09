# Nextflow lint results

- Generated: 2026-04-09T00:22:07.317820354Z
- Nextflow version: 26.03.2-edge
- Summary: 11 errors, 25 warnings

## :x: Errors

- Error: `main.nf:8:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/panoramaseq/workflows/panoramaseq.nf'

  ```nextflow
  include { PANORAMASEQ } from './workflows/panoramaseq'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:80:5`: `PANORAMASEQ` is not defined

  ```nextflow
      PANORAMASEQ(
      ^^^^^^^^^^^
  ```

- Error: `main.nf:87:22`: `PANORAMASEQ` is not defined

  ```nextflow
      multiqc_report = PANORAMASEQ.out.multiqc_report // channel: /path/to/multi
                       ^^^^^^^^^^^
  ```

- Error: `main.nf:88:38`: `PANORAMASEQ` is not defined

  ```nextflow
      versions       = ch_versions.mix(PANORAMASEQ.out.versions)
                                       ^^^^^^^^^^^
  ```

- Error: `nextflow.config:297:35`: `manifest` is not defined

  ```nextflow
  \033[0;35m  nf-core/panoramaseq ${manifest.version}\033[0m
                                    ^^^^^^^^
  ```

- Error: `nextflow.config:300:26`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                           ^^^^^^^^
  ```

- Error: `nextflow.config:300:69`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                      ^^^^^^^^
  ```

- Error: `nextflow.config:300:186`: `manifest` is not defined

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                                                                           ^^^^^^^^
  ```

- Error: `nextflow.config:309:22`: `validation` is not defined

  ```nextflow
          beforeText = validation.help.beforeText
                       ^^^^^^^^^^
  ```

- Error: `nextflow.config:310:21`: `validation` is not defined

  ```nextflow
          afterText = validation.help.afterText
                      ^^^^^^^^^^
  ```

- Error: `workflows/panoramaseq.nf:198:26`: Unexpected input: 'i'

  ```nextflow
                  for (int i = 0; i < items.size(); i += 2) {
                           ^
  ```

## :warning: Warnings

- Warning: `main.nf:27:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `main.nf:70:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_star_index = Channel.value(file(params.star_genome_dir, checkIfExists: true))
                          ^^^^^^^
  ```

- Warning: `main.nf:71:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gtf_file = Channel.value(file(params.star_gtf, checkIfExists: true))
                        ^^^^^^^
  ```

- Warning: `main.nf:107:94`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      PIPELINE_INITIALISATION.out.samplesheet.view { "PIPELINE_INITIALISATION.out.samplesheet: $it" }
                                                                                               ^^
  ```

- Warning: `modules/local/quik/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `nextflow.config:300:129`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                  ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:24:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fasta_input = Channel.value([[:], fasta])
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:26:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fasta = GUNZIP_FASTA.out.gunzip.map { meta, file -> file }
                                                   ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:29:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fasta = Channel.value(fasta)
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:36:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gtf_input = Channel.value([[:], gtf])
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:38:46`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_gtf = GUNZIP_GTF.out.gunzip.map { meta, file -> file }
                                               ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:41:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gtf = Channel.value(gtf)
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:52:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_additional_input = Channel.value([[:], additional_fasta])
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:54:70`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_additional_fasta = GUNZIP_ADDITIONAL.out.gunzip.map { meta, file -> file }
                                                                       ^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:57:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_additional_fasta = Channel.value(additional_fasta)
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:71:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_final_fasta.map { [ [:], it ] },
                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:72:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_gtf.map         { [ [:], it ] }
                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome/main.nf:79:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      index     = STAR_GENOMEGENERATE.out.index.map { it[1] } // path: STAR genome index directory
                                                      ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_panoramaseq_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_panoramaseq_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_panoramaseq_pipeline/main.nf:38:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_panoramaseq_pipeline/main.nf:81:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```
