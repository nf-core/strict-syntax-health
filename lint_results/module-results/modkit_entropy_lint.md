# Nextflow lint results

- Generated: 2026-11-28T00:16:00.844960+00:00
- Nextflow version: 26.11.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/modkit/entropy/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```

- Warning: `modules/nf-core/modkit/entropy/main.nf:30:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def bam_args = bams instanceof List ? bams.collect { "--in-bam ${it}" }.join(' ') : "--in-bam ${bams}"
                                                                       ^^^^^^^^^^
  ```
