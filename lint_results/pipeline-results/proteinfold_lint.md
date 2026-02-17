# Nextflow lint results

- Generated: 2026-02-17T00:23:04.108785328Z
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `conf/modules_boltz.config:63:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  saveAs: { filename -> "${meta.id}.pdb" },
                            ^^^^^^^^
  ```
