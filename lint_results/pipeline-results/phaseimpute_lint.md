# Nextflow lint results

- Generated: 2026-04-01T00:28:59.969586Z
- Nextflow version: 26.03.1-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `modules/nf-core/custom/geneticmapconvert/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      args = task.ext.args ?: ''
      ^^^^
  ```

- Warning: `workflows/phaseimpute/main.nf:129:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, map_file ->
                    ^^^^
  ```

- Warning: `workflows/phaseimpute/main.nf:309:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          if (params.tools.split(',').any{ it in ["stitch", "quilt"] }) {
                                           ^^
  ```
