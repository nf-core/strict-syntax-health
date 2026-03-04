# Nextflow lint results

- Generated: 2026-03-04T00:20:50.383497918Z
- Nextflow version: 26.02.0-edge
- Summary: 17 errors, 31 warnings

## :x: Errors

- Error: `main.nf:18:1`: Included name 'BACTMAP' is not defined in module '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/bactmap/workflows/bactmap.nf'

  ```nextflow
  include { BACTMAP                 } from './workflows/bactmap'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `main.nf:59:5`: `BACTMAP` is not defined

  ```nextflow
      BACTMAP (
      ^^^^^^^
  ```

- Error: `main.nf:64:22`: `BACTMAP` is not defined

  ```nextflow
      multiqc_report = BACTMAP.out.multiqc_report // channel: /path/to/multiqc_report.html
                       ^^^^^^^
  ```

- Error: `modules/local/alignpseudogenomes/main.nf:14:15`: `NUM_ALIGNMENT_GENOMES` is not defined

  ```nextflow
      tuple env(NUM_ALIGNMENT_GENOMES), path("aligned_pseudogenomes.fas"), emit: aligned_pseudogenomes
                ^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `modules/local/read_stats/main.nf:11:39`: `json` is already declared

  ```nextflow
      tuple val(meta), path(json), path(json)
                                        ^^^^
  ```

- Error: `modules/nf-core/snpsites/main.nf:16:11`: `CONSTANT_SITES` is not defined

  ```nextflow
      env   CONSTANT_SITES, emit: constant_sites_string
            ^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/longread_adapterremoval/main.nf:17:9`: Incorrect number of call arguments, expected 2 but received 1

  ```nextflow
          PORECHOP_ABI(reads)
          ^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/shortread_fastp/main.nf:23:22`: `reads` is already declared

  ```nextflow
          .map { meta, reads -> [meta, reads, [] ] }
                       ^^^^^
  ```

- Error: `subworkflows/local/shortread_fastp/main.nf:25:22`: `reads` is already declared

  ```nextflow
          .map { meta, reads -> [meta, reads, [] ] }
                       ^^^^^
  ```

- Error: `workflows/bactmap.nf:12:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  def checkPathParamList = [ params.input, params.fasta, params.multiqc_config,
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/bactmap.nf:16:1`: `for` loops are no longer supported

  ```nextflow
  for (param in checkPathParamList) { if (param) { file(param, checkIfExists: true) } }
  ^^^
  ```

- Error: `workflows/bactmap.nf:16:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  for (param in checkPathParamList) { if (param) { file(param, checkIfExists: true) } }
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/bactmap.nf:16:6`: `param` is not defined

  ```nextflow
  for (param in checkPathParamList) { if (param) { file(param, checkIfExists: true) } }
       ^^^^^
  ```

- Error: `workflows/bactmap.nf:16:40`: `param` is not defined

  ```nextflow
  for (param in checkPathParamList) { if (param) { file(param, checkIfExists: true) } }
                                         ^^^^^^^
  ```

- Error: `workflows/bactmap.nf:16:55`: `param` is not defined

  ```nextflow
  for (param in checkPathParamList) { if (param) { file(param, checkIfExists: true) } }
                                                        ^^^^^
  ```

- Error: `workflows/bactmap.nf:19:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  if ( params.input ) {
  ^
  ```

- Error: `workflows/bactmap.nf:76:1`: Invalid workflow definition -- check for missing or out-of-order section labels

  ```nextflow
  workflow BACTMAP {
  ^
  ```

## :warning: Warnings

- Warning: `conf/modules.config:124:191`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { ( params.perform_runmerging == false || ( params.perform_runmerging && !meta.is_multirun ) )  && params.perform_shortread_qc && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                ^^
  ```

- Warning: `conf/modules.config:156:191`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs:  { ( params.perform_runmerging == false || ( params.perform_runmerging && !meta.is_multirun ) ) && params.perform_shortread_qc && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                ^^
  ```

- Warning: `conf/modules.config:184:190`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { ( params.perform_runmerging == false || ( params.perform_runmerging && !meta.is_multirun ) ) && params.perform_shortread_qc && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                               ^^
  ```

- Warning: `conf/modules.config:214:225`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { ( params.perform_runmerging == false || ( params.perform_runmerging && !meta.is_multirun ) ) && params.perform_shortread_qc && !params.shortread_qc_mergepairs && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                  ^^
  ```

- Warning: `conf/modules.config:228:190`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { ( params.perform_runmerging == false || ( params.perform_runmerging && !meta.is_multirun ) ) && params.perform_shortread_qc && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                               ^^
  ```

- Warning: `conf/modules.config:252:308`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { ( params.perform_runmerging == false || ( params.perform_runmerging && !meta.is_multirun ) ) && !params.perform_longread_hostremoval && params.longread_qc_skipqualityfilter && !params.longread_qc_skipadaptertrim && params.perform_longread_qc && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                                                                                                     ^^
  ```

- Warning: `conf/modules.config:276:304`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && !params.perform_longread_hostremoval && params.longread_qc_skipqualityfilter && !params.longread_qc_skipadaptertrim && params.perform_longread_qc && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                                                                                                 ^^
  ```

- Warning: `conf/modules.config:305:266`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && !params.perform_longread_hostremoval && !params.longread_qc_skipqualityfilter && params.perform_longread_qc && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                                                           ^^
  ```

- Warning: `conf/modules.config:334:266`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  saveAs: { (params.perform_runmerging == false || (params.perform_runmerging && !meta.is_multirun)) && !params.perform_longread_hostremoval && !params.longread_qc_skipqualityfilter && params.perform_longread_qc && params.save_analysis_ready_fastqs ? it : null },
                                                                                                                                                                                                                                                                           ^^
  ```

- Warning: `main.nf:50:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_fasta = Channel.fromPath(params.fasta, checkIfExists: true).collect()
                     ^^^^^^^
  ```

- Warning: `modules/local/bcftools/consensus/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/bcftools/consensus/main.nf:48:9`: Variable was declared but not used

  ```nextflow
      def masking = mask ? "-m $mask" : ""
          ^^^^^^^
  ```

- Warning: `modules/local/bedtools/genomecov/main.nf:30:9`: Variable was declared but not used

  ```nextflow
      def buffer   = task.memory ? "--buffer-size=${task.memory.toGiga().intdiv(2)}G" : ''
          ^^^^^^
  ```

- Warning: `modules/local/clair3/main.nf:57:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/read_stats/main.nf:11:27`: Variable was declared but not used

  ```nextflow
      tuple val(meta), path(json), path(json)
                            ^^^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:67:9`: Variable was declared but not used

  ```nextflow
      def target = reference ?: (bam_input ? error("BAM input requires reference") : reads)
          ^^^^^^
  ```

- Warning: `modules/nf-core/nanoq/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/porechop/abi/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/porechop/abi/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def adapters_list = custom_adapters ? "--custom_adapters ${custom_adapters}" : ""
          ^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/seqtk/comp/main.nf:32:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sort_freebayes_bcftools/main.nf:19:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      FREEBAYES ( ch_input, ch_fasta_fai.map{ meta, fasta, fai -> [ meta, fasta ] }, ch_fasta_fai.map{ meta, fasta, fai -> [ meta, fai ] }, ch_samples, ch_populations, ch_cnv )
                                                           ^^^
  ```

- Warning: `subworkflows/local/bam_variant_calling_sort_freebayes_bcftools/main.nf:19:108`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      FREEBAYES ( ch_input, ch_fasta_fai.map{ meta, fasta, fai -> [ meta, fasta ] }, ch_fasta_fai.map{ meta, fasta, fai -> [ meta, fai ] }, ch_samples, ch_populations, ch_cnv )
                                                                                                             ^^^^^
  ```

- Warning: `subworkflows/local/shortread_adapterremoval/main.nf:19:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          single: it[0].single_end
                  ^^
  ```

- Warning: `subworkflows/local/shortread_adapterremoval/main.nf:20:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          paired: !it[0].single_end
                   ^^
  ```

- Warning: `subworkflows/local/shortread_fastp/main.nf:11:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      adapterlist
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/shortread_fastp/main.nf:18:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          single: it[0]['single_end'] == true
                  ^^
  ```

- Warning: `subworkflows/local/shortread_fastp/main.nf:19:17`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          paired: it[0]['single_end'] == false
                  ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_bactmap_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_bactmap_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/nf-core/fastq_align_bowtie2/main.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/bactmap.nf:20:5`: Variable was declared but not used

  ```nextflow
      ch_input = file(params.input, checkIfExists: true)
      ^^^^^^^^
  ```
