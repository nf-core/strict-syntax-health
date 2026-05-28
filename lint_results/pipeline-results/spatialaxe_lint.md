# Nextflow lint results

- Generated: 2026-05-28T00:39:43.932932085Z
- Nextflow version: 26.04.2
- Summary: 10 warnings

## :warning: Warnings

- Warning: `main.nf:84:5`: Emit name should be omitted when there is only one emit

    ```nextflow
        multiqc_report = SPATIALXE.out.multiqc_report // channel: /path/to/multiqc_report.html
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/baysor_generate_segfree/main.nf:51:5`: Emit name should be omitted when there is only one emit

    ```nextflow
        ncvs     = BAYSOR_SEGFREE.out.ncvs // channel: [ val(meta), ["ncvs.loom"] ]
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_spatialxe_pipeline/main.nf:30:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        monochrome_logs            // boolean: Do not use coloured log outputs
        ^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_spatialxe_pipeline/main.nf:76:144`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        after_text = """${workflow.manifest.doi ? "\n* The pipeline\n" : ""}${workflow.manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/', '')}" }.join("\n")}${workflow.manifest.doi ? "\n" : ""}
                                                                                                                                                   ^^
    ```

- Warning: `subworkflows/local/utils_nfcore_spatialxe_pipeline/main.nf:149:5`: Emit name should be omitted when there is only one emit

    ```nextflow
        samplesheet = ch_samplesheet
        ^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

    ```nextflow
        dummy_emit = true
        ^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

    ```nextflow
        valid_config = checkConfigProvided()
        ^^^^^^^^^^^^
    ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

    ```nextflow
        valid_config
        ^^^^^^^^^^^^
    ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:101:98`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        return ch_versions.unique().map { version -> processVersionsFromYAML(version) }.unique().mix(Channel.of(workflowVersionToYAML()))
                                                                                                     ^^^^^^^
    ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

    ```nextflow
        dummy_emit = true
        ^^^^^^^^^^^^^^^
    ```
