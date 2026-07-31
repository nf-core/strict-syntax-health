# Nextflow lint results

- Generated: 2026-07-31T00:32:20.100216677Z
- Nextflow version: 26.07.0-edge
- Summary: 13 warnings

## :warning: Warnings

- Warning: `subworkflows/local/sourmash/main.nf:140:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              .splitText() { it.trim() }
                                             ^^
  ```

- Warning: `subworkflows/local/sourmash/main.nf:141:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              .filter { it }
                                        ^^
  ```

- Warning: `subworkflows/local/sourmash/main.nf:150:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              .splitText() { it.trim() }
                                             ^^
  ```

- Warning: `subworkflows/local/sourmash/main.nf:151:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              .filter { it }
                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_magmap_pipeline/main.nf:53:5`: Variable was declared but not used

  ```nextflow
      ch_versions = channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `workflows/magmap.nf:248:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .splitText() { it.trim() }
                             ^^
  ```

- Warning: `workflows/magmap.nf:249:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it }
                        ^^
  ```

- Warning: `workflows/magmap.nf:262:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .splitText() { it.trim() }
                                     ^^
  ```

- Warning: `workflows/magmap.nf:263:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { it }
                                ^^
  ```

- Warning: `workflows/magmap.nf:271:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .splitText() { it.trim() }
                                     ^^
  ```

- Warning: `workflows/magmap.nf:272:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { it }
                                ^^
  ```

- Warning: `workflows/magmap.nf:330:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { pairs -> [ [ id: 'all' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                   ^^
  ```

- Warning: `workflows/magmap.nf:330:91`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { pairs -> [ [ id: 'all' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                                            ^^
  ```
