# Nextflow lint results

- Generated: 2026-03-14T00:22:22.586815454Z
- Nextflow version: 26.02.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `workflows/ribomsqc.nf:26:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `workflows/ribomsqc.nf:46:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.value(file(params.analytes_tsv, checkIfExists: true))
              ^^^^^^^
  ```
