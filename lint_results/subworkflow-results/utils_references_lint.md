# Nextflow lint results

- Generated: 2026-02-13T00:25:10.845817+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/utils_references/main.nf:18:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      references = Channel.fromList(samplesheetToList(yaml_reference, "${projectDir}/subworkflows/nf-core/utils_references/schema_references.json"))
                   ^^^^^^^^^^
  ```
