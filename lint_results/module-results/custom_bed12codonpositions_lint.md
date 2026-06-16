# Nextflow lint results

- Generated: 2026-06-16T00:54:14.277574+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/custom/bed12codonpositions/main.nf:22:5`: Variable was declared but not used

    ```nextflow
        args   = task.ext.args ?: ''
        ^^^^^^^^^^
    ```
