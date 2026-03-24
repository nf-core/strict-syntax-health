# Nextflow lint results

- Generated: 2026-03-24T00:24:41.440085+00:00
- Nextflow version: 26.03.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/custom/geneticmapconvert/main.nf:25:5`: Variable was declared but not used

    ```nextflow
        args = task.ext.args ?: ''
        ^^^^^^^^^^
    ```
