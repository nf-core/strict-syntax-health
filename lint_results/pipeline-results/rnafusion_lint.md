# Nextflow lint results

- Generated: 2026-06-23T00:44:55.608910087Z
- Nextflow version: 26.05.0-edge
- Summary: 6 warnings

## :warning: Warnings

- Warning: `subworkflows/local/fusioncatcher_workflow/main.nf:46:9`: Emit name should be omitted when there is only one emit

  ```nextflow
          fusions  = ch_fusioncatcher_fusions     // channel [ meta, fusions ]
          ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/fusioninspector_workflow/main.nf:76:9`: Emit name should be omitted when there is only one emit

  ```nextflow
          ch_arriba_visualisation = ch_arriba_visualisation
          ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:76:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```
