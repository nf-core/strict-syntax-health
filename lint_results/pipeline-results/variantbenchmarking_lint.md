# Nextflow lint results

- Generated: 2026-03-13T00:24:54.473113783Z
- Nextflow version: 26.02.0-edge
- Summary: 10 errors, 28 warnings

## :x: Errors

- Error: `subworkflows/local/concordance_analysis/main.nf:37:22`: Unexpected input: 'i'

  ```nextflow
              for (int i = 0; i < items.size(); i++) {
                       ^
  ```

- Error: `subworkflows/local/prepare_vcfs_test/main.nf:164:25`: `vcf` is already declared

  ```nextflow
          .branch { meta, vcf, tbi ->
                          ^^^
  ```

- Error: `subworkflows/local/prepare_vcfs_test/main.nf:175:45`: `vcf` is already declared

  ```nextflow
          ch_branched_vcf.needs_gt.map{ meta, vcf, _tbi -> tuple(meta, vcf) },
                                              ^^^
  ```

- Error: `subworkflows/local/sv_vcf_conversion/main.nf:86:19`: `input` is already declared

  ```nextflow
          .branch { input ->
                    ^^^^^
  ```

- Error: `subworkflows/local/sv_vcf_conversion/main.nf:135:19`: `input` is already declared

  ```nextflow
              .map{ input ->
                    ^^^^^
  ```

- Error: `subworkflows/local/wittyer_benchmark/main.nf:36:41`: `bed` is already declared

  ```nextflow
              .map{ meta, vcf, truth_vcf, bed -> [meta, vcf, truth_vcf, bed, []] }
                                          ^^^
  ```

- Error: `workflows/variantbenchmarking.nf:32:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/variantbenchmarking/subworkflows/local/concordance_analysis/main.nf'

  ```nextflow
  include { CONCORDANCE_ANALYSIS        } from '../subworkflows/local/concordance_analysis'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/variantbenchmarking.nf:249:7`: `CONCORDANCE_ANALYSIS` is not defined

  ```nextflow
        CONCORDANCE_ANALYSIS(
        ^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/variantbenchmarking.nf:256:43`: `CONCORDANCE_ANALYSIS` is not defined

  ```nextflow
          ch_reports       = ch_reports.mix(CONCORDANCE_ANALYSIS.out.summary_reports)
                                            ^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/variantbenchmarking.nf:257:41`: `CONCORDANCE_ANALYSIS` is not defined

  ```nextflow
          evals_ch         = evals_ch.mix(CONCORDANCE_ANALYSIS.out.tagged_variants)
                                          ^^^^^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/custom/merge_reports/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/custom/merge_sompy_features/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/custom/plots/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.benchmark_tool}"
          ^^^^^^
  ```

- Warning: `modules/local/custom/subtract_vcf/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/happy/happy/main.nf:64:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/ensemble_test_vcfs/main.nf:26:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      test_vcfs.branch { meta, vcf, index ->
                               ^^^
  ```

- Warning: `subworkflows/local/ensemble_test_vcfs/main.nf:26:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      test_vcfs.branch { meta, vcf, index ->
                                    ^^^^^
  ```

- Warning: `subworkflows/local/ensemble_test_vcfs/main.nf:37:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          branched_vcfs.missing_gt.map { meta, vcf, index -> tuple(meta, vcf) },
                                                    ^^^^^
  ```

- Warning: `subworkflows/local/ensemble_test_vcfs/main.nf:53:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_test_vcfs = ch_ready_for_merge.map { meta, vcf, index ->
                                                  ^^^^
  ```

- Warning: `subworkflows/local/ensemble_test_vcfs/main.nf:96:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_test_vcfs = vcf_ch.map { meta, vcf ->
                                      ^^^^
  ```

- Warning: `subworkflows/local/intersect_statistics/main.nf:20:13`: Variable was declared but not used

  ```nextflow
          def meta         = input[0]
              ^^^^
  ```

- Warning: `subworkflows/local/prepare_vcfs_test/main.nf:62:14`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_ch = Channel.empty()
               ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_vcfs_test/main.nf:164:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, vcf, tbi ->
                          ^^^
  ```

- Warning: `subworkflows/local/prepare_vcfs_test/main.nf:164:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, vcf, tbi ->
                               ^^^
  ```

- Warning: `subworkflows/local/sompy_benchmark/main.nf:23:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          input_ch.map{meta, test, test_index, truth, truth_index, regions, target -> [meta, test, truth, regions, target]},
                                   ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sompy_benchmark/main.nf:23:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          input_ch.map{meta, test, test_index, truth, truth_index, regions, target -> [meta, test, truth, regions, target]},
                                                      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sv_vcf_conversion/main.nf:43:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          out_vcf_ch = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/sv_vcf_conversion/main.nf:105:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          out_vcf_ch = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_variantbenchmarking_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_variantbenchmarking_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_variantbenchmarking_pipeline/main.nf:104:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/local/vcf_variant_filtering/main.nf:28:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              vcf_ch.map{ meta, vcf, index -> tuple(meta, vcf)}
                                     ^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:229:13`: Variable was declared but not used

  ```nextflow
          def meta = it[0]
              ^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:229:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def meta = it[0]
                     ^^
  ```

- Warning: `workflows/variantbenchmarking.nf:230:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def regions_file = it[2]
                             ^^
  ```

- Warning: `workflows/variantbenchmarking.nf:283:85`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(SV_GERMLINE_BENCHMARK.out.logs.map{ meta, log -> log })
                                                                                      ^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:399:118`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files                      = ch_multiqc_files.mix(REPORT_BENCHMARK_STATISTICS.out.merged_reports.map{ meta, report -> report }.flatten())
                                                                                                                       ^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:400:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files                      = ch_multiqc_files.mix(ch_reports.map{ meta, report -> report }.flatten())
                                                                                   ^^^^
  ```
