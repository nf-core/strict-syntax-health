# Nextflow lint results

- Generated: 2026-05-19T00:39:55.756432572Z
- Nextflow version: 26.04.1
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_hlatyping_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_hlatyping_pipeline/main.nf:357:92`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def actual = file.withInputStream { org.apache.commons.codec.digest.DigestUtils.md5Hex(it) }
                                                                                             ^^
  ```
