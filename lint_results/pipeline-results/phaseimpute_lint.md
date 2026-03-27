# Nextflow lint results

- Generated: 2026-03-27T00:25:40.130745369Z
- Nextflow version: 26.03.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `workflows/phaseimpute/main.nf:286:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          if (params.tools.split(',').any{ it in ["stitch", "quilt"] }) {
                                           ^^
  ```
