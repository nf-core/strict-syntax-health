# Nextflow lint results

- Generated: 2026-06-24T00:39:41.039706306Z
- Nextflow version: 26.05.0-edge
- Summary: 2 errors, 27 warnings

## :x: Errors

- Error: `modules/nf-core/bcftools/view/main.nf:60:9`: `index` is already declared

  ```nextflow
      def index = args.contains("--write-index=tbi") || args.contains("-W=tbi") ? "tbi" :
          ^^^^^
  ```

- Error: `modules/nf-core/snpsites/main.nf:16:11`: `CONSTANT_SITES` is not defined

  ```nextflow
      env   CONSTANT_SITES, emit: constant_sites_string
            ^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `main.nf:51:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      multiqc_report = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `main.nf:76:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/magma/modules/local/gatk4.nf:77:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/bcftools/merge/main.nf:28:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input = (vcfs.collect().size() > 1) ? vcfs.sort{ it.name } : vcfs
                                                           ^^
  ```

- Warning: `modules/nf-core/bwamem2/mem/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/bwamem2/mem/main.nf:62:9`: Variable was declared but not used

  ```nextflow
      def samtools_command = sort_bam ? 'sort' : 'view'
          ^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/bwamem2/mem/main.nf:66:9`: Variable was declared but not used

  ```nextflow
      def reference = fasta && extension=="cram"  ? "--reference ${fasta}" : ""
          ^^^^^^^^^
  ```

- Warning: `modules/nf-core/gatk4/markduplicates/main.nf:33:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = bam.collect{"--INPUT $it"}.join(' ')
                                            ^^
  ```

- Warning: `modules/nf-core/gatk4/variantstotable/main.nf:27:9`: Variable was declared but not used

  ```nextflow
      def include_intervals_arg = include_intervals ? "-L ${include_intervals}" : ""
          ^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/gatk4/variantstotable/main.nf:28:9`: Variable was declared but not used

  ```nextflow
      def exclude_intervals_arg = exclude_intervals ? "-XL ${exclude_intervals}" : ""
          ^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/iqtree/main.nf:68:9`: Variable was declared but not used

  ```nextflow
      def trees_rf_arg                = trees_rf                ? "-rf $trees_rf"                 : ''
          ^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/ismapper/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/lofreq/indelqual/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/samtools/stats/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/mtbseq/main.nf:33:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/mtbseq/main.nf:34:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files = Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/mtbseq/main.nf:36:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_reference_files = Channel.value([params.mtbseq_resilist,
                           ^^^^^^^
  ```

- Warning: `subworkflows/local/mtbseq/parallel_mode.nf:22:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/mtbseq/parallel_mode.nf:23:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_multiqc_files = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/mtbseq/quality_check.nf:12:28`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          samples_tsv_file = Channel.empty()
                             ^^^^^^^
  ```

- Warning: `subworkflows/local/mtbseq/quality_check.nf:27:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              samples_tsv_file = Channel.fromPath( params.mtbseq_cohort_tsv )
                                 ^^^^^^^
  ```

- Warning: `subworkflows/local/mtbseq/quality_check.nf:34:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      multiqc_files          = FASTQC.out.zip.collect{it[1]}
                                                      ^^
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

- Warning: `workflows/mtbseqnf.nf:54:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_workflow_summary = Channel.value(paramsSummaryMultiqc(summary_params))
                            ^^^^^^^
  ```

- Warning: `workflows/mtbseqnf.nf:60:45`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_methods_description                = Channel.value(
                                              ^^^^^^^
  ```
