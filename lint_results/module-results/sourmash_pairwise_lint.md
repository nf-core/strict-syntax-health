# Nextflow lint results

- Generated: 2026-08-03T00:32:33.441120+00:00
- Nextflow version: 26.07.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/sourmash/pairwise/main.nf:36:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          combine_cmd = "sourmash sig cat ${signatures.sort { it.toString() }.join(' ')} -o ${prefix}_collection.zip"
                                                              ^^^^^^^^^^
  ```
