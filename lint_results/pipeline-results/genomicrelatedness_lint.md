# Nextflow lint results

- Generated: 2026-06-16T14:18:43.833066815Z
- Nextflow version: 26.04.3
- Summary: 17 warnings

## :warning: Warnings

- Warning: `main.nf:49:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = GENOMICRELATEDNESS.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/base_quality_score_recalibration/main.nf:33:5`: Variable was declared but not used

  ```nextflow
      versions = channel.empty()
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/base_quality_score_recalibration/main.nf:34:5`: Variable was declared but not used

  ```nextflow
      multiqc_files = channel.empty()
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/call_variants_bcftools/main.nf:28:5`: Variable was declared but not used

  ```nextflow
      versions = channel.empty()
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/call_variants_bcftools/main.nf:29:5`: Variable was declared but not used

  ```nextflow
      multiqc_files = channel.empty()
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/call_variants_gatk/main.nf:30:5`: Variable was declared but not used

  ```nextflow
      versions = channel.empty()
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/combine_cram_crai_intervals/main.nf:24:13`: Variable was declared but not used

  ```nextflow
      }.set { cram_crai_intervals }
              ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/combine_cram_crai_intervals/main.nf:27:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      cram_crai_intervals
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/combine_cram_intervals/main.nf:24:13`: Variable was declared but not used

  ```nextflow
      }.set { cram_intervals }
              ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/combine_cram_intervals/main.nf:27:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      cram_intervals
      ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/cram_baserecalibrator/main.nf:57:5`: Variable was declared but not used

  ```nextflow
      table_bqsr = GATK4_GATHERBQSRREPORTS.out.table
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/cram_baserecalibrator/main.nf:67:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      table_bqsr
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      intervals_combined = BUILD_INTERVALS.out.output
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_intervals/main.nf:48:5`: Variable was declared but not used

  ```nextflow
      intervals_split = split_with_meta
      ^^^^^^^^^^^^^^^
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
