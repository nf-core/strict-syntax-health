# Nextflow lint results

- Generated: 2026-09-22T00:25:31.472697401Z
- Nextflow version: 26.08.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/plasmidid/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args   ?: ''
          ^^^^
  ```

- Warning: `workflows/viralrecon.nf:104:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      outdir
      ^^^^^^
  ```
