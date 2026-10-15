# Nextflow lint results

- Generated: 2026-10-15T00:21:02.242064702Z
- Nextflow version: 26.10.0
- Summary: 6 errors, 70 warnings

## :x: Errors

- Error: `modules/local/hmmibdrs/main.nf:32:9`: `bam` is not defined

  ```nextflow
          $bam
          ^^^^
  ```

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

- Error: `workflows/original_local.nf:16:1`: Invalid include source: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/pathogenepidemiology/modules/local/hmmibdrs/mainf.nf'

  ```nextflow
  include { HMMIBDRS             } from '../modules/local/hmmibdrs/mainf'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/bbduk_custom/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/gatk4/markduplicates_custom/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/hmmibdrs/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/untar/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bbmap/bbduk/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bcftools/concat/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bcftools/stats/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bcftools/view/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bwamem3/index/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/bwamem3/mem/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/deepvariant/callvariants/main.nf:16:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/deepvariant/makeexamples/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/deepvariant/postprocessvariants/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/fastqc/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gatk4/applyvqsr/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gatk4/cleansam/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gatk4/createsequencedictionary/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gatk4/genomicsdbimport/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gatk4/genotypegvcfs/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gatk4/haplotypecaller/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gatk4/markduplicates/main.nf:24:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gatk4/variantrecalibrator/main.nf:26:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:25:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/minimap2/index/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/mosdepth/main.nf:30:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/picard/collectinsertsizemetrics/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/picard/createsequencedictionary/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/picard/sortsam/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/faidx/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/index/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/samtools/stats/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/untar/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/local/gatk_MOI/main.nf:46:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_val = ch_queryfasta.map { meta, fasta -> fasta }.first()
                                         ^^^^
  ```

- Warning: `subworkflows/local/gatk_MOI/main.nf:47:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fai_val   = ch_queryfai.map   { meta, fai   -> fai   }.first()
                                         ^^^^
  ```

- Warning: `subworkflows/local/gatk_MOI/main.nf:48:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_dict_val  = ch_querydict.map  { meta, dict  -> dict  }.first()
                                         ^^^^
  ```

- Warning: `subworkflows/local/gatk_MOI/main.nf:72:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_dedup_bam.map { meta, bam, bai -> tuple(meta, bam) }
                                        ^^^
  ```

- Warning: `subworkflows/local/gatk_MOI/main.nf:84:20`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_intervals = Channel.fromPath("${projectDir}/assets/intervals/core_chr*.list")
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/gatk_MOI/main.nf:142:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi -> vcf.size() > 8000 }
                    ^^^^
  ```

- Warning: `subworkflows/local/gatk_MOI/main.nf:142:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi -> vcf.size() > 8000 }
                               ^^^
  ```

- Warning: `subworkflows/local/gatk_MOI/main.nf:200:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def vcfs = items.collect { it[1] }
                                         ^^
  ```

- Warning: `subworkflows/local/gatk_MOI/main.nf:201:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

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

- Warning: `subworkflows/local/preprocess_reads.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_adapters = Channel.fromPath("${projectDir}/assets/adapters.fa", checkIfExists: true)
                    ^^^^^^^
  ```

- Warning: `workflows/original_local.nf:53:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .join(ch_samples.map { meta, reads, platform -> tuple(meta, platform) }, by: 0)
                                   ^^^^^
  ```

- Warning: `workflows/original_local.nf:54:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter { meta, reads, platform ->
                ^^^^
  ```

- Warning: `workflows/original_local.nf:54:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter { meta, reads, platform ->
                      ^^^^^
  ```

- Warning: `workflows/original_local.nf:57:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .map { meta, reads, platform ->
                          ^^^^^^^^
  ```

- Warning: `workflows/original_local.nf:90:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .join(ch_samples.map { meta, reads, platform -> tuple(meta, platform) }, by: 0)
                                   ^^^^^
  ```

- Warning: `workflows/original_local.nf:91:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter { meta, reads, platform ->
                ^^^^
  ```

- Warning: `workflows/original_local.nf:91:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .filter { meta, reads, platform ->
                      ^^^^^
  ```

- Warning: `workflows/original_local.nf:94:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .map { meta, reads, platform ->
                          ^^^^^^^^
  ```

- Warning: `workflows/original_local.nf:113:55`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
    ch_wgs_bam_s     = aligned_s.aligned.filter { meta, bam -> meta.library_strategy == 'WGS' }
                                                        ^^^
  ```

- Warning: `workflows/original_local.nf:115:3`: Variable was declared but not used

  ```nextflow
    ch_amplicon_bam_s = aligned_s.aligned.filter { meta, bam -> meta.library_strategy != 'WGS' }
    ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/original_local.nf:115:56`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
    ch_amplicon_bam_s = aligned_s.aligned.filter { meta, bam -> meta.library_strategy != 'WGS' }
                                                         ^^^
  ```

- Warning: `workflows/original_local.nf:122:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.fromPath("${launchDir}/assets/Strains.2kb.vcf.gz"),
      ^^^^^^^
  ```

- Warning: `workflows/original_local.nf:123:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.fromPath("${launchDir}/assets/Strains.2kb.vcf.gz.tbi")
      ^^^^^^^
  ```

- Warning: `workflows/original_local.nf:158:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
    ch_multiqc_input = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `workflows/original_local.nf:160:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fastqc_out.collect { meta, files -> files },
                                  ^^^^
  ```

- Warning: `workflows/original_local.nf:161:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_bbduk_stats.collect { meta, files -> files },
                                   ^^^^
  ```

- Warning: `workflows/original_local.nf:162:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_bbduk_logs.collect { meta, files -> files },
                                  ^^^^
  ```

- Warning: `workflows/original_local.nf:163:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_bbduk_dropped.collect { meta, files -> files },
                                     ^^^^
  ```

- Warning: `workflows/original_local.nf:164:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_mm2stats.stats.collect { meta, files -> files },
                                      ^^^^
  ```

- Warning: `workflows/original_local.nf:165:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_bm3stats.stats.collect { meta, files -> files },
                                      ^^^^
  ```

- Warning: `workflows/original_local.nf:166:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          varcalls_s.collect { meta, files, idx -> files }//,
                               ^^^^
  ```

- Warning: `workflows/original_local.nf:166:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          varcalls_s.collect { meta, files, idx -> files }//,
                                            ^^^
  ```

- Warning: `workflows/pathogenepidemiology.nf:130:9`: Variable was declared but not used

  ```nextflow
      def ch_amplicon_bam_s = aligned_s.aligned.filter { meta, _bam -> meta.library_strategy != 'WGS' }
          ^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/pathogenepidemiology.nf:136:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath("${projectDir}/assets/Strains.2kb.vcf.gz", checkIfExists: true),
          ^^^^^^^
  ```

- Warning: `workflows/pathogenepidemiology.nf:137:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath("${projectDir}/assets/Strains.2kb.vcf.gz.tbi", checkIfExists: true)
          ^^^^^^^
  ```
