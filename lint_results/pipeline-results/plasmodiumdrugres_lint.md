# Nextflow lint results

- Generated: 2026-09-30T00:24:15.231534785Z
- Nextflow version: 26.09.1-edge
- Summary: 8 warnings

## :warning: Warnings

- Warning: `modules/local/concat_tables/main.nf:29:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      Rscript ${projectDir}/bin/concat_tables.R \
                ^^^^^^^^^^
  ```

- Warning: `modules/local/extract_population_map_from_pmo/main.nf:30:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      python3 ${projectDir}/bin/specimen_info_to_population_map.py \
                ^^^^^^^^^^
  ```

- Warning: `modules/local/index_population_assignment/main.nf:25:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      Rscript ${projectDir}/bin/index_population_assignment.R \
                ^^^^^^^^^^
  ```

- Warning: `modules/local/merge_tables/main.nf:40:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      Rscript ${projectDir}/bin/merge_tables.R --freq_table \${slaf_table} --population "\${true_population}" --prev_table \${slap_table} --output ${pop_index}.sl_summary.tsv
                ^^^^^^^^^^
  ```

- Warning: `modules/local/merge_tables/main.nf:42:19`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          Rscript ${projectDir}/bin/add_population_column.R --table \${mlaf_table} --population "\${true_population}" --output ${pop_index}.ml_summary.tsv
                    ^^^^^^^^^^
  ```

- Warning: `modules/local/merge_tables/main.nf:47:19`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          Rscript ${projectDir}/bin/add_population_column.R --table \${sl_from_ml_table} --population "\${true_population}" --output ${pop_index}.sl_from_ml_summary.tsv
                    ^^^^^^^^^^
  ```

- Warning: `modules/local/split_aa_table_by_population/main.nf:25:8`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
       ${projectDir}/bin/split_table_by_population_map.R \
         ^^^^^^^^^^
  ```

- Warning: `modules/local/split_allele_table_by_population/main.nf:28:7`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      ${projectDir}/bin/split_table_by_population_map.R \
        ^^^^^^^^^^
  ```
