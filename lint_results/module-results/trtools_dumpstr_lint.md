# Nextflow lint results

- Generated: 2026-06-13T00:52:33.652389+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/trtools/dumpstr/main.nf:29:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        def region_names = filter_regions ? filter_regions.collect { it.name.replaceFirst(/\.bed\.gz$/, '') }.join(',') : ''
                                                                     ^^^^^^^^^^
    ```
