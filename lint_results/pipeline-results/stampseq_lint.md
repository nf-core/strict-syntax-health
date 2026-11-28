# Nextflow lint results

- Generated: 2026-11-28T00:14:52.907498432Z
- Nextflow version: 26.11.0-edge
- Summary: 10 warnings

## :warning: Warnings

- Warning: `modules/local/filter_edits_bulk/main.nf:26:9`: Variable was declared but not used

    ```nextflow
        def prefix = meta.id
            ^^^^^^
    ```

- Warning: `modules/local/filter_edits_bulk/main.nf:39:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        ].findAll { it }.join(" ")
                    ^^
    ```

- Warning: `modules/local/filter_edits_sc/main.nf:25:9`: Variable was declared but not used

    ```nextflow
        def prefix = meta.id
            ^^^^^^
    ```

- Warning: `modules/local/filter_edits_sc/main.nf:31:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        ].findAll { it }.join(" ")
                    ^^
    ```

- Warning: `modules/local/normalize_edits_sc/main.nf:23:9`: Variable was declared but not used

    ```nextflow
        def prefix = meta.id
            ^^^^^^
    ```

- Warning: `modules/nf-core/fastqc/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

    ```nextflow
        when:
        ^^^^
    ```

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

    ```nextflow
        when:
        ^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_stampseq_pipeline/main.nf:452:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
            ].findAll { it }.join(' ').trim()
                        ^^
    ```

- Warning: `workflows/stampseq.nf:203:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
                                def majority = orig.countBy { it }.max { it.value }.key
                                                              ^^
    ```

- Warning: `workflows/stampseq.nf:203:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
                                def majority = orig.countBy { it }.max { it.value }.key
                                                                         ^^
    ```
