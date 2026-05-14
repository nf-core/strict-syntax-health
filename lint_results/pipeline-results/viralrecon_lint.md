# Nextflow lint results

- Generated: 2026-05-14T00:39:42.933732305Z
- Nextflow version: 26.04.1
- Summary: 152 warnings

## :warning: Warnings

- Warning: `subworkflows/local/additional_annotation/main.nf:62:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          BCFTOOLS_QUERY.out.output.collect{it[1]},
                                            ^^
  ```

- Warning: `subworkflows/local/additional_annotation/main.nf:63:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          SNPSIFT_EXTRACTFIELDS.out.txt.collect{it[1]}.ifEmpty([]),
                                                ^^
  ```

- Warning: `subworkflows/local/additional_annotation/main.nf:64:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          pangolin.collect{it[1]}.ifEmpty([])
                           ^^
  ```

- Warning: `subworkflows/local/assembly_minia/main.nf:44:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, contig -> contig.size() > 0 }
                    ^^^^
  ```

- Warning: `subworkflows/local/assembly_qc/main.nf:55:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .collect{ it[1] }
                        ^^
  ```

- Warning: `subworkflows/local/assembly_qc/main.nf:61:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              fasta.map { [ [:], it ] },
                                 ^^
  ```

- Warning: `subworkflows/local/assembly_qc/main.nf:75:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              fasta.map { [ [:], it ] }
                                 ^^
  ```

- Warning: `subworkflows/local/assembly_spades/main.nf:34:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, illumina, pacbio, nanopore -> !meta.single_end }
                              ^^^^^^^^
  ```

- Warning: `subworkflows/local/assembly_spades/main.nf:34:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, illumina, pacbio, nanopore -> !meta.single_end }
                                        ^^^^^^
  ```

- Warning: `subworkflows/local/assembly_spades/main.nf:34:47`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, illumina, pacbio, nanopore -> !meta.single_end }
                                                ^^^^^^^^
  ```

- Warning: `subworkflows/local/assembly_spades/main.nf:68:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, scaffold -> scaffold.size() > 0 }
                    ^^^^
  ```

- Warning: `subworkflows/local/assembly_spades/main.nf:74:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, gfa -> gfa.size() > 0 }
                    ^^^^
  ```

- Warning: `subworkflows/local/assembly_unicycler/main.nf:55:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, scaffold -> scaffold.size() > 0 }
                    ^^^^
  ```

- Warning: `subworkflows/local/assembly_unicycler/main.nf:61:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, gfa -> gfa.size() > 0 }
                    ^^^^
  ```

- Warning: `subworkflows/local/consensus_qc/main.nf:30:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .collect{ it[1] }
                    ^^
  ```

- Warning: `subworkflows/local/consensus_qc/main.nf:36:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              fasta.map { [ [:], it ] },
                                 ^^
  ```

- Warning: `subworkflows/local/consensus_qc/main.nf:60:67`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_pango_database = UNTAR_PANGODB.out.untar.map { it[1] }
                                                                    ^^
  ```

- Warning: `subworkflows/local/hiv_resitance_detection/main.nf:64:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              LIFTOFF.out.gff3.map { it[1] },
                                     ^^
  ```

- Warning: `subworkflows/local/hiv_resitance_detection/main.nf:92:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          SIERRALOCAL.out.json.collect{it[1]},
                                       ^^
  ```

- Warning: `subworkflows/local/hiv_resitance_detection/main.nf:93:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          RESISTANCE_TABLES.out.mutation_csv.collect{it[1]},
                                                     ^^
  ```

- Warning: `subworkflows/local/hiv_resitance_detection/main.nf:94:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          RESISTANCE_TABLES.out.resistance_csv.collect{it[1]},
                                                       ^^
  ```

- Warning: `subworkflows/local/hiv_resitance_detection/main.nf:95:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          nextclade_report.collect{it[1]},
                                   ^^
  ```

- Warning: `subworkflows/local/hiv_resitance_detection/main.nf:96:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          consensus.collect{it[1]},
                            ^^
  ```

