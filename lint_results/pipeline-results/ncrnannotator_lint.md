# Nextflow lint results

- Generated: 2026-03-25T00:26:06.557524658Z
- Nextflow version: 26.03.0-edge
- Summary: 4 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_ncrnannotator_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        monochrome_logs   // boolean: Do not use coloured log outputs
        ^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_ncrnannotator_pipeline/main.nf:180:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
                errors.collect { "    * ${it}" }.join("\n") + "\n" +
                                          ^^
    ```

- Warning: `workflows/ncrnannotator.nf:90:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
            CMSEARCH.out.tblout.collect { it[1] },
                                          ^^
    ```

- Warning: `workflows/ncrnannotator.nf:105:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        def topic_versions = Channel.topic("versions")
                             ^^^^^^^
    ```
