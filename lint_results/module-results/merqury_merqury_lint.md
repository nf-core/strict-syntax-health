# Nextflow lint results

- Generated: 2026-02-19T00:24:59.392127+00:00
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/merqury/merqury/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def VERSION = 1.3 // WARN: Version information not provided by tool on CLI. Please update this string when bumping container versions.
          ^^^^^^^^^^
  ```
