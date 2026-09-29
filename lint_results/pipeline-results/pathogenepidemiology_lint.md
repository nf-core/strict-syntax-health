# Nextflow lint results

- Generated: 2026-09-29T00:23:09.312269615Z
- Nextflow version: 26.09.1-edge
- Summary: 4 errors, 39 warnings

## :x: Errors

- Error: `subworkflows/nf-core/deepvariant/tests/deepvariant-workflow-and-process-equality-tester.nf:1:1`: Invalid include source: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/pathogenepidemiology/modules/nf-core/deepvariant/rundeepvariant/main.nf'

  ```nextflow
  include { DEEPVARIANT_RUNDEEPVARIANT      } from '../../../../modules/nf-core/deepvariant/rundeepvariant/main'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/nf-core/deepvariant/tests/deepvariant-workflow-and-process-equality-tester.nf:17:5`: `DEEPVARIANT_RUNDEEPVARIANT` is not defined

  ```nextflow
      DEEPVARIANT_RUNDEEPVARIANT(ch_input, ch_fasta, ch_fai, ch_gzi, ch_par_bed)
      ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/nf-core/deepvariant/tests/deepvariant-workflow-and-process-equality-tester.nf:21:14`: `DEEPVARIANT_RUNDEEPVARIANT` is not defined

  ```nextflow
      pc_vcf = DEEPVARIANT_RUNDEEPVARIANT.out.vcf
               ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/nf-core/deepvariant/tests/deepvariant-workflow-and-process-equality-tester.nf:23:15`: `DEEPVARIANT_RUNDEEPVARIANT` is not defined

  ```nextflow
      pc_gvcf = DEEPVARIANT_RUNDEEPVARIANT.out.gvcf
                ^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `subworkflows/local/gatk_MOI.nf:40:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/gatk_MOI.nf:47:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_val = ch_queryfasta.map { meta, fasta -> fasta }.first()
                                         ^^^^
  ```

- Warning: `subworkflows/local/gatk_MOI.nf:48:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fai_val   = ch_queryfai.map   { meta, fai   -> fai   }.first()
                                         ^^^^
  ```

- Warning: `subworkflows/local/gatk_MOI.nf:49:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_dict_val  = ch_querydict.map  { meta, dict  -> dict  }.first()
                                         ^^^^
  ```

- Warning: `subworkflows/local/gatk_MOI.nf:78:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_dedup_bam.map { meta, bam, bai -> tuple(meta, bam) }
                                        ^^^
  ```

- Warning: `subworkflows/local/gatk_MOI.nf:94:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_intervals = Channel.fromPath("${launchDir}/assets/intervals/core_chr*.list")
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/gatk_MOI.nf:156:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi -> vcf.size() > 8000 }
                    ^^^^
  ```

- Warning: `subworkflows/local/gatk_MOI.nf:156:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi -> vcf.size() > 8000 }
                               ^^^
  ```

- Warning: `subworkflows/local/gatk_MOI.nf:218:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def vcfs = items.collect { it[1] }
                                         ^^
  ```

- Warning: `subworkflows/local/gatk_MOI.nf:219:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def tbis = items.collect { it[2] }
                                         ^^
  ```

- Warning: `subworkflows/local/prepare_references.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_queryref = Channel.of(queryurl)
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_references.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_hostref  = Channel.of(hosturl)
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/preprocess_reads.nf:16:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_samples = Channel.fromPath(samplesheet)
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/preprocess_reads.nf:31:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_reads_raw = ch_samples.map { meta, reads, platform ->
                                                   ^^^^^^^^
  ```

- Warning: `subworkflows/local/preprocess_reads.nf:41:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_adapters = Channel.fromPath(adapters)
                    ^^^^^^^
  ```

- Warning: `workflows/download_references.nf:14:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_refs = Channel.of(params.queryurl, params.hosturl)
                ^^^^^^^
  ```

- Warning: `workflows/original_local.nf:73:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .join(ch_samples.map { meta, reads, platform -> tuple(meta, platform) }, by: 0)
                                   ^^^^^
  ```

- Warning: `workflows/original_local.nf:74:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter { meta, reads, platform ->
                ^^^^
  ```

- Warning: `workflows/original_local.nf:74:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter { meta, reads, platform ->
                      ^^^^^
  ```

- Warning: `workflows/original_local.nf:77:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .map { meta, reads, platform ->
                          ^^^^^^^^
  ```

- Warning: `workflows/original_local.nf:100:3`: Variable was declared but not used

  ```nextflow
    varcalls_l = CLAIR3_CUSTOM(
    ^^^^^^^^^^
  ```

- Warning: `workflows/original_local.nf:121:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .join(ch_samples.map { meta, reads, platform -> tuple(meta, platform) }, by: 0)
                                   ^^^^^
  ```

- Warning: `workflows/original_local.nf:122:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter { meta, reads, platform ->
                ^^^^
  ```

- Warning: `workflows/original_local.nf:122:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter { meta, reads, platform ->
                      ^^^^^
  ```

- Warning: `workflows/original_local.nf:125:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .map { meta, reads, platform ->
                          ^^^^^^^^
  ```

- Warning: `workflows/original_local.nf:144:55`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
    ch_wgs_bam_s     = aligned_s.aligned.filter { meta, bam -> meta.library_strategy == 'WGS' }
                                                        ^^^
  ```

- Warning: `workflows/original_local.nf:146:3`: Variable was declared but not used

  ```nextflow
    ch_amplicon_bam_s = aligned_s.aligned.filter { meta, bam -> meta.library_strategy != 'WGS' }
    ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/original_local.nf:146:56`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
    ch_amplicon_bam_s = aligned_s.aligned.filter { meta, bam -> meta.library_strategy != 'WGS' }
                                                         ^^^
  ```

- Warning: `workflows/original_local.nf:153:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.fromPath("${launchDir}/assets/Strains.2kb.vcf.gz"),
      ^^^^^^^
  ```

- Warning: `workflows/original_local.nf:154:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.fromPath("${launchDir}/assets/Strains.2kb.vcf.gz.tbi")
      ^^^^^^^
  ```

- Warning: `workflows/original_local.nf:174:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
    ch_multiqc_input = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `workflows/original_local.nf:176:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fastqc_out.collect { meta, files -> files },
                                  ^^^^
  ```

- Warning: `workflows/original_local.nf:177:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_bbduk_stats.collect { meta, files -> files },
                                   ^^^^
  ```

- Warning: `workflows/original_local.nf:178:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_bbduk_logs.collect { meta, files -> files },
                                  ^^^^
  ```

- Warning: `workflows/original_local.nf:179:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_bbduk_dropped.collect { meta, files -> files },
                                     ^^^^
  ```

- Warning: `workflows/original_local.nf:180:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_mm2stats.stats.collect { meta, files -> files },
                                      ^^^^
  ```

- Warning: `workflows/original_local.nf:181:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_bm3stats.stats.collect { meta, files -> files },
                                      ^^^^
  ```

- Warning: `workflows/original_local.nf:182:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          varcalls_s.collect { meta, files, idx -> files }//,
                               ^^^^
  ```

- Warning: `workflows/original_local.nf:182:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          varcalls_s.collect { meta, files, idx -> files }//,
                                            ^^^
  ```
