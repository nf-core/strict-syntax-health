# Nextflow lint results

- Generated: 2026-02-18T00:22:42.332104795Z
- Nextflow version: 26.01.1-edge
- Summary: 42 warnings

## :warning: Warnings

- Warning: `conf/modules.config:187:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> "${meta.id}_stardist_mask.tif" }
                        ^^^^^^^^
  ```

- Warning: `conf/modules.config:222:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename -> "${meta.id}_cellpose_mask.tif" }
                        ^^^^^^^^
  ```

- Warning: `modules/nf-core/cellpose/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/cellpose/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/stardist/main.nf:20:9`: Variable was declared but not used

  ```nextflow
      def prefix             = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/stardist/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args               = task.ext.args   ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_molkart_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_molkart_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_molkart_pipeline/main.nf:185:10`: Variable was declared but not used

  ```nextflow
      def (meta, files) = input
           ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_molkart_pipeline/main.nf:185:16`: Variable was declared but not used

  ```nextflow
      def (meta, files) = input
                 ^^^^^
  ```

- Warning: `workflows/molkart.nf:49:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[3] } // filter samples with membrane
                    ^^
  ```

- Warning: `workflows/molkart.nf:87:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def sorted = [tiffs, stains].transpose().sort { it[1] }
                                                              ^^
  ```

- Warning: `workflows/molkart.nf:94:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      grouped_map_stack.filter { !it[2] } // for rows without a present membrane image, set channel to no_stack
                                  ^^
  ```

- Warning: `workflows/molkart.nf:97:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      grouped_map_stack.filter{ it[2] }      // for rows where the membrane image is present, create a list of images to be stacked
                                ^^
  ```

- Warning: `workflows/molkart.nf:104:10`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          [it[0], it[1]]
           ^^
  ```

- Warning: `workflows/molkart.nf:104:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          [it[0], it[1]]
                  ^^
  ```

- Warning: `workflows/molkart.nf:118:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? tuple(it[0], 1) : tuple(it[0], 2)
                  ^^
  ```

- Warning: `workflows/molkart.nf:118:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? tuple(it[0], 1) : tuple(it[0], 2)
                                        ^^
  ```

- Warning: `workflows/molkart.nf:118:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? tuple(it[0], 1) : tuple(it[0], 2)
                                                          ^^
  ```

- Warning: `workflows/molkart.nf:129:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      tuple('matchkey', it[1])
                                        ^^
  ```

- Warning: `workflows/molkart.nf:130:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      }.groupTuple().map{ it[1]} )
                                          ^^
  ```

- Warning: `workflows/molkart.nf:148:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              grouped_map_stack.map{ tuple(it[0], it[1]) },
                                           ^^
  ```

- Warning: `workflows/molkart.nf:148:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              grouped_map_stack.map{ tuple(it[0], it[1]) },
                                                  ^^
  ```

- Warning: `workflows/molkart.nf:150:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? [[:],[]] : tuple(it[0], it[2]) // if no membrane channel specified, give empty membrane input; if membrane image exists, provide it to the process
                  ^^
  ```

- Warning: `workflows/molkart.nf:150:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? [[:],[]] : tuple(it[0], it[2]) // if no membrane channel specified, give empty membrane input; if membrane image exists, provide it to the process
                                                   ^^
  ```

- Warning: `workflows/molkart.nf:150:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? [[:],[]] : tuple(it[0], it[2]) // if no membrane channel specified, give empty membrane input; if membrane image exists, provide it to the process
                                                          ^^
  ```

- Warning: `workflows/molkart.nf:177:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              cellpose_custom_model ? cellpose_custom_model.map{it[2]} : []
                                                                ^^
  ```

- Warning: `workflows/molkart.nf:193:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? tuple(it[0], 1) : tuple(it[0], 2)
                  ^^
  ```

- Warning: `workflows/molkart.nf:193:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? tuple(it[0], 1) : tuple(it[0], 2)
                                        ^^
  ```

- Warning: `workflows/molkart.nf:193:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? tuple(it[0], 1) : tuple(it[0], 2)
                                                          ^^
  ```

- Warning: `workflows/molkart.nf:203:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ilastik_in.map{ [it[0], it[1]] },
                               ^^
  ```

- Warning: `workflows/molkart.nf:203:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ilastik_in.map{ [it[0], it[1]] },
                                      ^^
  ```

- Warning: `workflows/molkart.nf:204:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ilastik_in.map{ [it[0], it[2]] }
                               ^^
  ```

- Warning: `workflows/molkart.nf:204:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ilastik_in.map{ [it[0], it[2]] }
                                      ^^
  ```

- Warning: `workflows/molkart.nf:216:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              multicut_in.map{ tuple(it[0], it[1]) },
                                     ^^
  ```

- Warning: `workflows/molkart.nf:216:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              multicut_in.map{ tuple(it[0], it[1]) },
                                            ^^
  ```

- Warning: `workflows/molkart.nf:217:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              multicut_in.map{ tuple(it[0], it[4]) },
                                     ^^
  ```

- Warning: `workflows/molkart.nf:217:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              multicut_in.map{ tuple(it[0], it[4]) },
                                            ^^
  ```

- Warning: `workflows/molkart.nf:218:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              multicut_in.map{ tuple(it[0], it[3]) }
                                     ^^
  ```

- Warning: `workflows/molkart.nf:218:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              multicut_in.map{ tuple(it[0], it[3]) }
                                            ^^
  ```

- Warning: `workflows/molkart.nf:348:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              CROPHDF5.out.crop_summary.map{it[1]}
                                            ^^
  ```

- Warning: `workflows/molkart.nf:353:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              MOLKARTQC.out.qc.map{it[1]}
                                   ^^
  ```
