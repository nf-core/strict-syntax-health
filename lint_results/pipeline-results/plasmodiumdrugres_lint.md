# Nextflow lint results

- Generated: 2026-08-15T00:12:00.720102373Z
- Nextflow version: 26.07.0-edge
- Summary: 20 warnings

## :warning: Warnings

- Warning: `modules/local/add_ref_seqs_with_full_genome_ref_fasta/main.nf:25:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      Rscript ${projectDir}/bin/PGEcore/scripts/add_ref_seq_to_ref_bed_table/add_ref_seqs_with_full_genome_ref_fasta.R \
                ^^^^^^^^^^
  ```

- Warning: `modules/local/add_ref_seqs_with_targeted_ref_fasta/main.nf:25:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      Rscript ${projectDir}/bin/PGEcore/scripts/add_ref_seq_to_ref_bed_table/add_ref_seqs_with_targeted_ref_fasta.R \
                ^^^^^^^^^^
  ```

- Warning: `modules/local/concat_tables/main.nf:29:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      Rscript ${projectDir}/bin/concat_tables.R \
                ^^^^^^^^^^
  ```

- Warning: `modules/local/dcifer_slaf_wrapper/main.nf:26:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      Rscript ${projectDir}/bin/PGEcore/scripts/dcifer_slaf_wrapper/dcifer_slaf_wrapper.R \
                ^^^^^^^^^^
  ```

- Warning: `modules/local/estimate_allele_frequency_naive/main.nf:25:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      Rscript ${projectDir}/bin/PGEcore/scripts/estimate_allele_frequency_naive/estimate_allele_frequency_naive.R \
                ^^^^^^^^^^
  ```

- Warning: `modules/local/estimate_allele_prevalence_naive/main.nf:24:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      Rscript ${projectDir}/bin/PGEcore/scripts/estimate_allele_prevalence_naive/estimate_allele_prevalence_naive.R \
                ^^^^^^^^^^
  ```

- Warning: `modules/local/estimate_multilocus_prevfreq_naive/main.nf:29:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      Rscript ${projectDir}/bin/PGEcore/scripts/multilocus_prevfreq_naive/multilocus_prevfreq_naive.R \
                ^^^^^^^^^^
  ```

- Warning: `modules/local/extract_population_map_from_pmo/main.nf:30:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      python3 ${projectDir}/bin/specimen_info_to_population_map.py \
                ^^^^^^^^^^
  ```

- Warning: `modules/local/fem_wrapper/main.nf:26:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      Rscript ${projectDir}/bin/PGEcore/scripts/FreqEstimationModel_wrapper/FreqEstimationModel_wrapper.R \\
                ^^^^^^^^^^
  ```

- Warning: `modules/local/idm_wrapper/main.nf:24:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      Rscript ${projectDir}/bin/PGEcore/scripts/IDM_wrapper/IDM_wrapper.R \\
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

- Warning: `modules/local/mlbm_wrapper/main.nf:27:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      Rscript ${projectDir}/bin/PGEcore/scripts/MultiLociBiallelicModel_wrapper/MultiLociBiallelicModel_wrapper.R \
                ^^^^^^^^^^
  ```

- Warning: `modules/local/slaf_from_mhaps_freqs/main.nf:26:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      Rscript ${projectDir}/bin/PGEcore/scripts/calc_slaf_based_on_mhap_freqs/slaf_from_mhaps_freqs.R \
                ^^^^^^^^^^
  ```

- Warning: `modules/local/slaf_from_stave_mlaf/main.nf:24:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      Rscript ${projectDir}/bin/PGEcore/scripts/slaf_from_stave_mlaf/slaf_from_stave_mlaf.R \\
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

- Warning: `modules/local/translate_loci_of_interest/main.nf:29:15`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      Rscript ${projectDir}/bin/PGEcore/scripts/translate_loci_of_interest/translate_loci_of_interest.R \
                ^^^^^^^^^^
  ```
