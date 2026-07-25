# Nextflow lint results

- Generated: 2026-07-25T00:34:17.710405611Z
- Nextflow version: 26.07.0-edge
- Summary: 43 warnings

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

- Warning: `subworkflows/local/utils_nfcore_molkart_pipeline/main.nf:188:10`: Variable was declared but not used

  ```nextflow
      def (meta, files) = input
           ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_molkart_pipeline/main.nf:188:16`: Variable was declared but not used

  ```nextflow
      def (meta, files) = input
                 ^^^^^
  ```

- Warning: `workflows/molkart.nf:54:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[3] } // filter samples with membrane
                    ^^
  ```

- Warning: `workflows/molkart.nf:92:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def sorted = [tiffs, stains].transpose().sort { it[1] }
                                                              ^^
  ```

- Warning: `workflows/molkart.nf:99:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      grouped_map_stack.filter { !it[2] } // for rows without a present membrane image, set channel to no_stack
                                  ^^
  ```

- Warning: `workflows/molkart.nf:102:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      grouped_map_stack.filter{ it[2] }      // for rows where the membrane image is present, create a list of images to be stacked
                                ^^
  ```

- Warning: `workflows/molkart.nf:109:10`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          [it[0], it[1]]
           ^^
  ```

- Warning: `workflows/molkart.nf:109:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          [it[0], it[1]]
                  ^^
  ```

- Warning: `workflows/molkart.nf:123:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? tuple(it[0], 1) : tuple(it[0], 2)
                  ^^
  ```

- Warning: `workflows/molkart.nf:123:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? tuple(it[0], 1) : tuple(it[0], 2)
                                        ^^
  ```

- Warning: `workflows/molkart.nf:123:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? tuple(it[0], 1) : tuple(it[0], 2)
                                                          ^^
  ```

- Warning: `workflows/molkart.nf:134:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      tuple('matchkey', it[1])
                                        ^^
  ```

- Warning: `workflows/molkart.nf:135:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      }.groupTuple().map{ it[1]} )
                                          ^^
  ```

- Warning: `workflows/molkart.nf:153:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              grouped_map_stack.map{ tuple(it[0], it[1]) },
                                           ^^
  ```

- Warning: `workflows/molkart.nf:153:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              grouped_map_stack.map{ tuple(it[0], it[1]) },
                                                  ^^
  ```

- Warning: `workflows/molkart.nf:155:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? [[:],[]] : tuple(it[0], it[2]) // if no membrane channel specified, give empty membrane input; if membrane image exists, provide it to the process
                  ^^
  ```

- Warning: `workflows/molkart.nf:155:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? [[:],[]] : tuple(it[0], it[2]) // if no membrane channel specified, give empty membrane input; if membrane image exists, provide it to the process
                                                   ^^
  ```

- Warning: `workflows/molkart.nf:155:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? [[:],[]] : tuple(it[0], it[2]) // if no membrane channel specified, give empty membrane input; if membrane image exists, provide it to the process
                                                          ^^
  ```

- Warning: `workflows/molkart.nf:182:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              cellpose_custom_model ? cellpose_custom_model.map{it[2]} : []
                                                                ^^
  ```

- Warning: `workflows/molkart.nf:198:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? tuple(it[0], 1) : tuple(it[0], 2)
                  ^^
  ```

- Warning: `workflows/molkart.nf:198:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? tuple(it[0], 1) : tuple(it[0], 2)
                                        ^^
  ```

- Warning: `workflows/molkart.nf:198:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  it[2] == null ? tuple(it[0], 1) : tuple(it[0], 2)
                                                          ^^
  ```

- Warning: `workflows/molkart.nf:208:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ilastik_in.map{ [it[0], it[1]] },
                               ^^
  ```

- Warning: `workflows/molkart.nf:208:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ilastik_in.map{ [it[0], it[1]] },
                                      ^^
  ```

- Warning: `workflows/molkart.nf:209:30`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ilastik_in.map{ [it[0], it[2]] }
                               ^^
  ```

- Warning: `workflows/molkart.nf:209:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ilastik_in.map{ [it[0], it[2]] }
                                      ^^
  ```

- Warning: `workflows/molkart.nf:221:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              multicut_in.map{ tuple(it[0], it[1]) },
                                     ^^
  ```

- Warning: `workflows/molkart.nf:221:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              multicut_in.map{ tuple(it[0], it[1]) },
                                            ^^
  ```

- Warning: `workflows/molkart.nf:222:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              multicut_in.map{ tuple(it[0], it[4]) },
                                     ^^
  ```

- Warning: `workflows/molkart.nf:222:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              multicut_in.map{ tuple(it[0], it[4]) },
                                            ^^
  ```

- Warning: `workflows/molkart.nf:223:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              multicut_in.map{ tuple(it[0], it[3]) }
                                     ^^
  ```

- Warning: `workflows/molkart.nf:223:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              multicut_in.map{ tuple(it[0], it[3]) }
                                            ^^
  ```

- Warning: `workflows/molkart.nf:320:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_config        = channel.fromPath(
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/molkart.nf:322:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_custom_config = params.multiqc_config ?
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/molkart.nf:325:5`: Variable was declared but not used

  ```nextflow
      ch_multiqc_logo          = params.multiqc_logo ?
      ^^^^^^^^^^^^^^^
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
