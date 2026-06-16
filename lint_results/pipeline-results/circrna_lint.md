# Nextflow lint results

- Generated: 2026-06-16T14:10:56.915006444Z
- Nextflow version: 26.04.3
- Summary: 29 warnings

## :warning: Warnings

- Warning: `main.nf:81:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = CIRCRNA.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/circtest/prepare/main.nf:19:5`: Variable was declared but not used

  ```nextflow
      prefix = task.ext.prefix ?: meta.id
      ^^^^^^
  ```

- Warning: `modules/local/ciri/build_list/main.nf:19:5`: Variable was declared but not used

  ```nextflow
      max_shift = task.ext.max_shift ?: 0
      ^^^^^^^^^
  ```

- Warning: `modules/local/combinebeds/reads/main.nf:21:5`: Variable was declared but not used

  ```nextflow
      consider_strand = task.ext.consider_strand ?: false
      ^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/combinebeds/reads/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      min_tools       = task.ext.min_tools       ?: 2
      ^^^^^^^^^
  ```

- Warning: `modules/local/combinebeds/shifts/main.nf:19:5`: Variable was declared but not used

  ```nextflow
      prefix      = task.ext.prefix      ?: "${meta.id}"
      ^^^^^^
  ```

- Warning: `modules/local/majority_vote/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      min_tools = params.mirna_min_tools
      ^^^^^^^^^
  ```

- Warning: `modules/local/matrix/join_samples/main.nf:21:5`: Variable was declared but not used

  ```nextflow
      metacols = task.ext.metacols ?: "gene_id,gene_name"
      ^^^^^^^^
  ```

- Warning: `modules/local/matrix/join_samples/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      has_header = task.ext.has_header == null ? true : task.ext.has_header
      ^^^^^^^^^^
  ```

- Warning: `modules/local/mirna_targets/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/tximeta/tximeta/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      prefix = task.ext.prefix ?: meta.id
      ^^^^^^
  ```

- Warning: `modules/nf-core/bwa/mem/main.nf:32:9`: Variable was declared but not used

  ```nextflow
      def samtools_command = sort_bam ? 'sort' : 'view'
          ^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/bwa/mem/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def reference = fasta && extension=="cram"  ? "--reference ${fasta}" : ""
          ^^^^^^^^^
  ```

- Warning: `subworkflows/local/fli_tools/jccirc.nf:40:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions = ch_versions
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/longread.nf:15:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions = ch_versions
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/longread_tools/circtools.nf:19:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions = ch_versions
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/mirna_prediction.nf:82:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions = ch_versions
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/statistical_tests.nf:76:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions = ch_versions
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastqc_trimgalore.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastqc_trimgalore.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      fastqc_html = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastqc_trimgalore.nf:17:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      fastqc_zip  = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastqc_trimgalore.nf:24:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      trim_html  = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastqc_trimgalore.nf:25:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      trim_zip   = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastqc_trimgalore.nf:26:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      trim_log   = Channel.empty()
                   ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastqc_trimgalore.nf:27:5`: Variable was declared but not used

  ```nextflow
      trimgalore_versions = Channel.empty()
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fastqc_trimgalore.nf:27:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      trimgalore_versions = Channel.empty()
                            ^^^^^^^
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
