# Nextflow lint results

- Generated: 2026-09-19T00:22:16.115674947Z
- Nextflow version: 26.08.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_phaseimpute_pipeline/main.nf:928:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  def toolBibliographyText(steps, tools, compute_freq, phase) {
                                         ^^^^^^^^^^^^
  ```
