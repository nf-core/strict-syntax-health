# Nextflow lint results

- Generated: 2026-10-08T00:20:39.033795546Z
- Nextflow version: 26.09.2-edge
- Summary: 35 warnings

## :warning: Warnings

- Warning: `modules/local/summary_report/main.nf:90:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              dada_ref_taxonomy_list.collect { params.dada_ref_databases[it]["title"] }.join('; ') :
                                                                        ^^
  ```

- Warning: `modules/local/summary_report/main.nf:93:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          dada_ref_taxonomy_list.collect { params.dada_ref_databases[it]["file"] }.flatten().join(', ') :
                                                                    ^^
  ```

- Warning: `modules/local/summary_report/main.nf:96:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          dada_ref_taxonomy_list.collect { params.dada_ref_databases[it]["citation"] }.join(' | ') :
                                                                    ^^
  ```

- Warning: `subworkflows/local/comparison_wf/main.nf:24:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_observed_sequences.map { it = [ [id: val_md5sum_version], file(it) ] },
                                      ^^
  ```

- Warning: `subworkflows/local/comparison_wf/main.nf:24:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_observed_sequences.map { it = [ [id: val_md5sum_version], file(it) ] },
                                                                            ^^
  ```

- Warning: `subworkflows/local/comparison_wf/main.nf:47:45`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          COMPARE_SEQUENCES.out.matches.map { it = [ [id: val_md5sum_version], file(it) ] },
                                              ^^
  ```

- Warning: `subworkflows/local/comparison_wf/main.nf:47:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          COMPARE_SEQUENCES.out.matches.map { it = [ [id: val_md5sum_version], file(it) ] },
                                                                                    ^^
  ```

- Warning: `subworkflows/local/comparison_wf/main.nf:57:20`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { it = [ [id: val_md5sum_version], it ] },
                     ^^
  ```

- Warning: `subworkflows/local/comparison_wf/main.nf:57:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { it = [ [id: val_md5sum_version], it ] },
                                                      ^^
  ```

- Warning: `subworkflows/local/dada2_preprocessing/main.nf:54:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .findAll { it.trim() }  // Remove empty lines
                                 ^^
  ```

- Warning: `subworkflows/local/dada2_preprocessing/main.nf:55:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .collect { it.trim().toInteger() }
                                 ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ampliseq_pipeline/main.nf:517:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def collisions = filesToKeys.values().findAll { it.size() > 1 }
                                                          ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ampliseq_pipeline/main.nf:520:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  collisions.collect { "'${it.join("', '")}'" }.join(", ") + ". List each database only once.")
                                           ^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:35:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { pairs -> pairs.sort { it[0] } }
                                       ^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:36:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { pairs -> [ [ id: 'rank.tblout' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                   ^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:36:91`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { pairs -> [ [ id: 'rank.tblout' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                                            ^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:52:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { pairs -> pairs.sort { it[0] } }
                                           ^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:53:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { pairs -> [ [ id: 'rank.domtblout' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                          ^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:53:98`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { pairs -> [ [ id: 'rank.domtblout' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                                                   ^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:59:81`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_domtblout_parquet = DUCKDB_TABLE2PARQUET_DOMTBLOUT.out.parquet.map { meta, parquet -> parquet }
                                                                                  ^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:61:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_domtblout_parquet = Channel.value([])
                                 ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_hmmsearch_rank_fastas/main.nf:68:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, parquet -> [ [ id: 'rank' ], parquet ] }
                 ^^^^
  ```

- Warning: `workflows/ampliseq.nf:906:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( KRAKEN2_TAXONOMY_WF.out.tax_tsv.map { it = [ [database:val_kraken2_ref_taxonomy, classifier:"KRAKEN2"], file(it) ] } )
                                                                             ^^
  ```

- Warning: `workflows/ampliseq.nf:906:147`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( KRAKEN2_TAXONOMY_WF.out.tax_tsv.map { it = [ [database:val_kraken2_ref_taxonomy, classifier:"KRAKEN2"], file(it) ] } )
                                                                                                                                                    ^^
  ```

- Warning: `workflows/ampliseq.nf:922:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_sintax_tax.map { it = [ [database:val_sintax_ref_taxonomy, classifier:"SINTAX"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:922:127`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_sintax_tax.map { it = [ [database:val_sintax_ref_taxonomy, classifier:"SINTAX"], file(it) ] } )
                                                                                                                                ^^
  ```

- Warning: `workflows/ampliseq.nf:940:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_vsearch_lca_tax.map { it = [ [database:val_vsearch_lca_ref_taxonomy, classifier:"VSEARCH-LCA"], file(it) ] } )
                                                                ^^
  ```

- Warning: `workflows/ampliseq.nf:940:142`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_vsearch_lca_tax.map { it = [ [database:val_vsearch_lca_ref_taxonomy, classifier:"VSEARCH-LCA"], file(it) ] } )
                                                                                                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:970:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database: params.pplace_name ?: 'user_tree', classifier:"PPLACE"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:970:138`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database: params.pplace_name ?: 'user_tree', classifier:"PPLACE"], file(it) ] } )
                                                                                                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:1032:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database:"PPLACE", classifier:"PPLACE"], file(it) ] } )
                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:1032:116`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database:"PPLACE", classifier:"PPLACE"], file(it) ] } )
                                                                                                                     ^^
  ```

- Warning: `workflows/ampliseq.nf:1052:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_qiime2_tax.map { it = [ [database:val_qiime_ref_taxonomy, classifier:"QIIME2"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:1052:126`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_qiime2_tax.map { it = [ [database:val_qiime_ref_taxonomy, classifier:"QIIME2"], file(it) ] } )
                                                                                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:1295:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def val_params_string = params.findAll{ it.key != 'trace_report_suffix' }.toString()
                                                  ^^
  ```
