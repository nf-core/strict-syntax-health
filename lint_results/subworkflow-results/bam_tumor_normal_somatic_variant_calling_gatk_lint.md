# Nextflow lint results

- Generated: 2026-02-01T00:22:28.665574+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_tumor_normal_somatic_variant_calling_gatk/main.nf:25:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^^^^
  ```
