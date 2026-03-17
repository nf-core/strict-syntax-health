# Nextflow lint results

- Generated: 2026-03-17T00:30:02.422972+00:00
- Nextflow version: 26.02.0-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `modules/nf-core/numorph/resample/main.nf:18:9`: Variable was declared but not used

    ```nextflow
        def args = task.ext.args ?: ''
            ^^^^^^^^^^
    ```

- Warning: `modules/nf-core/numorph/resample/main.nf:19:9`: Variable was declared but not used

    ```nextflow
        def prefix = task.ext.prefix ?: "${meta.id}"
            ^^^^^^^^^^
    ```

- Warning: `modules/nf-core/numorph/resample/main.nf:36:9`: Variable was declared but not used

    ```nextflow
        def args = task.ext.args ?: ''
            ^^^^^^^^^^
    ```
