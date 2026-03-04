# Nextflow lint results

- Generated: 2026-03-04T00:21:21.300046622Z
- Nextflow version: 26.02.0-edge
- Summary: 4 warnings

## :warning: Warnings

- Warning: `modules/nf-core/stitch/main.nf:52:9`: Variable was declared but not used

  ```nextflow
      def rsync_version_cmd    = rdata ? "rsync: \$(rsync --version | head -n1 | sed 's/^rsync  version //; s/ .*\$//')" : ""
          ^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/stitch/main.nf:86:9`: Variable was declared but not used

  ```nextflow
      def rsync_version_cmd  = rdata ? "rsync: \$(rsync --version | head -n1 | sed 's/^rsync  version //; s/ .*\$//')" : ""
          ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/phaseimpute/main.nf:233:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  VCF_NORMALIZE_BCFTOOLS.out.vcf_tbi.map{ meta, vcf, index -> [meta, [], []]}, // No scaffold
                                                                ^^^
  ```

- Warning: `workflows/phaseimpute/main.nf:233:68`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  VCF_NORMALIZE_BCFTOOLS.out.vcf_tbi.map{ meta, vcf, index -> [meta, [], []]}, // No scaffold
                                                                     ^^^^^
  ```
