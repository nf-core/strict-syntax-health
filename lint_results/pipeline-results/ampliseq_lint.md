# Nextflow lint results

- Generated: 2026-10-29T00:14:37.487596571Z
- Nextflow version: 26.10.4
- Summary: 67 warnings

## :warning: Warnings

- Warning: `modules/local/build_asv_annotations/main.nf:28:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/decontam/main.nf:27:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/hmmer/hmmextract/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/summary_report/main.nf:91:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              dada_ref_taxonomy_list.collect { params.dada_ref_databases[it]["title"] }.join('; ') :
                                                                        ^^
  ```

- Warning: `modules/local/summary_report/main.nf:94:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          dada_ref_taxonomy_list.collect { params.dada_ref_databases[it]["file"] }.flatten().join(', ') :
                                                                    ^^
  ```

- Warning: `modules/local/summary_report/main.nf:97:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          dada_ref_taxonomy_list.collect { params.dada_ref_databases[it]["citation"] }.join(' | ') :
                                                                    ^^
  ```

- Warning: `modules/local/summary_table_counts/main.nf:16:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/summary_table_taxonomy/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/chopper/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/clustalo/align/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/cutadapt/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/duckdb/table2parquet/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/epang/place/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/epang/split/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fastqc/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gappa/examineassign/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gappa/examinegraft/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gappa/examineheattree/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hmmer/eslalimask/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hmmer/eslreformat/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hmmer/formattsv/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hmmer/hmmalign/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hmmer/hmmbuild/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hmmer/hmmrank/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/hmmer/hmmsearch/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/mafft/align/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pigz/uncompress/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/porechop/abi/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/seqtk/subseq/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/untar/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/vsearch/cluster/main.nf:29:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/vsearch/sintax/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/vsearch/usearchglobal/main.nf:29:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
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

- Warning: `subworkflows/local/utils_nfcore_ampliseq_pipeline/main.nf:536:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def collisions = filesToKeys.values().findAll { it.size() > 1 }
                                                          ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ampliseq_pipeline/main.nf:539:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

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

- Warning: `workflows/ampliseq.nf:920:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( KRAKEN2_TAXONOMY_WF.out.tax_tsv.map { it = [ [database:val_kraken2_ref_taxonomy, classifier:"KRAKEN2"], file(it) ] } )
                                                                             ^^
  ```

- Warning: `workflows/ampliseq.nf:920:147`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( KRAKEN2_TAXONOMY_WF.out.tax_tsv.map { it = [ [database:val_kraken2_ref_taxonomy, classifier:"KRAKEN2"], file(it) ] } )
                                                                                                                                                    ^^
  ```

- Warning: `workflows/ampliseq.nf:936:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_sintax_tax.map { it = [ [database:val_sintax_ref_taxonomy, classifier:"SINTAX"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:936:127`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_sintax_tax.map { it = [ [database:val_sintax_ref_taxonomy, classifier:"SINTAX"], file(it) ] } )
                                                                                                                                ^^
  ```

- Warning: `workflows/ampliseq.nf:955:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_vsearch_lca_tax.map { it = [ [database:val_vsearch_lca_ref_taxonomy, classifier:"VSEARCH-LCA"], file(it) ] } )
                                                                ^^
  ```

- Warning: `workflows/ampliseq.nf:955:142`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_vsearch_lca_tax.map { it = [ [database:val_vsearch_lca_ref_taxonomy, classifier:"VSEARCH-LCA"], file(it) ] } )
                                                                                                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:1003:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database: params.pplace_name ?: 'user_tree', classifier:"PPLACE"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:1003:138`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database: params.pplace_name ?: 'user_tree', classifier:"PPLACE"], file(it) ] } )
                                                                                                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:1065:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database:"PPLACE", classifier:"PPLACE"], file(it) ] } )
                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:1065:116`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_tax_tsv = ch_tax_tsv.mix( ch_pplace_tax.map { it = [ [database:"PPLACE", classifier:"PPLACE"], file(it) ] } )
                                                                                                                     ^^
  ```

- Warning: `workflows/ampliseq.nf:1085:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_qiime2_tax.map { it = [ [database:val_qiime_ref_taxonomy, classifier:"QIIME2"], file(it) ] } )
                                                           ^^
  ```

- Warning: `workflows/ampliseq.nf:1085:126`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_tax_tsv = ch_tax_tsv.mix( ch_qiime2_tax.map { it = [ [database:val_qiime_ref_taxonomy, classifier:"QIIME2"], file(it) ] } )
                                                                                                                               ^^
  ```

- Warning: `workflows/ampliseq.nf:1332:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def val_params_string = params.findAll{ it.key != 'trace_report_suffix' }.toString()
                                                  ^^
  ```
