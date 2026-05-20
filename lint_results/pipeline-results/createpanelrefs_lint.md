# Nextflow lint results

- Generated: 2026-05-20T00:39:30.855080667Z
- Nextflow version: 26.04.1
- Summary: 1 warning

## :warning: Warnings

- Warning: `conf/modules/mutect2.config:50:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              saveAs: { meta.num_intervals > 1 ? null : it },
                                                        ^^
  ```
