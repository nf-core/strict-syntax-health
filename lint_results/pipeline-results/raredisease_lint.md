# Nextflow lint results

- Generated: 2026-07-18T00:27:17.986241215Z
- Nextflow version: 26.07.0-edge
- Summary: 9 warnings

## :warning: Warnings

- Warning: `subworkflows/local/call_snv_sentieon/main.nf:67:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def sorted = [vcfs, idxs].transpose().sort { it[0].name }
                                                               ^^
  ```

- Warning: `subworkflows/local/call_snv_sentieon/main.nf:68:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  return [meta, sorted.collect { it[0] }, sorted.collect { it[1] }]
                                                 ^^
  ```

- Warning: `subworkflows/local/call_snv_sentieon/main.nf:68:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  return [meta, sorted.collect { it[0] }, sorted.collect { it[1] }]
                                                                           ^^
  ```

- Warning: `subworkflows/local/call_sv_MT/main.nf:145:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .filter { !it.isEmpty() }
                             ^^
  ```

- Warning: `subworkflows/local/contamination/main.nf:58:65`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_variants_vcf = ch_contamination_sites.map { vcf, tbi -> vcf }.collect()
                                                                  ^^^
  ```

- Warning: `subworkflows/local/contamination/main.nf:59:60`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              ch_variants_tbi = ch_contamination_sites.map { vcf, tbi -> tbi }.collect()
                                                             ^^^
  ```

- Warning: `workflows/raredisease.nf:1132:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_config        = channel.fromPath(
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/raredisease.nf:1134:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_custom_config = val_multiqc_config ?
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/raredisease.nf:1137:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_logo          = val_multiqc_logo ?
      ^^^^^^^^^^^^^^^
  ```
