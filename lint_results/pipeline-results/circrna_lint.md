# Nextflow lint results

- Generated: 2026-03-31T00:24:31.479951081Z
- Nextflow version: 26.03.1-edge
- Summary: 20 warnings

## :warning: Warnings

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
