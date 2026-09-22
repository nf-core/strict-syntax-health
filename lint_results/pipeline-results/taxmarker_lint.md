# Nextflow lint results

- Generated: 2026-09-22T00:25:05.802951875Z
- Nextflow version: 26.08.0-edge
- Summary: 17 warnings

## :warning: Warnings

- Warning: `subworkflows/local/ensure_aligned/main.nf:54:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      CHECKALIGNED(ch_sequences.map { [ [ id: 'user-alignment' ], it ] })
                                                                  ^^
  ```

- Warning: `subworkflows/local/ensure_aligned/main.nf:75:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { [ [ id: 'hmm' ], it ] }
                                      ^^
  ```

- Warning: `subworkflows/local/raxtax_prefilter/main.nf:35:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_meta_taxonomy   = ch_taxonomy.map  { [ [ id: 'user-alignment' ], it ] }
                                                                              ^^
  ```

- Warning: `subworkflows/local/raxtax_prefilter/main.nf:36:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_alignment_fasta = ch_alignment.map { [ [ id: 'user-alignment' ], it ] }
                                                                              ^^
  ```

- Warning: `subworkflows/local/sativa/main.nf:66:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_ref_tree   // channel: [ val(meta), path(tree.nwk) ]
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sativa/main.nf:69:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_ref_model  // channel: [ val(meta), path(model.txt) ]
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/sativa/main.nf:75:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_alignment_meta = ch_alignment.map { [ [ id: 'user-alignment' ], it ] }
                                                                             ^^
  ```

- Warning: `subworkflows/local/sativa/main.nf:89:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ch_taxonomy_meta = ch_taxonomy.map { [ [ id: 'user-alignment' ], it ] }
                                                                           ^^
  ```

- Warning: `subworkflows/local/sativa/main.nf:115:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_reference_input.map { meta, _alignment, _taxonomy, _taxcode, reftree, _refmodel -> reftree },
                                   ^^^^
  ```

- Warning: `subworkflows/local/sativa/main.nf:116:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_reference_input.map { meta, _alignment, _taxonomy, _taxcode, _reftree, refmodel -> refmodel }
                                   ^^^^
  ```

- Warning: `subworkflows/local/taxonomy2phylogeny/main.nf:11:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_taxonomy_alignment.map { meta, taxonomy, alignment, raxmlng_model -> [ meta, taxonomy ] }
                                                      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/taxonomy2phylogeny/main.nf:11:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_taxonomy_alignment.map { meta, taxonomy, alignment, raxmlng_model -> [ meta, taxonomy ] }
                                                                 ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/taxonomy2phylogeny/main.nf:20:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, taxonomy, alignment, raxmlng_model -> [ meta, alignment, raxmlng_model ] }
                       ^^^^^^^^
  ```

- Warning: `subworkflows/local/taxonomy2phylogeny/main.nf:27:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_search_input.map { meta, alignment, raxmlng_model, guide_tree -> guide_tree },
                                ^^^^
  ```

- Warning: `subworkflows/local/taxonomy2phylogeny/main.nf:27:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_search_input.map { meta, alignment, raxmlng_model, guide_tree -> guide_tree },
                                      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/taxonomy2phylogeny/main.nf:27:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_search_input.map { meta, alignment, raxmlng_model, guide_tree -> guide_tree },
                                                 ^^^^^^^^^^^^^
  ```

- Warning: `workflows/taxmarker.nf:121:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      EMBOSS_SEQRET(ch_sequences_checked.map { [ [ id: 'user-alignment' ], it ] }, 'fasta')
                                                                           ^^
  ```
