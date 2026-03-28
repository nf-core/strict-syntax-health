# Nextflow lint results

- Generated: 2026-03-28T00:24:04.678770+00:00
- Nextflow version: 26.03.1-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/dia_proteomics_analysis/main.nf:343:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              [meta + mass_settings, ms_files, [], [], speclib.unique{ it.name }, diann_quant]
                                                                       ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/dia_proteomics_analysis/main.nf:396:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              [meta, [], ms_files.collect{ f -> f.name}, fasta.unique{ it.name }, empirical_library.unique{ it.name }, diann_quant] // Use ms_file_names instead of ms_files for final quant; deduplicate shared files
                                                                       ^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/dia_proteomics_analysis/main.nf:396:107`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              [meta, [], ms_files.collect{ f -> f.name}, fasta.unique{ it.name }, empirical_library.unique{ it.name }, diann_quant] // Use ms_file_names instead of ms_files for final quant; deduplicate shared files
                                                                                                            ^^^^^^^^^^
  ```
