# Nextflow lint results

- Generated: 2026-07-28T00:31:31.282805655Z
- Nextflow version: 26.07.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_phaseimpute_pipeline/main.nf:923:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  def toolBibliographyText(steps, tools, compute_freq, phase) {
                                         ^^^^^^^^^^^^
  ```
