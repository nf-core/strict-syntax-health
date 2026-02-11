# Nextflow lint results

- Generated: 2026-02-11T00:29:54.573452656Z
- Nextflow version: 26.01.0-edge
- Summary: 10 errors, 69 warnings

## :x: Errors

- Error: `modules/nf-core/wittyer/main.nf:8:5`: Invalid process directive

  ```nextflow
      if (workflow.profile.tokenize(',').intersect(['conda', 'mamba']).size() >= 1) {
      ^
  ```

- Error: `subworkflows/local/concordance_analysis/main.nf:38:22`: Unexpected input: 'i'

  ```nextflow
              for (int i = 0; i < items.size(); i++) {
                       ^
  ```

- Error: `subworkflows/local/sv_vcf_conversion/main.nf:90:19`: `input` is already declared

  ```nextflow
          .branch { input ->
                    ^^^^^
  ```

- Error: `subworkflows/local/sv_vcf_conversion/main.nf:142:19`: `input` is already declared

  ```nextflow
              .map{ input ->
                    ^^^^^
  ```

- Error: `subworkflows/local/wittyer_benchmark/main.nf:42:41`: `bed` is already declared

  ```nextflow
              .map{ meta, vcf, truth_vcf, bed -> [meta, vcf, truth_vcf, bed, []] }
                                          ^^^
  ```