- Warning: `subworkflows/local/hiv_resitance_detection/main.nf:97:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          CONSENSUS_LIFTOFF.out.gff3.collect{it[1]}
                                             ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:45:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta    = GUNZIP_FASTA.out.gunzip.map { it[1] }
                                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:59:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gff      = GUNZIP_GFF.out.gunzip.map { it[1] }
                                                        ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:69:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta.map { [ [:], it, [] ] },
                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:72:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fai         = SAMTOOLS_FAIDX.out.fai.map { it[1] }
                                                    ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:73:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_chrom_sizes = SAMTOOLS_FAIDX.out.sizes.map { it[1] }
                                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:85:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_kraken2_db = UNTAR_KRAKEN2_DB.out.untar.map { it[1] }
                                                                   ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:109:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_primer_bed = GUNZIP_PRIMER_BED.out.gunzip.map { it[1] }
                                                                     ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:130:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      ch_primer_fasta = GUNZIP_PRIMER_FASTA.out.gunzip.map { it[1] }
                                                                             ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:136:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      ch_primer_bed.map { [ [:], it ] },
                                                 ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:179:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_nextclade_db = UNTAR_NEXTCLADE_DB.out.untar.map { it[1] }
                                                                       ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:212:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      ch_fasta.map { [ [:], it ] },
                                            ^^
  ```

- Warning: `subworkflows/local/prepare_genome_nanopore/main.nf:22:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      bowtie2_index
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome_nanopore/main.nf:38:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta    = GUNZIP_FASTA.out.gunzip.map { it[1] }
                                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome_nanopore/main.nf:52:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gff      = GUNZIP_GFF.out.gunzip.map { it[1] }
                                                        ^^
  ```

- Warning: `subworkflows/local/prepare_genome_nanopore/main.nf:62:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta.map { [ [:], it, [] ] },
                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome_nanopore/main.nf:65:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fai         = SAMTOOLS_FAIDX.out.fai.map { it[1] }
                                                    ^^
  ```

- Warning: `subworkflows/local/prepare_genome_nanopore/main.nf:66:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_chrom_sizes = SAMTOOLS_FAIDX.out.sizes.map { it[1] }
                                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome_nanopore/main.nf:78:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_kraken2_db = UNTAR_KRAKEN2_DB.out.untar.map { it[1] }
                                                                   ^^
  ```

- Warning: `subworkflows/local/prepare_genome_nanopore/main.nf:99:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_primer_bed = GUNZIP_PRIMER_BED.out.gunzip.map { it[1] }
                                                                 ^^
  ```

- Warning: `subworkflows/local/prepare_genome_nanopore/main.nf:129:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_nextclade_db = UNTAR.out.untar.map { it[1] }
                                                          ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralrecon_pipeline/main.nf:106:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, fastq_1, fastq_2, barcode->
                                          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralrecon_pipeline/main.nf:115:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  validateInputSamplesheet(it)
                                           ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralrecon_pipeline/main.nf:128:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      meta, fastq_1, fastq_2, barcode->
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralrecon_pipeline/main.nf:128:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      meta, fastq_1, fastq_2, barcode->
                                     ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralrecon_pipeline/main.nf:348:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input_file.eachLine { line ->
                            ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralrecon_pipeline/main.nf:357:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  def checkContigsInBED(fai_contigs, bed_contigs, log) {
                                                  ^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralrecon_pipeline/main.nf:384:17`: Variable was declared but not used

  ```nextflow
              def cells = headers.eachWithIndex { header, header_index ->
                  ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralrecon_pipeline/main.nf:417:9`: Variable was declared but not used

  ```nextflow
      def logname = flagstat_file.getBaseName() - 'flagstat'
          ^^^^^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:26:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta = fasta_fai.map { meta, fasta_file, fai_file -> fasta_file }
                                 ^^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:26:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta = fasta_fai.map { meta, fasta_file, fai_file -> fasta_file }
                                                   ^^^^^^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:40:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi, stats -> getNumVariantsFromBCFToolsStats(stats) > 0 }
                    ^^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:40:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi, stats -> getNumVariantsFromBCFToolsStats(stats) > 0 }
                          ^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:40:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi, stats -> getNumVariantsFromBCFToolsStats(stats) > 0 }
                               ^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:44:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, vcf, tbi, stats -> [ meta, vcf ] }
                            ^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:44:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, vcf, tbi, stats -> [ meta, vcf ] }
                                 ^^^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:48:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, vcf, tbi, stats -> [ meta, tbi ] }
                       ^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:48:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, vcf, tbi, stats -> [ meta, tbi ] }
                                 ^^^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:52:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, vcf, tbi, stats -> [ meta, stats ] }
                       ^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:52:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, vcf, tbi, stats -> [ meta, stats ] }
                            ^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:60:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta.map { [ [:], it ] }
                                ^^
  ```

- Warning: `subworkflows/local/variants_ivar/main.nf:45:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, tsv -> getNumLinesInFile(tsv) > 1 }
                    ^^^^
  ```

