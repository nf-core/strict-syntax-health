# Nextflow lint results

- Generated: 2026-03-18T00:26:52.649787238Z
- Nextflow version: 26.02.0-edge
- Summary: 1 error, 3 warnings

## :x: Errors

- Error: `tests/nextflow.config:28:27`: `SENTIEON_AUTH_MECH` is not defined (hint: use `env('...')` to access environment variable)

  ```nextflow
      SENTIEON_AUTH_MECH = "$SENTIEON_AUTH_MECH"
                            ^^^^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `main.nf:604:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          path { destination, value -> destination }
                              ^^^^^
  ```

- Warning: `subworkflows/local/annotate_structural_variants/main.nf:100:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .mix(ENSEMBLVEP_SV.out.report.map{ meta, process, vep, html -> return [meta, html] })
                                                       ^^^^^^^
  ```

- Warning: `subworkflows/local/annotate_structural_variants/main.nf:100:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .mix(ENSEMBLVEP_SV.out.report.map{ meta, process, vep, html -> return [meta, html] })
                                                                ^^^
  ```
