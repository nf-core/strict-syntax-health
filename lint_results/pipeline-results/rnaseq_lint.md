# Nextflow lint results

- Generated: 2026-06-19T00:53:53.698304325Z
- Nextflow version: 26.04.4
- Summary: 5 warnings

## :warning: Warnings

- Warning: `subworkflows/local/multiqc_rnaseq/main.nf:247:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      report = MULTIQC.out.report.map { _meta, report -> report }
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_stringtie_merge/main.nf:29:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      stringtie_gtf = STRINGTIE_MERGE.out.merged_gtf // channel: [ meta, gtf ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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
