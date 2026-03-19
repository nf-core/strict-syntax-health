# Nextflow lint results

- Generated: 2026-03-19T00:24:36.192114144Z
- Nextflow version: 26.03.0-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `main.nf:604:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { destination, value -> destination }
                              ^^^^^
  ```

- Warning: `subworkflows/local/annotate_structural_variants/main.nf:98:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .mix(ENSEMBLVEP_SV.out.report.map{ meta, process, vep, html -> return [meta, html] })
                                                       ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_structural_variants/main.nf:98:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .mix(ENSEMBLVEP_SV.out.report.map{ meta, process, vep, html -> return [meta, html] })
                                                                ^^^
  ```
