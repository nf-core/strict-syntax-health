# Nextflow lint results

- Generated: 2026-09-26T00:19:30.204688499Z
- Nextflow version: 26.09.1-edge
- Summary: 26 warnings

## :warning: Warnings

- Warning: `modules/local/summary_report.nf:90:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              dada_ref_taxonomy_list.collect { params.dada_ref_databases[it]["title"] }.join('; ') :
                                                                        ^^
  ```

- Warning: `modules/local/summary_report.nf:93:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          dada_ref_taxonomy_list.collect { params.dada_ref_databases[it]["file"] }.flatten().join(', ') :
                                                                    ^^
  ```

- Warning: `modules/local/summary_report.nf:96:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          dada_ref_taxonomy_list.collect { params.dada_ref_databases[it]["citation"] }.join(' | ') :
                                                                    ^^
  ```

- Warning: `subworkflows/local/comparison_wf.nf:24:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_observed_sequences.map { it = [ [id: val_md5sum_version], file(it) ] },
                                      ^^
  ```

- Warning: `subworkflows/local/comparison_wf.nf:24:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_observed_sequences.map { it = [ [id: val_md5sum_version], file(it) ] },
                                                                            ^^
  ```

- Warning: `subworkflows/local/comparison_wf.nf:47:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          COMPARE_SEQUENCES.out.matches.map { it = [ [id: val_md5sum_version], file(it) ] },
                                              ^^
  ```

- Warning: `subworkflows/local/comparison_wf.nf:47:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          COMPARE_SEQUENCES.out.matches.map { it = [ [id: val_md5sum_version], file(it) ] },
                                                                                    ^^
  ```

- Warning: `subworkflows/local/comparison_wf.nf:57:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { it = [ [id: val_md5sum_version], it ] },
                     ^^
  ```

- Warning: `subworkflows/local/comparison_wf.nf:57:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { it = [ [id: val_md5sum_version], it ] },
                                                      ^^
  ```

- Warning: `subworkflows/local/dada2_preprocessing.nf:54:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .findAll { it.trim() }  // Remove empty lines
                                 ^^
  ```

- Warning: `subworkflows/local/dada2_preprocessing.nf:55:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .collect { it.trim().toInteger() }
                                 ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ampliseq_pipeline/main.nf:505:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def collisions = filesToKeys.values().findAll { it.size() > 1 }
                                                          ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ampliseq_pipeline/main.nf:508:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  collisions.collect { "'${it.join("', '")}'" }.join(", ") + ". List each database only once.")
                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:910:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( KRAKEN2_TAXONOMY_WF.out.tax_tsv.map { it = [ [database:val_kraken2_ref_taxonomy, classifier:"KRAKEN2"], file(it) ] } )
                                                                             ^^
  ```

- Warning: `workflows/ampliseq.nf:910:147`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( KRAKEN2_TAXONOMY_WF.out.tax_tsv.map { it = [ [database:val_kraken2_ref_taxonomy, classifier:"KRAKEN2"], file(it) ] } )
                                                                                                                                                    ^^
  ```

- Warning: `workflows/ampliseq.nf:926:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_sintax_tax.map { it = [ [database:val_sintax_ref_taxonomy, classifier:"SINTAX"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:926:127`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_sintax_tax.map { it = [ [database:val_sintax_ref_taxonomy, classifier:"SINTAX"], file(it) ] } )
                                                                                                                                ^^
  ```

- Warning: `workflows/ampliseq.nf:944:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_vsearch_lca_tax.map { it = [ [database:val_vsearch_lca_ref_taxonomy, classifier:"VSEARCH-LCA"], file(it) ] } )
                                                                ^^
  ```

- Warning: `workflows/ampliseq.nf:944:142`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_vsearch_lca_tax.map { it = [ [database:val_vsearch_lca_ref_taxonomy, classifier:"VSEARCH-LCA"], file(it) ] } )
                                                                                                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:975:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database: params.pplace_name ?: 'user_tree', classifier:"PPLACE"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:975:138`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database: params.pplace_name ?: 'user_tree', classifier:"PPLACE"], file(it) ] } )
                                                                                                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:1039:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database:"PPLACE", classifier:"PPLACE"], file(it) ] } )
                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:1039:116`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database:"PPLACE", classifier:"PPLACE"], file(it) ] } )
                                                                                                                     ^^
  ```

- Warning: `workflows/ampliseq.nf:1059:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_qiime2_tax.map { it = [ [database:val_qiime_ref_taxonomy, classifier:"QIIME2"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:1059:126`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_qiime2_tax.map { it = [ [database:val_qiime_ref_taxonomy, classifier:"QIIME2"], file(it) ] } )
                                                                                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:1304:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def val_params_string = params.findAll{ it.key != 'trace_report_suffix' }.toString()
                                                  ^^
  ```
