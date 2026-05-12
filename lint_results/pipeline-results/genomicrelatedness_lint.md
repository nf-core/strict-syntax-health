# Nextflow lint results

- Generated: 2026-05-12T00:34:18.556549689Z
- Nextflow version: 26.04.1
- Summary: 10 warnings

## :warning: Warnings

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

- Warning: `subworkflows/local/combine_cram_intervals/main.nf:24:13`: Variable was declared but not used

  ```nextflow
      }.set { cram_intervals }
              ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/cram_baserecalibrator/main.nf:57:5`: Variable was declared but not used

  ```nextflow
      table_bqsr = GATK4_GATHERBQSRREPORTS.out.table
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
