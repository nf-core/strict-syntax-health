# Nextflow lint results

- Generated: 2026-02-10T00:27:01.449166+00:00
- Nextflow version: 26.01.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/cnvkit/access/main.nf:24:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def exclude_cmd = exclude_bed.collect { "-x ${it}" }.join(" ")
                                                    ^^^^^^^^^^
  ```