- Warning: `subworkflows/local/variants_long_table/main.nf:25:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          BCFTOOLS_QUERY.out.output.collect{it[1]},
                                            ^^
  ```

- Warning: `subworkflows/local/variants_long_table/main.nf:26:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          snpsift.collect{it[1]}.ifEmpty([]),
                          ^^
  ```

- Warning: `subworkflows/local/variants_long_table/main.nf:27:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          pangolin.collect{it[1]}.ifEmpty([])
                           ^^
  ```

- Warning: `subworkflows/local/variants_qc/main.nf:9:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      bam           // channel: [ val(meta), [ bam ] ]
      ^^^
  ```

- Warning: `subworkflows/local/variants_qc/main.nf:11:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      stats         // channel: [ val(meta), [ bcftools_stats ] ]
      ^^^^^
  ```

- Warning: `subworkflows/local/variants_qc/main.nf:13:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      sizes         // channel: /path/to/genome.sizes
      ^^^^^
  ```

- Warning: `subworkflows/local/variants_qc/main.nf:15:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      bed           // channel: /path/to/primers.bed
      ^^^
  ```

- Warning: `workflows/viralrecon.nf:106:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      multiqc_config
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:107:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      multiqc_logo
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:108:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      multiqc_methods_description
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:117:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_artic_scheme
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:130:9`: Variable was declared but not used

  ```nextflow
      def valid_params = [
          ^^^^^^^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:162:41`: Variable was declared but not used

  ```nextflow
      if (params.input)                 { ch_input          = file(params.input)                 } else { exit 1, 'Input samplesheet file not specified!' }
                                          ^^^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:182:80`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def assemblers = params.assemblers ? params.assemblers.split(',').collect{ it.trim().toLowerCase() } : []
                                                                                 ^^
  ```

- Warning: `workflows/viralrecon.nf:251:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { isMultiFasta(it, log) }
                                  ^^
  ```

- Warning: `workflows/viralrecon.nf:257:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { checkPrimerSuffixes(it, params.primer_left_suffix, params.primer_right_suffix, log) }
                                             ^^
  ```

- Warning: `workflows/viralrecon.nf:262:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { [ getColFromFile(it, 0, true) ] }
                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:267:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { [ getColFromFile(it, 0, true) ] }
                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:276:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .map { checkIfSwiftProtocol(it, 'covid19genome', log) }
                                                  ^^
  ```

- Warning: `workflows/viralrecon.nf:300:100`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQ_TRIM_FASTP_FASTQC.out.fastqc_raw_zip.collect{it[1]}.ifEmpty([]))
                                                                                                     ^^
  ```

- Warning: `workflows/viralrecon.nf:301:95`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQ_TRIM_FASTP_FASTQC.out.trim_json.collect{it[1]}.ifEmpty([]))
                                                                                                ^^
  ```

- Warning: `workflows/viralrecon.nf:317:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map { meta, reads, json, pass -> if (pass) [ meta, reads ] }
                                      ^^^^
  ```

- Warning: `workflows/viralrecon.nf:322:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      meta, reads, json, pass ->
                            ^^^^^
  ```

- Warning: `workflows/viralrecon.nf:352:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files =  ch_multiqc_files.mix(KRAKEN2_KRAKEN2.out.report.collect{it[1]}.ifEmpty([]))
                                                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:378:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQ_ALIGN_BOWTIE2.out.log_out.collect{it[1]}.ifEmpty([]))
                                                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:379:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQ_ALIGN_BOWTIE2.out.flagstat.collect{it[1]}.ifEmpty([]))
                                                                                           ^^
  ```

- Warning: `workflows/viralrecon.nf:393:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map { meta, ofile, mapped, pass -> if (pass) [ meta, ofile ] }
                                      ^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:398:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map { meta, ofile, mapped, pass -> if (pass) [ meta, ofile ] }
                                      ^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:437:96`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(BAM_TRIM_PRIMERS_IVAR.out.flagstat.collect{it[1]}.ifEmpty([]))
                                                                                                 ^^
  ```

- Warning: `workflows/viralrecon.nf:451:100`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(BAM_MARKDUPLICATES_PICARD.out.flagstat.collect{it[1]}.ifEmpty([]))
                                                                                                     ^^
  ```

- Warning: `workflows/viralrecon.nf:460:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  genome.fasta.map { [ [:], it ] },
                                            ^^
  ```

- Warning: `workflows/viralrecon.nf:461:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  genome.fai.map { [ [:], it ] }
                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:476:92`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(MOSDEPTH_GENOME.out.global_txt.collect{it[1]}.ifEmpty([]))
                                                                                             ^^
  ```

