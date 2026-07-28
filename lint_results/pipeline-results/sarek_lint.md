# Nextflow lint results

- Generated: 2026-07-28T00:35:31.690735851Z
- Nextflow version: 26.07.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/cnvkit/batch/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def tumor_bam = tumor_exists && tumor.Extension == "bam" ? true : false
          ^^^^^^^^^
  ```

- Warning: `modules/nf-core/cnvkit/batch/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def normal_bam = normal_exists && normal.Extension == "bam" ? true : false
          ^^^^^^^^^^
  ```
