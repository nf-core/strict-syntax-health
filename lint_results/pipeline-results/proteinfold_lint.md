# Nextflow lint results

- Generated: 2026-02-12T00:22:06.454219097Z
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `conf/modules_boltz.config:63:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  saveAs: { filename -> "${meta.id}.pdb" },
                            ^^^^^^^^
  ```
