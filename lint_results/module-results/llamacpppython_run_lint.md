# Nextflow lint results

- Generated: 2026-05-08T00:36:08.058687+00:00
- Nextflow version: 26.04.0
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/llamacpppython/run/main.nf:21:5`: Variable was declared but not used

    ```nextflow
        args = task.ext.args ?: ''
        ^^^^^^^^^^
    ```
