# Nextflow lint results

- Generated: 2026-03-13T00:20:13.432510240Z
- Nextflow version: 26.02.0-edge
- Summary: 10 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_genephylomodeler_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        monochrome_logs   // boolean: Do not use coloured log outputs
        ^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genephylomodeler_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        input             //  string: Path to input samplesheet
        ^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genephylomodeler_pipeline/main.nf:42:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        ch_versions = Channel.empty()
                      ^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genephylomodeler_pipeline/main.nf:67:144`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        after_text = """${workflow.manifest.doi ? "\n* The pipeline\n" : ""}${workflow.manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${workflow.manifest.doi ? "\n" : ""}
                                                                                                                                                   ^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genephylomodeler_pipeline/main.nf:104:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        Channel
        ^^^^^^^
    ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:101:98`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        return ch_versions.unique().map { version -> processVersionsFromYAML(version) }.unique().mix(Channel.of(workflowVersionToYAML()))
                                                                                                     ^^^^^^^
    ```

- Warning: `workflows/genephylomodeler.nf:29:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        ch_versions = Channel.empty()
                      ^^^^^^^
    ```

- Warning: `workflows/genephylomodeler.nf:36:19`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
                meta, alignment, tree ->
                      ^^^^^^^^^
    ```

- Warning: `workflows/genephylomodeler.nf:36:30`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
                meta, alignment, tree ->
                                 ^^^^
    ```

- Warning: `workflows/genephylomodeler.nf:105:17`: Variable was declared but not used

    ```nextflow
            ).set { ch_collated_versions }
                    ^^^^^^^^^^^^^^^^^^^^
    ```
