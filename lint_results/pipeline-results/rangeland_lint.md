# Nextflow lint results

- Generated: 2026-03-25T00:26:59.587358248Z
- Nextflow version: 26.03.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `workflows/rangeland.nf:160:5`: Variable was declared but not used

  ```nextflow
      grouped_trend_data = HIGHER_LEVEL.out.mosaic.map{ it -> it[1] }.flatten().buffer( size: Integer.MAX_VALUE, remainder: true )
      ^^^^^^^^^^^^^^^^^^
  ```
