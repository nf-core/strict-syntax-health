# Nextflow lint results

- Generated: 2026-08-13T00:19:36.982328664Z
- Nextflow version: 26.07.0-edge
- Summary: 24 warnings

## :warning: Warnings

- Warning: `modules/local/savont_export.nf:20:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
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

- Warning: `workflows/ampliseq.nf:822:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_dada2_tax.map { it = [ [database:val_dada_ref_taxonomy, classifier:"DADA2"], file(it) ] } )
                                                          ^^
  ```

- Warning: `workflows/ampliseq.nf:822:123`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_dada2_tax.map { it = [ [database:val_dada_ref_taxonomy, classifier:"DADA2"], file(it) ] } )
                                                                                                                            ^^
  ```

- Warning: `workflows/ampliseq.nf:837:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( KRAKEN2_TAXONOMY_WF.out.tax_tsv.map { it = [ [database:val_kraken2_ref_taxonomy, classifier:"KRAKEN2"], file(it) ] } )
                                                                             ^^
  ```

- Warning: `workflows/ampliseq.nf:837:147`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( KRAKEN2_TAXONOMY_WF.out.tax_tsv.map { it = [ [database:val_kraken2_ref_taxonomy, classifier:"KRAKEN2"], file(it) ] } )
                                                                                                                                                    ^^
  ```

- Warning: `workflows/ampliseq.nf:853:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_sintax_tax.map { it = [ [database:val_sintax_ref_taxonomy, classifier:"SINTAX"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:853:127`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_sintax_tax.map { it = [ [database:val_sintax_ref_taxonomy, classifier:"SINTAX"], file(it) ] } )
                                                                                                                                ^^
  ```

- Warning: `workflows/ampliseq.nf:871:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_vsearch_lca_tax.map { it = [ [database:val_vsearch_lca_ref_taxonomy, classifier:"VSEARCH-LCA"], file(it) ] } )
                                                                ^^
  ```

- Warning: `workflows/ampliseq.nf:871:142`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_vsearch_lca_tax.map { it = [ [database:val_vsearch_lca_ref_taxonomy, classifier:"VSEARCH-LCA"], file(it) ] } )
                                                                                                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:902:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database: params.pplace_name ?: 'user_tree', classifier:"PPLACE"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:902:138`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database: params.pplace_name ?: 'user_tree', classifier:"PPLACE"], file(it) ] } )
                                                                                                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:966:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database:"PPLACE", classifier:"PPLACE"], file(it) ] } )
                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:966:116`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database:"PPLACE", classifier:"PPLACE"], file(it) ] } )
                                                                                                                     ^^
  ```

- Warning: `workflows/ampliseq.nf:986:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_qiime2_tax.map { it = [ [database:val_qiime_ref_taxonomy, classifier:"QIIME2"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:986:126`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_qiime2_tax.map { it = [ [database:val_qiime_ref_taxonomy, classifier:"QIIME2"], file(it) ] } )
                                                                                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:1193:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def val_params_string = params.findAll{ it.key != 'trace_report_suffix' }.toString()
                                                  ^^
  ```
