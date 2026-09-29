# Nextflow lint results

- Generated: 2026-09-29T00:26:05.686100+00:00
- Nextflow version: 26.09.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/trtools/dumpstr/main.nf:29:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def region_names = filter_regions ? filter_regions.collect { it.name.replaceFirst(/\.bed\.gz$/, '') }.join(',') : ''
                                                                   ^^^^^^^^^^
  ```
