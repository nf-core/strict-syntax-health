# Nextflow lint results

- Generated: 2026-09-12T00:25:28.751150+00:00
- Nextflow version: 26.08.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/krakenuniq/preloadedkrakenuniq/main.nf:112:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def prefix_list = prefixes.collect { "'${it}'" }.join(' ')
                                               ^^^^^^^^^^
  ```
