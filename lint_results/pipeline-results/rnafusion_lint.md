# Nextflow lint results

- Generated: 2026-06-16T14:31:31.066864330Z
- Nextflow version: 26.04.3
- Summary: 27 warnings

## :warning: Warnings

- Warning: `modules/nf-core/agat/convertgff2bed/main.nf:36:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args   ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/cat/cat/main.nf:23:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def file_list = files_in.collect { it.toString() }
                                         ^^
  ```

- Warning: `modules/nf-core/cat/cat/main.nf:58:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def file_list   = files_in.collect { it.toString() }
                                           ^^
  ```

- Warning: `modules/nf-core/cat/fastq/main.nf:22:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def readList = reads instanceof List ? reads.collect { it.toString() } : [reads.toString()]
                                                             ^^
  ```

- Warning: `modules/nf-core/cat/fastq/main.nf:58:60`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def readList = reads instanceof List ? reads.collect { it.toString() } : [reads.toString()]
                                                             ^^
  ```

- Warning: `modules/nf-core/ctatsplicing/prepgenomelib/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/ctatsplicing/prepgenomelib/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/ctatsplicing/prepgenomelib/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/ctatsplicing/prepgenomelib/main.nf:39:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/gatk4/markduplicates/main.nf:33:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = bam.collect { "--INPUT ${it}" }.join(' ')
                                                ^^
  ```

- Warning: `modules/nf-core/gffread/main.nf:26:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def extension   = args.contains("-T")       ? 'gtf' : ( ( ['-w', '-x', '-y' ].any { args.contains(it) } ) ? 'fasta' : 'gff3' )
                                                                                                        ^^
  ```

- Warning: `modules/nf-core/gffread/main.nf:30:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def args_sorted = args.replaceAll(/(.*)(-[wxy])(.*)/) { all, pre, param, post -> "$pre $post $param" }.trim()
                                                              ^^^
  ```

- Warning: `modules/nf-core/gffread/main.nf:49:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def extension   = args.contains("-T")       ? 'gtf' : ( ( ['-w', '-x', '-y' ].any { args.contains(it) } ) ? 'fasta' : 'gff3' )
                                                                                                        ^^
  ```

- Warning: `modules/nf-core/salmon/quant/main.nf:34:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      meta.single_end ? [reads].flatten().each { reads1 << it } : reads.eachWithIndex { v, ix -> (ix & 1 ? reads2 : reads1) << v }
                                                           ^^
  ```

- Warning: `subworkflows/local/fusioninspector_workflow/main.nf:27:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/fusioninspector_workflow/main.nf:28:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_arriba_visualisation = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/fusioninspector_workflow/main.nf:33:51`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              ch_whitelist = ch_fusion_list.combine(Channel.value(file(whitelist, checkIfExists:true)))
                                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/qc_workflow/main.nf:18:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnafusion_pipeline/main.nf:111:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnafusion_pipeline/main.nf:205:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          def setDfamParams = dfamParams.findAll { params[it] }
                                                         ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_rnafusion_pipeline/main.nf:263:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def strandedness_ok = metas.collect{ it.strandedness }.unique().size == 1
                                           ^^
  ```

- Warning: `subworkflows/nf-core/bam_stringtie_merge/main.nf:12:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions       = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_stringtie_merge/main.nf:13:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_stringtie_gtfs = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_stringtie_merge/main.nf:22:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { it[1] }
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
