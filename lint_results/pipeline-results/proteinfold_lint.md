# Nextflow lint results

- Generated: 2026-02-25T00:24:03.277972452Z
- Nextflow version: 26.01.1-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `conf/modules_boltz.config:63:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  saveAs: { filename -> "${meta.id}.pdb" },
                            ^^^^^^^^
  ```

- Warning: `modules/local/run_helixfold3/main.nf:107:9`: Variable was declared but not used

  ```nextflow
      def VERSION = '705c2974a833cdc3a4420f4e3379da596091c97f'
          ^^^^^^^
  ```
