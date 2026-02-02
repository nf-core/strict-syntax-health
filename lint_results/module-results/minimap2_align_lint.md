# Nextflow lint results

- Generated: 2026-02-02T00:19:53.431201+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/minimap2/align/main.nf:62:9`: Variable was declared but not used

  ```nextflow
      def target = reference ?: (bam_input ? error("BAM input requires reference") : reads)
          ^^^^^^^^^^
  ```
