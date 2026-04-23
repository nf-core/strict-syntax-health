# Nextflow lint results

- Generated: 2026-04-23T00:34:16.835309539Z
- Nextflow version: 26.03.3-edge
- Summary: 10 warnings

## :warning: Warnings

- Warning: `modules/local/cometconfig/main.nf:59:9`: Variable was declared but not used

    ```nextflow
        def prefix = task.ext.prefix ?: "${meta.id}"
            ^^^^^^
    ```

- Warning: `modules/local/ms2rescore/runms2rescore/main.nf:24:5`: Variable was declared but not used

    ```nextflow
        spectra_file = mzml ?: raw_spectra
        ^^^^^^^^^^^^
    ```

- Warning: `modules/local/ms2rescore/runms2rescore/main.nf:25:5`: Variable was declared but not used

    ```nextflow
        ms2pip_model = meta.ms2pip_model ?: 'HCD'
        ^^^^^^^^^^^^
    ```

- Warning: `modules/local/ms2rescore/runms2rescore/main.nf:26:5`: Variable was declared but not used

    ```nextflow
        spectrum_id_pattern = meta.spectrum_id_pattern ?: '.*scan=(\\d+)$'
        ^^^^^^^^^^^^^^^^^^^
    ```

- Warning: `modules/local/ms2rescore/runms2rescore/main.nf:27:5`: Variable was declared but not used

    ```nextflow
        fragment_tol_da = meta.fragment_tol_da ?: 0.02
        ^^^^^^^^^^^^^^^
    ```

- Warning: `modules/local/ms2rescore/runms2rescore/main.nf:28:5`: Variable was declared but not used

    ```nextflow
        chunk_size = task.ext.chunk_size ?: 100000
        ^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_mspepid_pipeline/main.nf:31:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        monochrome_logs // boolean: Do not use coloured log outputs
        ^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_mspepid_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        input //  string: Path to input samplesheet
        ^^^^^
    ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

    ```nextflow
        valid_config = checkConfigProvided()
        ^^^^^^^^^^^^
    ```

- Warning: `workflows/mspepid.nf:116:16`: Variable was declared but not used

    ```nextflow
            .set { ch_collated_versions }
                   ^^^^^^^^^^^^^^^^^^^^
    ```