- Warning: `workflows/viralrecon.nf:478:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  MOSDEPTH_GENOME.out.regions_bed.collect { it[1] }
                                                            ^^
  ```

- Warning: `workflows/viralrecon.nf:491:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      MOSDEPTH_AMPLICON.out.regions_bed.collect { it[1] }
                                                                  ^^
  ```

- Warning: `workflows/viralrecon.nf:518:91`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(VARIANTS_IVAR.out.multiqc_tsv.collect{it[1]}.ifEmpty([]))
                                                                                            ^^
  ```

- Warning: `workflows/viralrecon.nf:519:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(VARIANTS_IVAR.out.stats.collect{it[1]}.ifEmpty([]))
                                                                                      ^^
  ```

- Warning: `workflows/viralrecon.nf:520:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(VARIANTS_IVAR.out.snpeff_csv.collect{it[1]}.ifEmpty([]))
                                                                                           ^^
  ```

- Warning: `workflows/viralrecon.nf:539:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(VARIANTS_BCFTOOLS.out.stats.collect{it[1]}.ifEmpty([]))
                                                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:540:94`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(VARIANTS_BCFTOOLS.out.snpeff_csv.collect{it[1]}.ifEmpty([]))
                                                                                               ^^
  ```

- Warning: `workflows/viralrecon.nf:572:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_genome_gff ? genome.gff.map { [ [:], it ] } : [ [:], [] ],
                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:578:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files    = ch_multiqc_files.mix(ch_pangolin_report.collect{it[1]}.ifEmpty([]))
                                                                                    ^^
  ```

- Warning: `workflows/viralrecon.nf:579:97`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files    = ch_multiqc_files.mix(CONSENSUS_IVAR.out.quast_results.collect{it[1]}.ifEmpty([]))
                                                                                                  ^^
  ```

- Warning: `workflows/viralrecon.nf:592:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_genome_gff ? genome.gff.map { [ [:], it ] } : [ [:], [] ],
                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:599:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files    = ch_multiqc_files.mix(CONSENSUS_BCFTOOLS.out.quast_results.collect{it[1]}.ifEmpty([]))
                                                                                                      ^^
  ```

- Warning: `workflows/viralrecon.nf:600:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files    = ch_multiqc_files.mix(ch_pangolin_report.collect{it[1]}.ifEmpty([]))
                                                                                    ^^
  ```

- Warning: `workflows/viralrecon.nf:650:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_annot       = GUNZIP_GFF.out.gunzip.map { it[1] }
                                                               ^^
  ```

- Warning: `workflows/viralrecon.nf:699:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files    = ch_multiqc_files.mix(CUTADAPT.out.log.collect{it[1]}.ifEmpty([]))
                                                                                  ^^
  ```

- Warning: `workflows/viralrecon.nf:717:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_genome_gff ? genome.gff.map { [ [:], it ] } : [ [:], [] ],
                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:723:95`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(ASSEMBLY_SPADES.out.quast_results.collect{it[1]}.ifEmpty([]))
                                                                                                ^^
  ```

- Warning: `workflows/viralrecon.nf:734:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_genome_gff ? genome.gff.map { [ [:], it ] } : [ [:], [] ],
                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:740:98`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(ASSEMBLY_UNICYCLER.out.quast_results.collect{it[1]}.ifEmpty([]))
                                                                                                   ^^
  ```

- Warning: `workflows/viralrecon.nf:751:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_genome_gff ? genome.gff.map { [ [:], it ] } : [ [:], [] ],
                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:757:94`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(ASSEMBLY_MINIA.out.quast_results.collect{it[1]}.ifEmpty([]))
                                                                                               ^^
  ```

- Warning: `workflows/viralrecon.nf:784:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  channel.of(ch_sequencing_summary).map { [ [:], it ] }
                                                                 ^^
  ```

- Warning: `workflows/viralrecon.nf:786:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(PYCOQC.out.json.collect{it[1]}.ifEmpty([]))
                                                                              ^^
  ```

- Warning: `workflows/viralrecon.nf:792:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { checkPrimerSuffixes(it, params.primer_left_suffix, params.primer_right_suffix, log) }
                                         ^^
  ```

- Warning: `workflows/viralrecon.nf:797:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { [ getColFromFile(it, 0, true) ] }
                                      ^^
  ```

