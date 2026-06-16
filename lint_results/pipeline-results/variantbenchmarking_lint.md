# Nextflow lint results

- Generated: 2026-06-16T19:46:34.996089471Z
- Nextflow version: 26.04.3
- Summary: 36 warnings

## :warning: Warnings

- Warning: `main.nf:58:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = VARIANTBENCHMARKING.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/plots/metrics/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.benchmark_tool}"
          ^^^^^^
  ```

- Warning: `subworkflows/local/concordance_analysis/main.nf:63:15`: Variable was declared but not used

  ```nextflow
          .set{ summary_reports }
                ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/ensemble_test_vcfs/main.nf:33:86`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      BCFTOOLS_UNIFY_HEADER.out.vcf.join(BCFTOOLS_UNIFY_HEADER.out.tbi).branch { meta, vcf, index ->
                                                                                       ^^^
  ```

- Warning: `subworkflows/local/ensemble_test_vcfs/main.nf:33:91`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      BCFTOOLS_UNIFY_HEADER.out.vcf.join(BCFTOOLS_UNIFY_HEADER.out.tbi).branch { meta, vcf, index ->
                                                                                            ^^^^^
  ```

- Warning: `subworkflows/local/ensemble_test_vcfs/main.nf:44:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          branched_vcfs.missing_gt.map { meta, vcf, index -> tuple(meta, vcf) },
                                                    ^^^^^
  ```

- Warning: `subworkflows/local/ensemble_test_vcfs/main.nf:60:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_test_vcfs = ch_ready_for_merge.map { meta, vcf, index ->
                                                  ^^^^
  ```

- Warning: `subworkflows/local/ensemble_test_vcfs/main.nf:132:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      truth_vcf    // channel: [val(meta), vcf.gz, index]
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/happy_benchmark/main.nf:67:15`: Variable was declared but not used

  ```nextflow
          .set{ summary_reports }
                ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/intersect_statistics/main.nf:18:13`: Variable was declared but not used

  ```nextflow
          def meta         = input[0]
              ^^^^
  ```

- Warning: `subworkflows/local/intersect_statistics/main.nf:77:15`: Variable was declared but not used

  ```nextflow
          .set{ summary_reports }
                ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/intersect_statistics/main.nf:80:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      summary_reports  // channel: [meta, summary_report.csv]
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/liftover_vcfs/main.nf:51:5`: Variable was declared but not used

  ```nextflow
      vcf_ch = BCFTOOLS_ANNOTATE.out.vcf
      ^^^^^^
  ```

- Warning: `subworkflows/local/liftover_vcfs/main.nf:68:5`: Variable was declared but not used

  ```nextflow
      bed_ch = BEDTOOLS_MERGE.out.bed
      ^^^^^^
  ```

- Warning: `subworkflows/local/prepare_vcfs_test/main.nf:186:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_ch   // channel: [val(meta), vcf.gz, tbi]
      ^^^^^^
  ```

- Warning: `subworkflows/local/report_benchmark_statistics/main.nf:73:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def clean_meta = meta.findAll { it.key != 'csv' }
                                              ^^
  ```

- Warning: `subworkflows/local/report_vcf_statistics/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      ch_stats  // channel: [stats]
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/sompy_benchmark/main.nf:33:15`: Variable was declared but not used

  ```nextflow
          .set{ summary_reports }
                ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/split_small_variants_test/main.nf:51:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      out_vcf_ch     // channel: [val(meta), vcf, index]
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/subsample_vcf_test/main.nf:26:5`: Variable was declared but not used

  ```nextflow
      vcf_ch = BCFTOOLS_VIEW_SUBSAMPLE.out.vcf
      ^^^^^^
  ```

- Warning: `subworkflows/local/subsample_vcf_test/main.nf:29:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_ch      // channel: [val(meta), vcf]
      ^^^^^^
  ```

- Warning: `subworkflows/local/sv_vcf_conversion/main.nf:100:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          out_vcf_ch = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/sv_vcf_conversion/main.nf:139:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_ch   // channel: [val(meta), vcf]
      ^^^^^^
  ```

- Warning: `subworkflows/local/svanalyzer_benchmark/main.nf:32:15`: Variable was declared but not used

  ```nextflow
          .set{ report }
                ^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_variantbenchmarking_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/vcf_variant_deduplication/main.nf:27:14`: Variable was declared but not used

  ```nextflow
          .set{ch_vcf}
               ^^^^^^
  ```

- Warning: `subworkflows/local/vcf_variant_deduplication/main.nf:30:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      ch_vcf      // channel: [ val(meta), vcf, index ]
      ^^^^^^
  ```

- Warning: `subworkflows/local/vcf_variant_filtering/main.nf:28:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              vcf_ch.map{ meta, vcf, index -> tuple(meta, vcf)}
                                     ^^^^^
  ```

- Warning: `subworkflows/local/vcf_variant_filtering/main.nf:54:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      vcf_ch    // [val(meta), vcf.gz, index]
      ^^^^^^
  ```

- Warning: `subworkflows/local/wittyer_benchmark/main.nf:42:15`: Variable was declared but not used

  ```nextflow
          .set{ report }
                ^^^^^^
  ```

- Warning: `subworkflows/local/wittyer_benchmark/main.nf:45:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      report       // channel: [val(meta), reports]
      ^^^^^^
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

- Warning: `workflows/variantbenchmarking.nf:232:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def _meta = it[0]
                      ^^
  ```

- Warning: `workflows/variantbenchmarking.nf:233:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def regions_file = it[2]
                             ^^
  ```
