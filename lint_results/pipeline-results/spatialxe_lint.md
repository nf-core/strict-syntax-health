# Nextflow lint results

- Generated: 2026-05-21T00:43:09.610685328Z
- Nextflow version: 26.04.1
- Summary: 6 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_spatialxe_pipeline/main.nf:30:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs            // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_spatialxe_pipeline/main.nf:76:144`: Implicit closure parameter is deprecated, declare an explicit parameter instead

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

- Warning: `workflows/spatialxe.nf:208:88`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def missing_required = bundle_required_files.findAll { !file("${bundle_path}/${it}").exists() }
                                                                                         ^^
  ```

- Warning: `workflows/spatialxe.nf:213:88`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def missing_optional = bundle_optional_files.findAll { !file("${bundle_path}/${it}").exists() }
                                                                                         ^^
  ```