- Warning: `workflows/viralrecon.nf:802:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { [ getColFromFile(it, 0, true) ] }
                                      ^^
  ```

- Warning: `workflows/viralrecon.nf:836:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { it[1] == null }
                                ^^
  ```

- Warning: `workflows/viralrecon.nf:837:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { it[-1] >= min_barcode_reads }
                                ^^
  ```

- Warning: `workflows/viralrecon.nf:854:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { it[-1] == null }
                                ^^
  ```

- Warning: `workflows/viralrecon.nf:869:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { (it[1] != null)  }
                                 ^^
  ```

- Warning: `workflows/viralrecon.nf:870:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { (it[-1] != null) }
                                 ^^
  ```

- Warning: `workflows/viralrecon.nf:891:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { barcode, sample, dir, count  ->
                        ^^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:891:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { barcode, sample, dir, count  ->
                                         ^^^
  ```

- Warning: `workflows/viralrecon.nf:917:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it[-1] > min_barcode_reads }
                        ^^
  ```

- Warning: `workflows/viralrecon.nf:918:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { barcode, sample, dir, count -> [ [ id: sample, barcode:barcode ], dir ] }
                                           ^^^^^
  ```

- Warning: `workflows/viralrecon.nf:943:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files =  ch_multiqc_files.mix(KRAKEN2_KRAKEN2.out.report.collect{it[1]}.ifEmpty([]))
                                                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:998:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ARTIC_GUPPYPLEX.out.fastq.filter { it[-1].countFastq() > min_guppyplex_reads },
                                                 ^^
  ```

- Warning: `workflows/viralrecon.nf:1003:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(ARTIC_MINION.out.json.collect{it[1]}.ifEmpty([]))
                                                                                ^^
  ```

- Warning: `workflows/viralrecon.nf:1030:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(BCFTOOLS_STATS.out.stats.collect{it[1]}.ifEmpty([]))
                                                                                   ^^
  ```

- Warning: `workflows/viralrecon.nf:1039:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FILTER_BAM_SAMTOOLS.out.flagstat.collect{it[1]}.ifEmpty([]))
                                                                                           ^^
  ```

- Warning: `workflows/viralrecon.nf:1055:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, bam, mapped, pass ->
                                ^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:1063:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, bai, mapped, pass ->
                                ^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:1071:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, fasta, mapped_reads, pass ->
                                  ^^^^^^^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:1114:93`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files  = ch_multiqc_files.mix(MOSDEPTH_GENOME.out.global_txt.collect{it[1]}.ifEmpty([]))
                                                                                              ^^
  ```

- Warning: `workflows/viralrecon.nf:1117:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  MOSDEPTH_GENOME.out.regions_bed.collect { it[1] }
                                                            ^^
  ```

- Warning: `workflows/viralrecon.nf:1130:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  MOSDEPTH_AMPLICON.out.regions_bed.collect { it[1] }
                                                              ^^
  ```

- Warning: `workflows/viralrecon.nf:1132:108`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(PLOT_MOSDEPTH_REGIONS_AMPLICON.out.heatmap_tsv.collect{it[1]}.ifEmpty([]))
                                                                                                             ^^
  ```

- Warning: `workflows/viralrecon.nf:1152:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      ch_pango_database = UNTAR_PANGODB.out.untar.map { it[1] }
                                                                        ^^
  ```

- Warning: `workflows/viralrecon.nf:1164:84`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files    = ch_multiqc_files.mix(ch_pangolin_multiqc.collect{it[1]}.ifEmpty([]))
                                                                                     ^^
  ```

- Warning: `workflows/viralrecon.nf:1216:102`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files  = ch_multiqc_files.mix(BAM_VARIANT_DEMIX_BOOT_FREYJA.out.demix.collect{it[1]}.ifEmpty([]))
                                                                                                       ^^
  ```

- Warning: `workflows/viralrecon.nf:1224:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .collect{ it[1] }
                            ^^
  ```

- Warning: `workflows/viralrecon.nf:1232:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(QUAST.out.results.collect{it[1]}.ifEmpty([]))
                                                                                ^^
  ```

- Warning: `workflows/viralrecon.nf:1246:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files  = ch_multiqc_files.mix(SNPEFF_SNPSIFT.out.csv.collect{it[1]}.ifEmpty([]))
                                                                                      ^^
  ```

- Warning: `workflows/viralrecon.nf:1274:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_annot       = GUNZIP_GFF.out.gunzip.map { it[1] }
                                                               ^^
  ```
