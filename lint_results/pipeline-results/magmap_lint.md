# Nextflow lint results

- Generated: 2026-08-11T00:15:57.835522888Z
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

- Warning: `subworkflows/local/utils_nfcore_magmap_pipeline/main.nf:55:5`: Variable was declared but not used

  ```nextflow
      ch_versions = channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `workflows/magmap.nf:250:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .splitText() { it.trim() }
                             ^^
  ```

- Warning: `workflows/magmap.nf:251:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it }
                        ^^
  ```

- Warning: `workflows/magmap.nf:264:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .splitText() { it.trim() }
                                     ^^
  ```

- Warning: `workflows/magmap.nf:265:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { it }
                                ^^
  ```

- Warning: `workflows/magmap.nf:273:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .splitText() { it.trim() }
                                     ^^
  ```

- Warning: `workflows/magmap.nf:274:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { it }
                                ^^
  ```

- Warning: `workflows/magmap.nf:332:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { pairs -> [ [ id: 'all' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                   ^^
  ```

- Warning: `workflows/magmap.nf:332:91`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { pairs -> [ [ id: 'all' ], pairs.collect { it[0] }, pairs.collect { it[1] } ] }
                                                                                            ^^
  ```
