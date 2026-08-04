# Nextflow lint results

- Generated: 2026-08-04T00:33:03.533651499Z
- Nextflow version: 26.07.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `workflows/phyloplace.nf:29:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      text.readLines().collect { pad + it }.join('\n')
                                       ^^
  ```
