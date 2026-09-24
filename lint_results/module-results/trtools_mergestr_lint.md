# Nextflow lint results

- Generated: 2026-09-24T00:22:52.703918+00:00
- Nextflow version: 26.09.0-edge
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
