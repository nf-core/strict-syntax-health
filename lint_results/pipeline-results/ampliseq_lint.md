# Nextflow lint results

- Generated: 2026-08-06T00:25:24.244776567Z
- Nextflow version: 26.07.0-edge
- Summary: 22 warnings

## :warning: Warnings

- Warning: `modules/local/savont_export.nf:20:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/comparison_wf.nf:21:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_observed_sequences.map { it = [ [id: val_md5sum_version], file(it) ] },
                                      ^^
  ```

- Warning: `subworkflows/local/comparison_wf.nf:21:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_observed_sequences.map { it = [ [id: val_md5sum_version], file(it) ] },
                                                                            ^^
  ```

- Warning: `subworkflows/local/comparison_wf.nf:35:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      COMPARE_PERFORMANCE ( COMPARE_SEQUENCES.out.matches.map { it = [ [id: val_md5sum_version], file(it) ] }, ch_observed_abundances, ch_expected_abundances )
                                                                ^^
  ```

- Warning: `subworkflows/local/comparison_wf.nf:35:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      COMPARE_PERFORMANCE ( COMPARE_SEQUENCES.out.matches.map { it = [ [id: val_md5sum_version], file(it) ] }, ch_observed_abundances, ch_expected_abundances )
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

- Warning: `workflows/ampliseq.nf:845:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_dada2_tax.map { it = [ [database:val_dada_ref_taxonomy, classifier:"DADA2"], file(it) ] } )
                                                          ^^
  ```

- Warning: `workflows/ampliseq.nf:845:123`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_dada2_tax.map { it = [ [database:val_dada_ref_taxonomy, classifier:"DADA2"], file(it) ] } )
                                                                                                                            ^^
  ```

- Warning: `workflows/ampliseq.nf:860:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( KRAKEN2_TAXONOMY_WF.out.tax_tsv.map { it = [ [database:val_kraken2_ref_taxonomy, classifier:"KRAKEN2"], file(it) ] } )
                                                                             ^^
  ```

- Warning: `workflows/ampliseq.nf:860:147`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( KRAKEN2_TAXONOMY_WF.out.tax_tsv.map { it = [ [database:val_kraken2_ref_taxonomy, classifier:"KRAKEN2"], file(it) ] } )
                                                                                                                                                    ^^
  ```

- Warning: `workflows/ampliseq.nf:876:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_sintax_tax.map { it = [ [database:val_sintax_ref_taxonomy, classifier:"SINTAX"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:876:127`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_sintax_tax.map { it = [ [database:val_sintax_ref_taxonomy, classifier:"SINTAX"], file(it) ] } )
                                                                                                                                ^^
  ```

- Warning: `workflows/ampliseq.nf:894:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_vsearch_lca_tax.map { it = [ [database:val_vsearch_lca_ref_taxonomy, classifier:"VSEARCH-LCA"], file(it) ] } )
                                                                ^^
  ```

- Warning: `workflows/ampliseq.nf:894:142`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_vsearch_lca_tax.map { it = [ [database:val_vsearch_lca_ref_taxonomy, classifier:"VSEARCH-LCA"], file(it) ] } )
                                                                                                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:925:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database: params.pplace_name ?: 'user_tree', classifier:"PPLACE"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:925:138`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database: params.pplace_name ?: 'user_tree', classifier:"PPLACE"], file(it) ] } )
                                                                                                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:989:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database:"PPLACE", classifier:"PPLACE"], file(it) ] } )
                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:989:116`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database:"PPLACE", classifier:"PPLACE"], file(it) ] } )
                                                                                                                     ^^
  ```

- Warning: `workflows/ampliseq.nf:1009:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_qiime2_tax.map { it = [ [database:val_qiime_ref_taxonomy, classifier:"QIIME2"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:1009:126`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_qiime2_tax.map { it = [ [database:val_qiime_ref_taxonomy, classifier:"QIIME2"], file(it) ] } )
                                                                                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:1216:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def val_params_string = params.findAll{ it.key != 'trace_report_suffix' }.toString()
                                                  ^^
  ```
