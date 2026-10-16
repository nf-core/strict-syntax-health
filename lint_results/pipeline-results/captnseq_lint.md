# Nextflow lint results

- Generated: 2026-10-16T00:17:58.329806103Z
- Nextflow version: 26.10.1
- Summary: 4 warnings

## :warning: Warnings

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

- Warning: `workflows/captnseq.nf:113:74`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        PRODUCE_INSERTION_COUNTS(SAM2SITES.out.unstranded_unnormalized.map { meta, bg -> bg }.collect())
                                                                             ^^^^
    ```

- Warning: `workflows/captnseq.nf:114:67`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        PRODUCE_CHR_COUNTS(GREP_OTHER_CHROMOSOMES.out.chr_count.map { meta, tsv -> tsv }.collect())
                                                                      ^^^^
    ```
