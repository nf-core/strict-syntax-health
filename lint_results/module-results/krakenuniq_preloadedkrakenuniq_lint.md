# Nextflow lint results

- Generated: 2026-09-24T00:22:52.558668+00:00
- Nextflow version: 26.09.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/krakenuniq/preloadedkrakenuniq/main.nf:112:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def prefix_list = prefixes.collect { "'${it}'" }.join(' ')
                                               ^^^^^^^^^^
  ```
