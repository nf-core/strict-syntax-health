# Nextflow lint results

- Generated: 2026-09-26T00:23:49.731684+00:00
- Nextflow version: 26.09.1-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/openms/mapaligneridentification/main.nf:22:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def trafo_out = id_files.collect { "${it.baseName}.trafoXML" }.join(' ')
                                            ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/openms/mapaligneridentification/main.nf:32:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def trafo_out = id_files.collect { "${it.baseName}.trafoXML" }.join(' ')
                                            ^^^^^^^^^^
  ```
