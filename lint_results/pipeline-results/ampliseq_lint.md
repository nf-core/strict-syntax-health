# Nextflow lint results

- Generated: 2026-08-21T00:10:54.506214261Z
- Nextflow version: 26.08.0-edge
- Summary: 23 warnings

## :warning: Warnings

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

- Warning: `subworkflows/local/utils_nfcore_ampliseq_pipeline/main.nf:542:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def collisions = filesToKeys.values().findAll { it.size() > 1 }
                                                          ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ampliseq_pipeline/main.nf:545:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  collisions.collect { "'${it.join("', '")}'" }.join(", ") + ". List each database only once.")
                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:881:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( KRAKEN2_TAXONOMY_WF.out.tax_tsv.map { it = [ [database:val_kraken2_ref_taxonomy, classifier:"KRAKEN2"], file(it) ] } )
                                                                             ^^
  ```

- Warning: `workflows/ampliseq.nf:881:147`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( KRAKEN2_TAXONOMY_WF.out.tax_tsv.map { it = [ [database:val_kraken2_ref_taxonomy, classifier:"KRAKEN2"], file(it) ] } )
                                                                                                                                                    ^^
  ```

- Warning: `workflows/ampliseq.nf:897:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_sintax_tax.map { it = [ [database:val_sintax_ref_taxonomy, classifier:"SINTAX"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:897:127`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_sintax_tax.map { it = [ [database:val_sintax_ref_taxonomy, classifier:"SINTAX"], file(it) ] } )
                                                                                                                                ^^
  ```

- Warning: `workflows/ampliseq.nf:915:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_vsearch_lca_tax.map { it = [ [database:val_vsearch_lca_ref_taxonomy, classifier:"VSEARCH-LCA"], file(it) ] } )
                                                                ^^
  ```

- Warning: `workflows/ampliseq.nf:915:142`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_vsearch_lca_tax.map { it = [ [database:val_vsearch_lca_ref_taxonomy, classifier:"VSEARCH-LCA"], file(it) ] } )
                                                                                                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:946:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database: params.pplace_name ?: 'user_tree', classifier:"PPLACE"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:946:138`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database: params.pplace_name ?: 'user_tree', classifier:"PPLACE"], file(it) ] } )
                                                                                                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:1010:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database:"PPLACE", classifier:"PPLACE"], file(it) ] } )
                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:1010:116`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database:"PPLACE", classifier:"PPLACE"], file(it) ] } )
                                                                                                                     ^^
  ```

- Warning: `workflows/ampliseq.nf:1030:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_qiime2_tax.map { it = [ [database:val_qiime_ref_taxonomy, classifier:"QIIME2"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:1030:126`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_qiime2_tax.map { it = [ [database:val_qiime_ref_taxonomy, classifier:"QIIME2"], file(it) ] } )
                                                                                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:1243:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def val_params_string = params.findAll{ it.key != 'trace_report_suffix' }.toString()
                                                  ^^
  ```
