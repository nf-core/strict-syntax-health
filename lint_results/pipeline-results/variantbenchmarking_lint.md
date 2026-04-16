# Nextflow lint results

- Generated: 2026-04-16T00:33:24.672898887Z
- Nextflow version: 26.03.2-edge
- Summary: 10 errors, 40 warnings

## :x: Errors

- Error: `subworkflows/local/concordance_analysis/main.nf:37:22`: Unexpected input: 'i'

  ```nextflow
              for (int i = 0; i < items.size(); i++) {
                       ^
  ```

- Error: `subworkflows/local/prepare_vcfs_test/main.nf:162:25`: `vcf` is already declared

  ```nextflow
          .branch { meta, vcf, tbi ->
                          ^^^
  ```

- Error: `subworkflows/local/prepare_vcfs_test/main.nf:173:45`: `vcf` is already declared

  ```nextflow
          ch_branched_vcf.needs_gt.map{ meta, vcf, _tbi -> tuple(meta, vcf) },
                                              ^^^
  ```

- Error: `subworkflows/local/sv_vcf_conversion/main.nf:81:19`: `input` is already declared

  ```nextflow
          .branch { input ->
                    ^^^^^
  ```

- Error: `subworkflows/local/sv_vcf_conversion/main.nf:130:19`: `input` is already declared

  ```nextflow
              .map{ input ->
                    ^^^^^
  ```

- Error: `subworkflows/local/wittyer_benchmark/main.nf:36:41`: `bed` is already declared

  ```nextflow
              .map{ meta, vcf, truth_vcf, bed -> [meta, vcf, truth_vcf, bed, []] }
                                          ^^^
  ```

- Error: `workflows/variantbenchmarking.nf:33:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/variantbenchmarking/subworkflows/local/concordance_analysis/main.nf'

  ```nextflow
  include { CONCORDANCE_ANALYSIS        } from '../subworkflows/local/concordance_analysis'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/variantbenchmarking.nf:246:7`: `CONCORDANCE_ANALYSIS` is not defined

  ```nextflow
        CONCORDANCE_ANALYSIS(
        ^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/variantbenchmarking.nf:253:43`: `CONCORDANCE_ANALYSIS` is not defined

  ```nextflow
          ch_reports       = ch_reports.mix(CONCORDANCE_ANALYSIS.out.summary_reports)
                                            ^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/variantbenchmarking.nf:254:41`: `CONCORDANCE_ANALYSIS` is not defined

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

- Warning: `modules/local/plots/metrics/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.benchmark_tool}"
          ^^^^^^
  ```

- Warning: `modules/local/sompy_features/merge/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/happy/happy/main.nf:64:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/variantextractor/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      pass_only    = task.ext.args?.contains('--pass-only')       ? 'True'  : 'False'
      ^^^^^^^^^
  ```

- Warning: `modules/nf-core/variantextractor/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      ensure_pairs = task.ext.args?.contains('--no-ensure-pairs') ? 'False' : 'True'
      ^^^^^^^^^^^^
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

- Warning: `subworkflows/local/ensemble_test_vcfs/main.nf:103:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_test_vcfs = vcf_ch.map { meta, vcf ->
                                      ^^^^
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

- Warning: `subworkflows/local/intersect_statistics/main.nf:75:15`: Variable was declared but not used

  ```nextflow
          .set{ summary_reports }
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

- Warning: `subworkflows/local/prepare_vcfs_test/main.nf:59:14`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_ch = Channel.empty()
               ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_vcfs_test/main.nf:162:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, vcf, tbi ->
                          ^^^
  ```

- Warning: `subworkflows/local/prepare_vcfs_test/main.nf:162:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, vcf, tbi ->
                               ^^^
  ```

- Warning: `subworkflows/local/sompy_benchmark/main.nf:22:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          input_ch.map{meta, test, test_index_, truth, truth_index_, regions, target -> [meta, test, truth, regions, target]},
                                   ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sompy_benchmark/main.nf:22:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          input_ch.map{meta, test, test_index_, truth, truth_index_, regions, target -> [meta, test, truth, regions, target]},
                                                       ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sompy_benchmark/main.nf:33:15`: Variable was declared but not used

  ```nextflow
          .set{ summary_reports }
                ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/subsample_vcf_test/main.nf:26:5`: Variable was declared but not used

  ```nextflow
      vcf_ch = BCFTOOLS_VIEW_SUBSAMPLE.out.vcf
      ^^^^^^
  ```

- Warning: `subworkflows/local/sv_vcf_conversion/main.nf:38:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          out_vcf_ch = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/sv_vcf_conversion/main.nf:100:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          out_vcf_ch = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/svanalyzer_benchmark/main.nf:32:15`: Variable was declared but not used

  ```nextflow
          .set{ report }
                ^^^^^^
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

- Warning: `subworkflows/local/vcf_variant_deduplication/main.nf:27:14`: Variable was declared but not used

  ```nextflow
          .set{ch_vcf}
               ^^^^^^
  ```

- Warning: `subworkflows/local/vcf_variant_filtering/main.nf:28:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              vcf_ch.map{ meta, vcf, index -> tuple(meta, vcf)}
                                     ^^^^^
  ```

- Warning: `subworkflows/local/wittyer_benchmark/main.nf:42:15`: Variable was declared but not used

  ```nextflow
          .set{ report }
                ^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:227:13`: Variable was declared but not used

  ```nextflow
          def meta = it[0]
              ^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:227:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def meta = it[0]
                     ^^
  ```

- Warning: `workflows/variantbenchmarking.nf:228:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def regions_file = it[2]
                             ^^
  ```

- Warning: `workflows/variantbenchmarking.nf:277:76`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(SV_BENCHMARK.out.logs.map{ meta, log -> log })
                                                                             ^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:307:77`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(CNV_BENCHMARK.out.logs.map{ meta, log -> log })
                                                                              ^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:409:118`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files                      = ch_multiqc_files.mix(REPORT_BENCHMARK_STATISTICS.out.merged_reports.map{ meta, report -> report }.flatten())
                                                                                                                       ^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:410:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files                      = ch_multiqc_files.mix(ch_reports.map{ meta, report -> report }.flatten())
                                                                                   ^^^^
  ```
