# Nextflow lint results

- Generated: 2026-06-19T00:50:12.658315346Z
- Nextflow version: 26.04.4
- Summary: 136 warnings

## :warning: Warnings

- Warning: `modules/nf-core/hifiasm/main.nf:36:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def long_reads_sorted = long_reads instanceof List ? long_reads.sort{ it.name } : long_reads
                                                                            ^^
  ```

- Warning: `modules/nf-core/hifiasm/main.nf:37:69`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def ul_reads_sorted = ul_reads instanceof List ? ul_reads.sort{ it.name } : ul_reads
                                                                      ^^
  ```

- Warning: `modules/nf-core/meryl/unionsum/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:66:9`: Variable was declared but not used

  ```nextflow
      def target = reference ?: (bam_input ? error("BAM input requires reference") : reads)
          ^^^^^^
  ```

- Warning: `modules/nf-core/trimgalore/main.nf:47:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          args_list.removeAll { it.toLowerCase().contains('_r2 ') }
                                ^^
  ```

- Warning: `subworkflows/local/assemble/main.nf:22:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_refs }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/assemble/main.nf:23:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_ref_bam }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/assemble/main.nf:24:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_assembly_bam }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/assemble/main.nf:25:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_assembly }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/assemble/main.nf:26:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { flye_inputs }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/assemble/main.nf:27:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { hifiasm_inputs }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/assemble/main.nf:28:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { longreads }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/assemble/main.nf:29:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/assemble/main.nf:45:13`: Variable was declared but not used

  ```nextflow
          def hifi_only = params.hifi && !params.ont ? true : false
              ^^^^^^^^^
  ```

- Warning: `subworkflows/local/assemble/main.nf:171:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.empty().set { ch_ref_bam }
          ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_sort_stat/main.nf:20:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/bam_sort_stat/main.nf:26:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions.mix(SAMTOOLS_INDEX.out.versions).mix(BAM_STATS_SAMTOOLS.out.versions)
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/hifi/main.nf:9:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/hifi/main.nf:13:38`: Variable was declared but not used

  ```nextflow
      PREPARE_HIFI.out.hifireads.set { hifi_reads }
                                       ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/hifi/main.nf:17:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/jellyfish/main.nf:13:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { genomescope_in }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/jellyfish/main.nf:14:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/jellyfish/main.nf:44:45`: Variable was declared but not used

  ```nextflow
      GENOMESCOPE.out.estimated_hap_len.set { hap_len }
                                              ^^^^^^^
  ```

- Warning: `subworkflows/local/jellyfish/main.nf:46:35`: Variable was declared but not used

  ```nextflow
      GENOMESCOPE.out.summary.set { genomescope_summary }
                                    ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/jellyfish/main.nf:48:32`: Variable was declared but not used

  ```nextflow
      GENOMESCOPE.out.plot.set { genomescope_plot }
                                 ^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/jellyfish/main.nf:50:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/liftoff/main.nf:9:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/liftoff/main.nf:18:28`: Variable was declared but not used

  ```nextflow
      LIFTOFF.out.gff3.set { lifted_annotations }
                             ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/liftoff/main.nf:20:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions.mix(LIFTOFF.out.versions)
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/mapping/map_sr/main.nf:10:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/mapping/map_to_assembly/main.nf:10:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/mapping/map_to_assembly/main.nf:31:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions.mix(ALIGN.out.versions).mix(BAM_STATS.out.versions)
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/mapping/map_to_ref/main.nf:10:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/mapping/map_to_ref/main.nf:30:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions.mix(ALIGN.out.versions).mix(BAM_STATS.out.versions)
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/ont/main.nf:10:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/ont/main.nf:11:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.of([[],[]])
      ^^^^^^^
  ```

- Warning: `subworkflows/local/ont/main.nf:17:35`: Variable was declared but not used

  ```nextflow
      PREPARE_ONT.out.trimmed.set { ont_reads }
                                    ^^^^^^^^^
  ```

- Warning: `subworkflows/local/ont/main.nf:19:40`: Variable was declared but not used

  ```nextflow
      PREPARE_ONT.out.nanoq_report.set { nanoq_report }
                                         ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/ont/main.nf:21:39`: Variable was declared but not used

  ```nextflow
      PREPARE_ONT.out.nanoq_stats.set { nanoq_stats }
                                        ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/ont/main.nf:35:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/main.nf:16:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/main.nf:17:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { polish_busco_reports }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/main.nf:18:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { polish_quast_reports }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/main.nf:19:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { polish_merqury_reports }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/main.nf:73:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/medaka/polish_medaka/main.nf:14:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/medaka/polish_medaka/main.nf:15:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { quast_out }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/medaka/polish_medaka/main.nf:15:27`: Variable was declared but not used

  ```nextflow
      Channel.empty().set { quast_out }
                            ^^^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/medaka/polish_medaka/main.nf:16:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { busco_out }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/medaka/polish_medaka/main.nf:16:27`: Variable was declared but not used

  ```nextflow
      Channel.empty().set { busco_out }
                            ^^^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/medaka/polish_medaka/main.nf:17:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { merqury_report_files }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/medaka/polish_medaka/main.nf:17:27`: Variable was declared but not used

  ```nextflow
      Channel.empty().set { merqury_report_files }
                            ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/medaka/polish_medaka/main.nf:33:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/medaka/run_medaka/main.nf:16:31`: Variable was declared but not used

  ```nextflow
      MEDAKA.out.assembly.set { medaka_out }
                                ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/medaka/run_medaka/main.nf:17:31`: Variable was declared but not used

  ```nextflow
      MEDAKA.out.versions.set { versions }
                                ^^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/pilon/polish_pilon/main.nf:16:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/pilon/polish_pilon/main.nf:37:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/pilon/run_pilon/main.nf:17:5`: Variable was declared but not used

  ```nextflow
      versions = PILON.out.versions
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/polishing/pilon/run_pilon/main.nf:18:5`: Variable was declared but not used

  ```nextflow
      improved_assembly = PILON.out.improved_assembly
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_hifi/main.nf:9:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_hifi/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_ont/chop/main.nf:8:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { chopped_reads }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_ont/chop/main.nf:9:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_ont/chop/main.nf:19:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_ont/collect/main.nf:8:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_ont/collect/main.nf:19:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_ont/main.nf:10:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_ont/main.nf:20:39`: Variable was declared but not used

  ```nextflow
      RUN_NANOQ.out.median_length.set { med_len }
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_ont/main.nf:22:32`: Variable was declared but not used

  ```nextflow
      RUN_NANOQ.out.report.set { nanoq_report }
                                 ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_ont/main.nf:24:31`: Variable was declared but not used

  ```nextflow
      RUN_NANOQ.out.stats.set { nanoq_stats }
                                ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_ont/main.nf:26:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions.mix(COLLECT.out.versions).mix(CHOP.out.versions).mix(RUN_NANOQ.out.versions)
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_ont/run_nanoq/main.nf:8:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_ont/run_nanoq/main.nf:12:28`: Variable was declared but not used

  ```nextflow
      NANOQ.out.report.set { report }
                             ^^^^^^
  ```

- Warning: `subworkflows/local/prepare_ont/run_nanoq/main.nf:14:27`: Variable was declared but not used

  ```nextflow
      NANOQ.out.stats.set { stats }
                            ^^^^^
  ```

- Warning: `subworkflows/local/prepare_ont/run_nanoq/main.nf:16:35`: Variable was declared but not used

  ```nextflow
      NANOQ.out.median_length.set { median_length }
                                    ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_shortreads/main.nf:10:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_shortreads/main.nf:13:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { create_shortread_channel(it) }
                                          ^^
  ```

- Warning: `subworkflows/local/prepare_shortreads/main.nf:23:39`: Variable was declared but not used

  ```nextflow
      MERYL_UNIONSUM.out.meryl_db.set { meryl_kmers }
                                        ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_shortreads/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions.mix(MERYL_COUNT.out.versions).mix(MERYL_UNIONSUM.out.versions)
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/qc/busco/main.nf:8:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/qc/busco/main.nf:9:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { batch_summary }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/qc/busco/main.nf:10:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { short_summary_txt }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/qc/busco/main.nf:11:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { short_summary_json }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/qc/main.nf:15:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/qc/main.nf:16:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { quast_out }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/qc/main.nf:17:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { busco_out }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/qc/main.nf:18:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { merqury_report_files }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/qc/main.nf:19:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { map_to_assembly }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/qc/main.nf:54:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/qc/merqury/main.nf:9:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/qc/quast/main.nf:11:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/qc/quast/main.nf:16:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { quast_results }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/qc/quast/main.nf:17:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { quast_tsv }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/links/main.nf:15:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/links/main.nf:39:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/longstitch/main.nf:16:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/longstitch/main.nf:37:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/main.nf:16:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/main.nf:17:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { links_busco }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/main.nf:18:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { links_quast }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/main.nf:19:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { links_merqury }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/main.nf:20:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { longstitch_busco }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/main.nf:21:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { longstitch_quast }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/main.nf:22:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { longstitch_merqury }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/main.nf:23:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ragtag_busco }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/main.nf:24:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ragtag_quast }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/main.nf:25:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ragtag_merqury }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/main.nf:57:16`: Variable was declared but not used

  ```nextflow
          .set { scaffold_busco_reports }
                 ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/main.nf:62:16`: Variable was declared but not used

  ```nextflow
          .set { scaffold_quast_reports }
                 ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/main.nf:67:16`: Variable was declared but not used

  ```nextflow
          .set { scaffold_merqury_reports }
                 ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/main.nf:69:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/ragtag/main.nf:16:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/ragtag/main.nf:30:45`: Variable was declared but not used

  ```nextflow
      RAGTAG_SCAFFOLD.out.corrected_agp.set { ragtag_scaffold_agp }
                                              ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/scaffolding/ragtag/main.nf:43:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomeassembler_pipeline/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomeassembler_pipeline/main.nf:104:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_refs }
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomeassembler_pipeline/main.nf:105:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.fromPath(params.input)
      ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_sort_stats_samtools/main.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/bam_stats_samtools/main.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
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

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/genomeassembler.nf:44:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_ref_bam }
      ^^^^^^^
  ```

- Warning: `workflows/genomeassembler.nf:45:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_polished_genome }
      ^^^^^^^
  ```

- Warning: `workflows/genomeassembler.nf:46:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_ont_reads }
      ^^^^^^^
  ```

- Warning: `workflows/genomeassembler.nf:47:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_hifi_reads }
      ^^^^^^^
  ```

- Warning: `workflows/genomeassembler.nf:48:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_shortreads }
      ^^^^^^^
  ```

- Warning: `workflows/genomeassembler.nf:49:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { meryl_kmers }
      ^^^^^^^
  ```

- Warning: `workflows/genomeassembler.nf:50:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { genome_size }
      ^^^^^^^
  ```

- Warning: `workflows/genomeassembler.nf:51:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty().set { ch_versions }
      ^^^^^^^
  ```

- Warning: `workflows/genomeassembler.nf:53:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `workflows/genomeassembler.nf:198:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `workflows/genomeassembler.nf:203:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `workflows/genomeassembler.nf:209:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          merqury_files = Channel.of([])
                          ^^^^^^^
  ```

- Warning: `workflows/genomeassembler.nf:212:117`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      REPORT(report_files, report_functions, nanoq_files, genomescope_files, quast_files, busco_files, merqury_files, Channel.fromPath("${params.outdir}/pipeline_info/nf_core_pipeline_software_versions.yml"))
                                                                                                                      ^^^^^^^
  ```

- Warning: `workflows/genomeassembler.nf:234:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```
