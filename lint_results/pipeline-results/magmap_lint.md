# Nextflow lint results

- Generated: 2026-09-17T00:19:47.561066158Z
- Nextflow version: 26.08.0-edge
- Summary: 13 warnings

## :warning: Warnings

- Warning: `subworkflows/local/sourmash/main.nf:144:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              .splitText() { it.trim() }
                                             ^^
  ```

- Warning: `subworkflows/local/sourmash/main.nf:145:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              .filter { it }
                                        ^^
  ```

- Warning: `subworkflows/local/sourmash/main.nf:154:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              .splitText() { it.trim() }
                                             ^^
  ```

- Warning: `subworkflows/local/sourmash/main.nf:155:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                              .filter { it }
                                        ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_magmap_pipeline/main.nf:55:5`: Variable was declared but not used

  ```nextflow
      ch_versions = channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `workflows/magmap.nf:253:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .splitText() { it.trim() }
                             ^^
  ```

- Warning: `workflows/magmap.nf:254:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it }
                        ^^
  ```

- Warning: `workflows/magmap.nf:267:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .splitText() { it.trim() }
                                     ^^
  ```

- Warning: `workflows/magmap.nf:268:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { it }
                                ^^
  ```

- Warning: `workflows/magmap.nf:276:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .splitText() { it.trim() }
                                     ^^
  ```

- Warning: `workflows/magmap.nf:277:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { it }
                                ^^
  ```

- Warning: `workflows/magmap.nf:335:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { pairs -> [ [ id: 'all' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                   ^^
  ```

- Warning: `workflows/magmap.nf:335:91`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { pairs -> [ [ id: 'all' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                                            ^^
  ```
