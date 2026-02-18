# Nextflow lint results

- Generated: 2026-02-18T00:23:15.080886230Z
- Nextflow version: 26.01.1-edge
- Summary: 3 errors, 41 warnings

## :x: Errors

- Error: `modules/nf-core/bwa/index/main.nf:14:27`: `bwa` is not defined

  ```nextflow
      tuple val(meta), path(bwa) , emit: index
                            ^^^
  ```

- Error: `tests/nextflow.config:28:27`: `SENTIEON_AUTH_MECH` is not defined (hint: use `env('...')` to access environment variable)

  ```nextflow
      SENTIEON_AUTH_MECH = "$SENTIEON_AUTH_MECH"
                            ^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/raredisease.nf:645:50`: `run_mt_for_wes` is not defined

  ```nextflow
      if (val_analysis_type.matches("wgs|mito") || run_mt_for_wes) {
                                                   ^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/nf-core/bwa/mem/main.nf:56:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/bwa/mem/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def samtools_command = sort_bam ? 'sort' : 'view'
          ^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/bwamem2/mem/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/bwamem2/mem/main.nf:62:9`: Variable was declared but not used

  ```nextflow
      def samtools_command = sort_bam ? 'sort' : 'view'
          ^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/bwamem2/mem/main.nf:66:9`: Variable was declared but not used

  ```nextflow
      def reference = fasta && extension=="cram"  ? "--reference ${fasta}" : ""
          ^^^^^^^^^
  ```

- Warning: `modules/nf-core/bwameme/mem/main.nf:75:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/bwameme/mem/main.nf:78:9`: Variable was declared but not used

  ```nextflow
      def samtools_command = sort_bam ? 'sort' : 'view'
          ^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/bwameme/mem/main.nf:82:9`: Variable was declared but not used

  ```nextflow
      def reference = fasta && extension=="cram"  ? "--reference ${fasta}" : ""
          ^^^^^^^^^
  ```

- Warning: `modules/nf-core/cadd/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
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

- Warning: `modules/nf-core/custom/addmostsevereconsequence/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/custom/addmostsevereconsequence/main.nf:49:9`: Variable was declared but not used

  ```nextflow
      def args2 = task.ext.args2 ?: ''
          ^^^^^
  ```

- Warning: `modules/nf-core/custom/addmostseverepli/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/custom/addmostseverepli/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args2 = task.ext.args2 ?: ''
          ^^^^^
  ```

- Warning: `modules/nf-core/gatk4/determinegermlinecontigploidy/main.nf:27:80`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def exclude = exclude_beds ? exclude_beds.collect { "--exclude-intervals ${it}" }.join(" ") : ""
                                                                                 ^^
  ```

- Warning: `modules/nf-core/gatk4/determinegermlinecontigploidy/main.nf:30:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = counts.collect { "--input ${it}" }.join(" ")
                                                   ^^
  ```

- Warning: `modules/nf-core/gatk4/filtermutectcalls/main.nf:29:117`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def orientationbias_command = orientationbias ? orientationbias.collect { "--orientation-bias-artifact-priors ${it}" }.join(' ') : ''
                                                                                                                      ^^
  ```

- Warning: `modules/nf-core/gatk4/filtermutectcalls/main.nf:30:94`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def segmentation_command = segmentation ? segmentation.collect { "--tumor-segmentation ${it}" }.join(' ') : ''
                                                                                               ^^
  ```

- Warning: `modules/nf-core/gatk4/filtermutectcalls/main.nf:32:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def table_command = table ? table.collect { "--contamination-table ${it}" }.join(' ') : ''
                                                                           ^^
  ```

- Warning: `modules/nf-core/gatk4/germlinecnvcaller/main.nf:28:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = tsv.collect { "--input ${it}" }.join(' ')
                                                ^^
  ```

- Warning: `modules/nf-core/gatk4/mergevcfs/main.nf:25:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = vcf.collect { "--INPUT ${it}" }.join(' ')
                                                ^^
  ```

- Warning: `modules/nf-core/gatk4/postprocessgermlinecnvcalls/main.nf:25:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def calls_command = calls ? calls.collect { "--calls-shard-path ${it}" }.join(' ') : ""
                                                                        ^^
  ```

- Warning: `modules/nf-core/gatk4/postprocessgermlinecnvcalls/main.nf:26:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def model_command = model ? model.collect { "--model-shard-path ${it}" }.join(' ') : ""
                                                                        ^^
  ```

- Warning: `modules/nf-core/glnexus/main.nf:27:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input = gvcfs.collect { it.toString() }
                                  ^^
  ```

- Warning: `modules/nf-core/haplocheck/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/last/lastdb/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:40:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def pairs = vcfs.indices.collect { [vcfs[it], input_priority[it]] }
                                                      ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:40:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def pairs = vcfs.indices.collect { [vcfs[it], input_priority[it]] }
                                                                          ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:42:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              vcfs = pairs.collect { it[0] }
                                     ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:43:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              priority = pairs.collect { it[1] }
                                         ^^
  ```

- Warning: `modules/nf-core/svdb/merge/main.nf:57:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          input = (vcfs.collect().size() > 1 && sort_inputs) ? vcfs.sort { it.name } : vcfs
                                                                           ^^
  ```

- Warning: `modules/nf-core/vcf2cytosure/main.nf:51:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/vcf2cytosure/main.nf:52:9`: Variable was declared but not used

  ```nextflow
      def coverage = coverage_bed ? "--coverage ${coverage_bed}" : ''
          ^^^^^^^^
  ```

- Warning: `modules/nf-core/vcf2cytosure/main.nf:53:9`: Variable was declared but not used

  ```nextflow
      def cnvkit = cns ? ( coverage_bed ? '' : "--cn ${cns}" ) : ''
          ^^^^^^
  ```

- Warning: `modules/nf-core/vcf2cytosure/main.nf:54:9`: Variable was declared but not used

  ```nextflow
      def snv = snv_vcf ? ( coverage_bed ? '' : "--snv ${snv_vcf}" ) : ''
          ^^^
  ```

- Warning: `modules/nf-core/vcf2cytosure/main.nf:55:9`: Variable was declared but not used

  ```nextflow
      def blacklist = blacklist_bed ? "--blacklist ${blacklist_bed}" : ''
          ^^^^^^^^^
  ```

- Warning: `subworkflows/local/call_structural_variants.nf:18:9`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_mt_bam_bai          // channel: [mandatory] [ val(meta), path(bam), path(bai) ]
          ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/call_structural_variants.nf:30:9`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          run_mt_for_wes         // boolean
          ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/call_sv_MT/main.nf:39:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_versions = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/vcf_filter_bcftools_ensemblvep/main.nf:14:5`: Variable was declared but not used

  ```nextflow
      ch_versions = channel.empty()
      ^^^^^^^^^^^
  ```
