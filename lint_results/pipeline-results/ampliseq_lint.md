# Nextflow lint results

- Generated: 2026-06-16T20:16:24.585783013Z
- Nextflow version: 26.04.3
- Summary: 10 warnings

## :warning: Warnings

- Warning: `main.nf:46:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = AMPLISEQ.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/dada2_preprocessing.nf:54:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .findAll { it.trim() }  // Remove empty lines
                                 ^^
  ```

- Warning: `subworkflows/local/dada2_preprocessing.nf:55:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .collect { it.trim().toInteger() }
                                 ^^
  ```

- Warning: `subworkflows/local/parse_input.nf:84:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      reads   = ch_reads
      ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/qiime2_preptax.nf:96:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      classifier = QIIME2_TRAIN.out.qza
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sintax_taxonomy_wf.nf:47:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      tax      = ch_sintax_tax
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ampliseq_pipeline/main.nf:126:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions    = ch_versions
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      valid_config = valid_config
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```
