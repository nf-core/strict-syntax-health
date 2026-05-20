# Nextflow lint results

- Generated: 2026-05-20T00:45:14.592361+00:00
- Nextflow version: 26.04.1
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/humann3/renorm/main.nf:42:9`: Variable was declared but not used

    ```nextflow
        def args = task.ext.args ?: ''
            ^^^^^^^^^^
    ```
