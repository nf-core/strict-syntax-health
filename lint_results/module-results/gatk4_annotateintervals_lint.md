# Nextflow lint results

- Generated: 2026-01-22T00:21:30.686230+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gatk4/annotateintervals/main.nf:31:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def inputs = intervals.collect { "--intervals ${it}" }.join(" ")
                                                      ^^^^^^^^^^
  ```
