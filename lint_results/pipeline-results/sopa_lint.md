# Nextflow lint results

- Generated: 2026-09-17T00:23:40.045303154Z
- Nextflow version: 26.08.0-edge
- Summary: 12 warnings

## :warning: Warnings

- Warning: `modules/local/utils.nf:23:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          return "[" + value.collect { stringifyValueForCli(it) }.join(", ") + "]"
                                                            ^^
  ```

- Warning: `modules/local/utils.nf:194:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          return channels.split(/[ ,|]+/).findAll { it }
                                                    ^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:23:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              tar: it[1].name.contains(".gz")
                   ^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:24:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              dir: !it[1].name.contains(".gz")
                    ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_sopa_pipeline/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_sopa_pipeline/main.nf:104:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_sopa_pipeline/main.nf:279:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def enabled = ALL_METHODS.findAll { params[it] }
                                                ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_sopa_pipeline/main.nf:280:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def enabled_transcript = TRANSCRIPT_BASED_METHODS.findAll { params[it] }
                                                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_sopa_pipeline/main.nf:281:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def enabled_staining = STAINING_BASED_METHODS.findAll { params[it] }
                                                                    ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_sopa_pipeline/main.nf:323:93`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          error("Invalid combination of nf-core/sopa parameters:\n" + errors.collect { "  - ${it}" }.join("\n") + "\nSee https://nf-co.re/sopa/docs/usage/ for the supported configurations.")
                                                                                              ^^
  ```

- Warning: `workflows/sopa.nf:159:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```
