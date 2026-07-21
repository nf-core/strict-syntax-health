# Nextflow lint results

- Generated: 2026-07-21T00:31:37.221634578Z
- Nextflow version: 26.07.0-edge
- Summary: 11 warnings

## :warning: Warnings

- Warning: `modules/local/plots/metrics/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.benchmark_tool}"
          ^^^^^^
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

- Warning: `subworkflows/local/intersect_statistics/main.nf:18:13`: Variable was declared but not used

  ```nextflow
          def meta         = input[0]
              ^^^^
  ```

- Warning: `subworkflows/local/report_benchmark_statistics/main.nf:73:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def clean_meta = meta.findAll { it.key != 'csv' }
                                              ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_variantbenchmarking_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/vcf_variant_filtering/main.nf:28:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              vcf_ch.map{ meta, vcf, index -> tuple(meta, vcf)}
                                     ^^^^^
  ```

- Warning: `workflows/variantbenchmarking.nf:231:21`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def _meta = it[0]
                      ^^
  ```

- Warning: `workflows/variantbenchmarking.nf:232:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def regions_file = it[2]
                             ^^
  ```
