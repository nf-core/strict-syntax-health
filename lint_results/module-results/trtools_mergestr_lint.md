# Nextflow lint results

- Generated: 2026-07-21T00:32:29.092246+00:00
- Nextflow version: 26.07.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/trtools/mergestr/main.nf:24:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      if ( vcfs.any{ "${it}" == "${prefix}.vcf" || "${it}" == "${prefix}.vcf.gz" } ) {
                        ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/trtools/mergestr/main.nf:24:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      if ( vcfs.any{ "${it}" == "${prefix}.vcf" || "${it}" == "${prefix}.vcf.gz" } ) {
                                                      ^^^^^^^^^^
  ```
