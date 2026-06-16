# Nextflow lint results

- Generated: 2026-06-16T14:11:45.864457732Z
- Nextflow version: 26.04.3
- Summary: 12 warnings

## :warning: Warnings

- Warning: `main.nf:63:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = CREATETAXDB.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/ganon/buildcustom/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/ganon/buildcustom/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def taxonomy_args = taxonomy_files ? "--taxonomy-files ${taxonomy_files}" : ""
          ^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/ganon/buildcustom/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def genome_size_args = genome_size_files ? "--genome-size-files ${genome_size_files}" : ""
          ^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/malt/build/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/pigz/compress/main.nf:35:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/unzip/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/kmcp_create/main.nf:40:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      db = KMCP_INDEX.out.kmcp // channel: [ val(meta), [ db ] ]
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sourmash_create/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      db = SOURMASH_INDEX.out.signature_index // channel: [ val(meta), index ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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
