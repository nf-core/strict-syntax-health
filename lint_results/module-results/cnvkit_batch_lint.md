# Nextflow lint results

- Generated: 2026-03-17T00:30:02.346252+00:00
- Nextflow version: 26.02.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/cnvkit/batch/main.nf:110:9`: Variable was declared but not used

  ```nextflow
      def tumor_cram = tumor_exists && tumor.Extension == "cram" ? true : false
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/cnvkit/batch/main.nf:111:9`: Variable was declared but not used

  ```nextflow
      def normal_cram = normal_exists && normal.Extension == "cram" ? true : false
          ^^^^^^^^^^
  ```
