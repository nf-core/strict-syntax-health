# Nextflow lint results

- Generated: 2026-08-01T00:29:23.712321354Z
- Nextflow version: 26.07.0-edge
- Summary: 1 error, 12 warnings

## :x: Errors

- Error: `main.nf:40:5`: Incorrect number of call arguments, expected 0 but received 2

  ```nextflow
      DAAMICROBIOME (
      ^
  ```

## :warning: Warnings

- Warning: `modules/local/apply_weighted_consensus/main.nf:24:13`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
    Rscript ${projectDir}/bin/apply_weighted_consensus.R \
              ^^^^^^^^^^
  ```

- Warning: `modules/local/da_scoring/main.nf:27:13`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
    Rscript ${projectDir}/bin/run_scoring.R \
              ^^^^^^^^^^
  ```

- Warning: `modules/local/da_tools/metagenomeseq/main.nf:28:14`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
    Rscript "${projectDir}/bin/run_metagenomeseq.R" --input "${rds_file}" --output_dir "." \
               ^^^^^^^^^^
  ```

- Warning: `modules/local/da_tools_real/metagenomeseq_real/main.nf:39:14`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
    Rscript "${projectDir}/bin/run_metagenomeseq.R" --input "${rds_file}" --output_dir "." \
               ^^^^^^^^^^
  ```

- Warning: `modules/local/extract_control/main.nf:20:13`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
    Rscript ${projectDir}/bin/extract_control.R \
              ^^^^^^^^^^
  ```

- Warning: `modules/local/k_intersection/main.nf:25:13`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
    Rscript ${projectDir}/bin/run_k_intersection.R \
              ^^^^^^^^^^
  ```

- Warning: `modules/local/simulation/main.nf:36:13`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
    Rscript ${projectDir}/bin/run_simulation.R \
              ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/differentiaL_abundance_real/main.nf:58:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
            params.tool_locom, params.tool_maaslin2, params.tool_metagenomeseq].any { it }) {
                                                                                      ^^
  ```

- Warning: `subworkflows/local/differential_abundance/main.nf:18:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      results = Channel.empty()
                ^^^^^^^
  ```

- Warning: `subworkflows/local/differential_abundance/main.nf:58:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
            params.tool_locom, params.tool_maaslin2, params.tool_metagenomeseq].any { it }) {
                                                                                      ^^
  ```

- Warning: `workflows/daamicrobiome.nf:67:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { rid, tool, p -> tuple(rid, p) }
                          ^^^^
  ```

- Warning: `workflows/daamicrobiome.nf:126:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          def real_da_root_ch = real_ch.map { rid, rds ->
                                                   ^^^
  ```
