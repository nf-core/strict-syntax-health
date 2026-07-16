# Nextflow lint results

- Generated: 2026-07-16T00:33:07.425002+00:00
- Nextflow version: 26.06.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/gridss/preprocess/main.nf:23:9`: Variable was declared but not used

    ```nextflow
        def prefix = task.ext.prefix ?: "${meta.id}"
            ^^^^^^^^^^
    ```

- Warning: `modules/nf-core/gridss/preprocess/main.nf:46:9`: Variable was declared but not used

    ```nextflow
        def args = task.ext.args ?: ''
            ^^^^^^^^^^
    ```
