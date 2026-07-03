# Nextflow lint results

- Generated: 2026-07-03T00:37:55.228624+00:00
- Nextflow version: 26.06.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/fgumi/fastq/main.nf:34:9`: Variable was declared but not used

    ```nextflow
        def args = task.ext.args ?: ''
            ^^^^^^^^^^
    ```
