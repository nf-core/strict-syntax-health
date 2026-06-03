# Nextflow lint results

- Generated: 2026-06-03T00:52:00.920945533Z
- Nextflow version: 26.04.3
- Summary: 50 warnings

## :warning: Warnings

- Warning: `main.nf:54:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = PHYLOPLACE.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/local/hmmer/hmmextract/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      phyloplace_input  //  string: Path to phyloplace input samplesheet
      ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      phylosearch_input //  string: Path to phylosearch input samplesheet
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:123:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          id: it.target,
                              ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:124:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          min_bitscore: it.min_bitscore
                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:127:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          alignmethod:    it.alignmethod  ? it.alignmethod                             : 'hmmer',
                                          ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:127:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          alignmethod:    it.alignmethod  ? it.alignmethod                             : 'hmmer',
                                                            ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:128:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          hmm:            file(it.hmm,  checkIfExists: true),
                                               ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:129:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          extract_hmm:    it.extract_hmm,
                                          ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:130:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          refseqfile:     it.refseqfile   ? file(it.refseqfile,   checkIfExists: true) : [],
                                          ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:130:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          refseqfile:     it.refseqfile   ? file(it.refseqfile,   checkIfExists: true) : [],
                                                                 ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:131:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          refphylogeny:   it.refphylogeny ? file(it.refphylogeny, checkIfExists: true) : [],
                                          ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:131:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          refphylogeny:   it.refphylogeny ? file(it.refphylogeny, checkIfExists: true) : [],
                                                                 ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:132:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          model:          it.model,
                                          ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:133:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          taxonomy:       it.taxonomy     ? file(it.taxonomy,     checkIfExists: true) : []
                                          ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:133:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          taxonomy:       it.taxonomy     ? file(it.taxonomy,     checkIfExists: true) : []
                                                                 ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:144:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      meta: [ id: it.sample ],
                                  ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:146:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          alignmethod:  it.alignmethod ? it.alignmethod    : 'hmmer',
                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:146:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          alignmethod:  it.alignmethod ? it.alignmethod    : 'hmmer',
                                                         ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:147:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          queryseqfile: file(it.queryseqfile),
                                             ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:148:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          refseqfile:   file(it.refseqfile),
                                             ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:149:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          hmmfile:      it.hmmfile     ? file(it.hmmfile,  checkIfExists: true) : [],
                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:149:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          hmmfile:      it.hmmfile     ? file(it.hmmfile,  checkIfExists: true) : [],
                                                              ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:150:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          refphylogeny: file(it.refphylogeny),
                                             ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:151:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          model:        it.model,
                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:152:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          taxonomy:     it.taxonomy    ? file(it.taxonomy, checkIfExists: true) : []
                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_phyloplace_pipeline/main.nf:152:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                          taxonomy:     it.taxonomy    ? file(it.taxonomy, checkIfExists: true) : []
                                                              ^^
  ```

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      valid_config = valid_config
      ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:76:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/phyloplace.nf:42:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it.data.extract_hmm }
                    ^^
  ```

- Warning: `workflows/phyloplace.nf:43:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [ it.meta, it.data.hmm, it.data.extract_hmm ] }
                   ^^
  ```

- Warning: `workflows/phyloplace.nf:43:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [ it.meta, it.data.hmm, it.data.extract_hmm ] }
                            ^^
  ```

- Warning: `workflows/phyloplace.nf:43:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { [ it.meta, it.data.hmm, it.data.extract_hmm ] }
                                         ^^
  ```

- Warning: `workflows/phyloplace.nf:52:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .filter { ! it.data.extract_hmm }
                              ^^
  ```

- Warning: `workflows/phyloplace.nf:53:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { [ it.meta, it.data.hmm ] }
                           ^^
  ```

- Warning: `workflows/phyloplace.nf:53:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { [ it.meta, it.data.hmm ] }
                                    ^^
  ```

- Warning: `workflows/phyloplace.nf:62:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .filter { it.data.alignmethod && it.data.refseqfile && it.data.refphylogeny }
                            ^^
  ```

- Warning: `workflows/phyloplace.nf:62:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .filter { it.data.alignmethod && it.data.refseqfile && it.data.refphylogeny }
                                                   ^^
  ```

- Warning: `workflows/phyloplace.nf:62:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .filter { it.data.alignmethod && it.data.refseqfile && it.data.refphylogeny }
                                                                         ^^
  ```

- Warning: `workflows/phyloplace.nf:63:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { [ [ id: it.meta.id ], it ] }
                                 ^^
  ```

- Warning: `workflows/phyloplace.nf:63:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { [ [ id: it.meta.id ], it ] }
                                               ^^
  ```

- Warning: `workflows/phyloplace.nf:66:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              meta: it[2].meta,
                    ^^
  ```

- Warning: `workflows/phyloplace.nf:68:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  alignmethod: it[2].data.alignmethod,
                               ^^
  ```

- Warning: `workflows/phyloplace.nf:69:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  queryseqfile: it[1],
                                ^^
  ```

- Warning: `workflows/phyloplace.nf:70:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  refseqfile: it[2].data.refseqfile,
                              ^^
  ```

- Warning: `workflows/phyloplace.nf:71:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  refphylogeny: it[2].data.refphylogeny,
                                ^^
  ```

- Warning: `workflows/phyloplace.nf:72:24`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  model: it[2].data.model,
                         ^^
  ```

- Warning: `workflows/phyloplace.nf:73:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  taxonomy: it[2].data.taxonomy
                            ^^
  ```
