# Nextflow lint results

- Generated: 2026-05-13T00:41:04.204243973Z
- Nextflow version: 26.04.1
- Summary: 4 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_spatialxe_pipeline/main.nf:30:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs            // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_spatialxe_pipeline/main.nf:75:144`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      after_text = """${workflow.manifest.doi ? "\n* The pipeline\n" : ""}${workflow.manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/', '')}" }.join("\n")}${workflow.manifest.doi ? "\n" : ""}
                                                                                                                                                 ^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:101:98`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return ch_versions.unique().map { version -> processVersionsFromYAML(version) }.unique().mix(Channel.of(workflowVersionToYAML()))
                                                                                                   ^^^^^^^
  ```
