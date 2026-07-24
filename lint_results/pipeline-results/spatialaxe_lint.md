# Nextflow lint results

- Generated: 2026-07-24T00:29:31.118089208Z
- Nextflow version: 26.07.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:101:98`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return ch_versions.unique().map { version -> processVersionsFromYAML(version) }.unique().mix(Channel.of(workflowVersionToYAML()))
                                                                                                   ^^^^^^^
  ```
