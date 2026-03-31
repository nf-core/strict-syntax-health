# Nextflow lint results

- Generated: 2026-03-31T00:29:12.671595573Z
- Nextflow version: 26.03.1-edge
- Summary: 1 error, 5 warnings

## :x: Errors

- Error: `subworkflows/local/call_sv_MT/main.nf:145:48`: `_` is not allowed as an identifier because it is reserved for future use

  ```nextflow
                  .concat(ch_saltshaker_vcf.map{ _ -> ["mitosalt"] })
                                                 ^
  ```

## :warning: Warnings

- Warning: `main.nf:666:29`: Parameter was not used -- prefix with `_` to suppress warning

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

- Warning: `subworkflows/local/call_sv_cnvnator/main.nf:20:9`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fai       // channel: [mandatory] [ val(meta), path(fai) ]
          ^^^^^^
  ```

- Warning: `subworkflows/local/qc_bam/main.nf:22:9`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_bam                          // channel: [mandatory] [ val(meta), path(bam) ]
          ^^^^^^
  ```
