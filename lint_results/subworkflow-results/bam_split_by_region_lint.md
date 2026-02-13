# Nextflow lint results

- Generated: 2026-02-13T00:25:10.829169+00:00
- Nextflow version: 26.01.1-edge
- Summary: 4 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_split_by_region/main.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_split_by_region/main.nf:23:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, bam, bai, regions_file ->
                    ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_split_by_region/main.nf:23:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              meta, bam, bai, regions_file ->
                         ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_split_by_region/main.nf:50:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, bam, bai, regions, chrom -> [ meta + [ genomic_region:chrom ], bam, bai ] }
                                ^^^^^^^^^^
  ```
