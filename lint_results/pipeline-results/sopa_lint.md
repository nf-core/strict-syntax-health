# Nextflow lint results

- Generated: 2026-03-21T00:24:38.288890772Z
- Nextflow version: 26.03.0-edge
- Summary: 7 errors, 13 warnings

## :x: Errors

- Error: `modules/nf-core/spaceranger/count/main.nf:27:9`: `probeset` is already declared

  ```nextflow
      def probeset = probeset ? "--probe-set=\"${probeset}\"" : ""
          ^^^^^^^^
  ```

- Error: `modules/nf-core/spaceranger/count/main.nf:28:9`: `alignment` is already declared

  ```nextflow
      def alignment = alignment ? "--loupe-alignment=\"${alignment}\"" : ""
          ^^^^^^^^^
  ```

- Error: `modules/nf-core/spaceranger/count/main.nf:29:9`: `slidefile` is already declared

  ```nextflow
      def slidefile = slidefile ? "--slidefile=\"${slidefile}\"" : ""
          ^^^^^^^^^
  ```

- Error: `modules/nf-core/spaceranger/count/main.nf:30:9`: `image` is already declared

  ```nextflow
      def image = image ? "--image=\"${image}\"" : ""
          ^^^^^
  ```

- Error: `modules/nf-core/spaceranger/count/main.nf:31:9`: `cytaimage` is already declared

  ```nextflow
      def cytaimage = cytaimage ? "--cytaimage=\"${cytaimage}\"" : ""
          ^^^^^^^^^
  ```

- Error: `modules/nf-core/spaceranger/count/main.nf:32:9`: `darkimage` is already declared

  ```nextflow
      def darkimage = darkimage ? "--darkimage=\"${darkimage}\"" : ""
          ^^^^^^^^^
  ```

- Error: `modules/nf-core/spaceranger/count/main.nf:33:9`: `colorizedimage` is already declared

  ```nextflow
      def colorizedimage = colorizedimage ? "--colorizedimage=\"${colorizedimage}\"" : ""
          ^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/utils.nf:23:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          return "[" + value.collect { stringifyValueForCli(it) }.join(", ") + "]"
                                                            ^^
  ```

- Warning: `modules/local/utils.nf:185:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

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

- Warning: `subworkflows/local/utils_nfcore_sopa_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_sopa_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_sopa_pipeline/main.nf:98:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_sopa_pipeline/main.nf:274:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      assert TRANSCRIPT_BASED_METHODS.count { params[it] } <= 1 : "Only one of ${TRANSCRIPT_BASED_METHODS} may be used"
                                                    ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_sopa_pipeline/main.nf:275:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      assert STAINING_BASED_METHODS.count { params[it] } <= 1 : "Only one of ${STAINING_BASED_METHODS} may be used"
                                                  ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_sopa_pipeline/main.nf:277:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          assert NON_VALID_STARDIST_METHODS.every { !params[it] } : "'stardist' cannot be combined with transcript-based methods, except proseg."
                                                           ^^
  ```

- Warning: `workflows/sopa.nf:151:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```

- Warning: `workflows/sopa.nf:175:17`: Variable was declared but not used

  ```nextflow
          ).set { ch_collated_versions }
                  ^^^^^^^^^^^^^^^^^^^^
  ```