- Error: `workflows/variantbenchmarking.nf:32:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/variantbenchmarking/subworkflows/local/concordance_analysis/main.nf'

  ```nextflow
  include { CONCORDANCE_ANALYSIS        } from '../subworkflows/local/concordance_analysis'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/variantbenchmarking.nf:235:7`: `CONCORDANCE_ANALYSIS` is not defined

  ```nextflow
        CONCORDANCE_ANALYSIS(
        ^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/variantbenchmarking.nf:242:44`: `CONCORDANCE_ANALYSIS` is not defined

  ```nextflow
          ch_versions      = ch_versions.mix(CONCORDANCE_ANALYSIS.out.versions)
                                             ^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/variantbenchmarking.nf:243:43`: `CONCORDANCE_ANALYSIS` is not defined

  ```nextflow
          ch_reports       = ch_reports.mix(CONCORDANCE_ANALYSIS.out.summary_reports)
                                            ^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/variantbenchmarking.nf:244:41`: `CONCORDANCE_ANALYSIS` is not defined

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

- Warning: `modules/nf-core/bedops/convert2bed/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/happy/happy/main.nf:64:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/happy/prepy/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/happy/prepy/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def restrict_region = bed ? "-R ${bed}": ""
          ^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/survivor/filter/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/survivor/filter/main.nf:51:9`: Variable was declared but not used

  ```nextflow
      def bed_file = bed ? "${bed}" : "NA"
          ^^^^^^^^
  ```

- Warning: `modules/nf-core/survivor/merge/main.nf:30:13`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          if (it.getExtension() == "gz"){
              ^^
  ```

- Warning: `modules/nf-core/survivor/merge/main.nf:57:13`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          if (it.getExtension() == "gz"){
              ^^
  ```

- Warning: `modules/nf-core/survivor/stats/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/svanalyzer/svbenchmark/main.nf:63:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/wittyer/main.nf:62:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/intersect_statistics/main.nf:20:13`: Variable was declared but not used

  ```nextflow
          def meta         = input[0]
              ^^^^
  ```

- Warning: `subworkflows/local/prepare_vcfs_test/main.nf:61:14`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      vcf_ch = Channel.empty()
               ^^^^^^^
  ```

- Warning: `subworkflows/local/sompy_benchmark/main.nf:24:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          input_ch.map{meta, test, test_index, truth, truth_index, regions, target -> [meta, test, truth, regions, target]},
                                   ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sompy_benchmark/main.nf:24:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          input_ch.map{meta, test, test_index, truth, truth_index, regions, target -> [meta, test, truth, regions, target]},
                                                      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/subsample_vcf_test/main.nf:31:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, vcf ->
                          ^^^
  ```

- Warning: `subworkflows/local/subsample_vcf_test/main.nf:38:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.value('q'),
          ^^^^^^^
  ```

- Warning: `subworkflows/local/subsample_vcf_test/main.nf:39:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.value('0p --include "1"'),
          ^^^^^^^
  ```

- Warning: `subworkflows/local/sv_vcf_conversion/main.nf:44:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          out_vcf_ch = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/sv_vcf_conversion/main.nf:110:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

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

- Warning: `subworkflows/local/vcf_variant_filtering/main.nf:30:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              vcf_ch.map{ meta, vcf, index -> tuple(meta, vcf)}
                                     ^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:55:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      fasta       = Channel.fromPath(params.fasta, checkIfExists: true)
                    ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:57:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      fai         = Channel.fromPath(params.fai, checkIfExists: true)
                    ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:61:42`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      truth_ch        = params.truth_vcf ? Channel.fromPath(params.truth_vcf, checkIfExists: true)
                                           ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:63:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                                          : Channel.empty()
                                            ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:65:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      regions_bed_ch = params.regions_bed ? Channel.fromPath(params.regions_bed, checkIfExists: true).collect()
                                            ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:66:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                                          : Channel.empty()
                                            ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:67:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      targets_bed_ch = params.targets_bed ? Channel.fromPath(params.targets_bed, checkIfExists: true).collect()
                                            ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:68:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                                          : Channel.empty()
                                            ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:87:55`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      falsepositive_bed   = params.falsepositive_bed  ? Channel.fromPath(params.falsepositive_bed, checkIfExists: true).map{ bed -> tuple([id: "falsepositive"], bed) }.collect()
                                                        ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:88:55`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                                                      : Channel.of([[id: "falsepositive"],[]]).collect()
                                                        ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:89:55`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ambiguous_beds      = params.ambiguous_beds     ? Channel.fromPath(params.ambiguous_beds, checkIfExists: true).map{ bed -> tuple([id: "ambiguous"], bed) }.collect()
                                                        ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:90:55`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                                                      : Channel.of([[id: "ambiguous"],[]]).collect()
                                                        ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:92:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          stratification_bed  = Channel.fromPath(params.stratification_bed, checkIfExists: true, type: 'dir').map{ bed -> tuple([id: "stratification"], bed) }.collect()
                                ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:93:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          stratification_tsv  = Channel.fromPath(params.stratification_tsv, checkIfExists: true).map{ tsv -> tuple([id: "stratification"], tsv) }.collect()
                                ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:95:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          stratification_bed  = Channel.of([[id: "stratification"],[]]).collect()
                                ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:96:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          stratification_tsv  = Channel.of([[id: "stratification"],[]]).collect()
                                ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:100:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      sdf             = params.sdf        ? Channel.fromPath(params.sdf, checkIfExists: true).map{ sdf -> tuple([id: sdf.getSimpleName()], sdf) }.collect()
                                            ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:101:43`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                                          : Channel.empty()
                                            ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:104:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          rename_chr = Channel.fromPath(params.rename_chr, checkIfExists: true).map{ txt -> tuple([id: txt.getSimpleName()], txt) }.collect()
                       ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:112:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              rename_chr = Channel.fromPath("${projectDir}/assets/rename_contigs/grch37_grch38.txt", checkIfExists: true).map{ txt -> tuple([id: txt.getSimpleName()], txt) }.collect()
                           ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:116:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              rename_chr = Channel.fromPath("${projectDir}/assets/rename_contigs/grch38_grch37.txt", checkIfExists: true).map{ txt -> tuple([id: txt.getSimpleName()], txt) }.collect()
                           ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:119:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              rename_chr = Channel.empty()
                           ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:127:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              chain           = Channel.fromPath(params.chain, checkIfExists: true).map{ bed -> tuple([id: bed.getSimpleName()], bed) }.collect()
                                ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:133:47`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          dictionary      = params.dictionary ? Channel.fromPath(params.dictionary, checkIfExists: true).map{ dict -> tuple([id: dict.getSimpleName()], dict) }.collect()                                           : Channel.empty()
                                                ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:133:213`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          dictionary      = params.dictionary ? Channel.fromPath(params.dictionary, checkIfExists: true).map{ dict -> tuple([id: dict.getSimpleName()], dict) }.collect()                                           : Channel.empty()
                                                                                                                                                                                                                      ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:135:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          chain           = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:136:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          dictionary      = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:213:13`: Variable was declared but not used

  ```nextflow
          def meta = it[0]
              ^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:213:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def meta = it[0]
                     ^^
  ```

- Warning: `workflows/variantbenchmarking.nf:214:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def regions_file = it[2]
                             ^^
  ```

- Warning: `workflows/variantbenchmarking.nf:266:85`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(SV_GERMLINE_BENCHMARK.out.logs.map{ meta, log -> log })
                                                                                      ^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:341:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:371:45`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_config                     = Channel.fromPath("$projectDir/assets/multiqc_config.yml", checkIfExists: true)
                                              ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:372:69`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_custom_config              = params.multiqc_config ? Channel.fromPath(params.multiqc_config, checkIfExists: true) :Channel.empty()
                                                                      ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:372:131`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_custom_config              = params.multiqc_config ? Channel.fromPath(params.multiqc_config, checkIfExists: true) :Channel.empty()
                                                                                                                                    ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:373:67`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_logo                       = params.multiqc_logo ? Channel.fromPath(params.multiqc_logo, checkIfExists: true) : Channel.empty()
                                                                    ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:373:128`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_logo                       = params.multiqc_logo ? Channel.fromPath(params.multiqc_logo, checkIfExists: true) : Channel.empty()
                                                                                                                                 ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:375:45`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_workflow_summary                   = Channel.value(paramsSummaryMultiqc(summary_params))
                                              ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:378:45`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_methods_description                = Channel.value(methodsDescriptionText(ch_multiqc_custom_methods_description))
                                              ^^^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:384:118`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files                      = ch_multiqc_files.mix(REPORT_BENCHMARK_STATISTICS.out.merged_reports.map{ meta, report -> report }.flatten())
                                                                                                                       ^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:385:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files                      = ch_multiqc_files.mix(ch_reports.map{ meta, report -> report }.flatten())
                                                                                   ^^^^
  ```
