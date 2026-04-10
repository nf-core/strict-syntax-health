# Nextflow lint results

- Generated: 2026-04-10T00:28:01.302030794Z
- Nextflow version: 26.03.2-edge
- Summary: 180 warnings

## :warning: Warnings

- Warning: `modules/nf-core/bcftools/consensus/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/bcftools/consensus/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def masking = mask ? "-m $mask" : ""
          ^^^^^^^
  ```

- Warning: `modules/nf-core/bcftools/norm/main.nf:56:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          if (['--write-index=tbi', '-W=tbi'].any { args.contains(it) }  && extension == 'vcf.gz') {
                                                                  ^^
  ```

- Warning: `modules/nf-core/bcftools/norm/main.nf:58:126`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          } else if (['--write-index=tbi', '-W=tbi', '--write-index=csi', '-W=csi', '--write-index', '-W'].any { args.contains(it) }) {
                                                                                                                               ^^
  ```

- Warning: `modules/nf-core/blast/blastn/main.nf:65:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/blast/makeblastdb/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args           = task.ext.args ?: ''
          ^^^^
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

- Warning: `modules/nf-core/custom/getchromsizes/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/ivar/trim/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:60:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:62:9`: Variable was declared but not used

  ```nextflow
      def paired       = meta.single_end ? "" : "--paired"
          ^^^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:65:9`: Variable was declared but not used

  ```nextflow
      def readclassification_option = save_reads_assignment ? "--output ${prefix}.kraken2.classifiedreads.txt" : "--output /dev/null"
          ^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/kraken2/kraken2/main.nf:66:9`: Variable was declared but not used

  ```nextflow
      def compress_reads_command = save_output_fastqs ? "pigz -p $task.cpus *.fastq" : ""
          ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/quast/main.nf:52:9`: Variable was declared but not used

  ```nextflow
      def args      = task.ext.args   ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/quast/main.nf:54:9`: Variable was declared but not used

  ```nextflow
      def features  = gff             ? "--features $gff" : ''
          ^^^^^^^^
  ```

- Warning: `modules/nf-core/quast/main.nf:55:9`: Variable was declared but not used

  ```nextflow
      def reference = fasta           ? "-r $fasta" : ''
          ^^^^^^^^^
  ```

- Warning: `modules/nf-core/spades/main.nf:80:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/spades/main.nf:82:9`: Variable was declared but not used

  ```nextflow
      def maxmem = task.memory.toGiga()
          ^^^^^^
  ```

- Warning: `modules/nf-core/spades/main.nf:86:9`: Variable was declared but not used

  ```nextflow
      def custom_hmms = hmm ? "--custom-hmms $hmm" : ""
          ^^^^^^^^^^^
  ```

- Warning: `modules/nf-core/spades/main.nf:87:9`: Variable was declared but not used

  ```nextflow
      def reads = yml ? "--dataset $yml" : "$illumina_reads $pacbio_reads $nanopore_reads"
          ^^^^^
  ```

- Warning: `subworkflows/local/additional_annotation/main.nf:66:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          BCFTOOLS_QUERY.out.output.collect{it[1]},
                                            ^^
  ```

- Warning: `subworkflows/local/additional_annotation/main.nf:67:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          SNPSIFT_EXTRACTFIELDS.out.txt.collect{it[1]}.ifEmpty([]),
                                                ^^
  ```

- Warning: `subworkflows/local/additional_annotation/main.nf:68:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          pangolin.collect{it[1]}.ifEmpty([])
                           ^^
  ```

- Warning: `subworkflows/local/assembly_minia/main.nf:37:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, contig -> contig.size() > 0 }
                    ^^^^
  ```

- Warning: `subworkflows/local/assembly_qc/main.nf:56:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .collect{ it[1] }
                        ^^
  ```

- Warning: `subworkflows/local/assembly_qc/main.nf:62:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              fasta.map { [ [:], it ] },
                                 ^^
  ```

- Warning: `subworkflows/local/assembly_qc/main.nf:77:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

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

- Warning: `subworkflows/local/assembly_spades/main.nf:71:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, scaffold -> scaffold.size() > 0 }
                    ^^^^
  ```

- Warning: `subworkflows/local/assembly_spades/main.nf:77:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, gfa -> gfa.size() > 0 }
                    ^^^^
  ```

- Warning: `subworkflows/local/assembly_unicycler/main.nf:57:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, scaffold -> scaffold.size() > 0 }
                    ^^^^
  ```

- Warning: `subworkflows/local/assembly_unicycler/main.nf:63:19`: Parameter was not used -- prefix with `_` to suppress warning

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

- Warning: `subworkflows/local/filter_bam_samtools/main.nf:25:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          bam_bai.map { it[2].getName().tokenize('.')[-1] }
                        ^^
  ```

- Warning: `subworkflows/local/hiv_resitance_detection/main.nf:68:36`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              LIFTOFF.out.gff3.map { it[1] },
                                     ^^
  ```

- Warning: `subworkflows/local/hiv_resitance_detection/main.nf:98:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          SIERRALOCAL.out.json.collect{it[1]},
                                       ^^
  ```

- Warning: `subworkflows/local/hiv_resitance_detection/main.nf:99:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          RESISTANCE_TABLES.out.mutation_csv.collect{it[1]},
                                                     ^^
  ```

- Warning: `subworkflows/local/hiv_resitance_detection/main.nf:100:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          RESISTANCE_TABLES.out.resistance_csv.collect{it[1]},
                                                       ^^
  ```

- Warning: `subworkflows/local/hiv_resitance_detection/main.nf:101:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          nextclade_report.collect{it[1]},
                                   ^^
  ```

- Warning: `subworkflows/local/hiv_resitance_detection/main.nf:102:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          consensus.collect{it[1]},
                            ^^
  ```

- Warning: `subworkflows/local/hiv_resitance_detection/main.nf:103:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          CONSENSUS_LIFTOFF.out.gff3.collect{it[1]}
                                             ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:45:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta    = GUNZIP_FASTA.out.gunzip.map { it[1] }
                                                      ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:60:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gff      = GUNZIP_GFF.out.gunzip.map { it[1] }
                                                        ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:71:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta.map { [ [:], it ] }
                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:73:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fai         = CUSTOM_GETCHROMSIZES.out.fai.map { it[1] }
                                                          ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:74:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_chrom_sizes = CUSTOM_GETCHROMSIZES.out.sizes.map { it[1] }
                                                            ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:87:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_kraken2_db = UNTAR_KRAKEN2_DB.out.untar.map { it[1] }
                                                                   ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:112:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_primer_bed = GUNZIP_PRIMER_BED.out.gunzip.map { it[1] }
                                                                     ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:134:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      ch_primer_fasta = GUNZIP_PRIMER_FASTA.out.gunzip.map { it[1] }
                                                                             ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:141:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      ch_primer_bed.map { [ [:], it ] },
                                                 ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:167:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_fasta.map { [ [:], it ] }
                                        ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:184:70`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_nextclade_db = UNTAR_NEXTCLADE_DB.out.untar.map { it[1] }
                                                                       ^^
  ```

- Warning: `subworkflows/local/prepare_genome_illumina/main.nf:219:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      ch_fasta.map { [ [:], it ] }
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

- Warning: `subworkflows/local/prepare_genome_nanopore/main.nf:53:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_gff      = GUNZIP_GFF.out.gunzip.map { it[1] }
                                                        ^^
  ```

- Warning: `subworkflows/local/prepare_genome_nanopore/main.nf:64:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_fasta.map { [ [:], it ] }
                                ^^
  ```

- Warning: `subworkflows/local/prepare_genome_nanopore/main.nf:66:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_fai         = CUSTOM_GETCHROMSIZES.out.fai.map { it[1] }
                                                          ^^
  ```

- Warning: `subworkflows/local/prepare_genome_nanopore/main.nf:67:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_chrom_sizes = CUSTOM_GETCHROMSIZES.out.sizes.map { it[1] }
                                                            ^^
  ```

- Warning: `subworkflows/local/prepare_genome_nanopore/main.nf:80:66`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_kraken2_db = UNTAR_KRAKEN2_DB.out.untar.map { it[1] }
                                                                   ^^
  ```

- Warning: `subworkflows/local/prepare_genome_nanopore/main.nf:102:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_primer_bed = GUNZIP_PRIMER_BED.out.gunzip.map { it[1] }
                                                                 ^^
  ```

- Warning: `subworkflows/local/prepare_genome_nanopore/main.nf:132:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_nextclade_db = UNTAR.out.untar.map { it[1] }
                                                          ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralrecon_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralrecon_pipeline/main.nf:102:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  meta, fastq_1, fastq_2, barcode->
                                          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralrecon_pipeline/main.nf:111:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  validateInputSamplesheet(it)
                                           ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralrecon_pipeline/main.nf:124:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      meta, fastq_1, fastq_2, barcode->
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_viralrecon_pipeline/main.nf:124:36`: Parameter was not used -- prefix with `_` to suppress warning

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

- Warning: `subworkflows/local/variants_bcftools/main.nf:30:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          fasta.map { [ [:], it ] },
                             ^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:41:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi, stats -> getNumVariantsFromBCFToolsStats(stats) > 0 }
                    ^^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:41:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi, stats -> getNumVariantsFromBCFToolsStats(stats) > 0 }
                          ^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:41:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, vcf, tbi, stats -> getNumVariantsFromBCFToolsStats(stats) > 0 }
                               ^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:45:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, vcf, tbi, stats -> [ meta, vcf ] }
                            ^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:45:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, vcf, tbi, stats -> [ meta, vcf ] }
                                 ^^^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:49:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, vcf, tbi, stats -> [ meta, tbi ] }
                       ^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:49:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, vcf, tbi, stats -> [ meta, tbi ] }
                                 ^^^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:53:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, vcf, tbi, stats -> [ meta, stats ] }
                       ^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:53:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, vcf, tbi, stats -> [ meta, stats ] }
                            ^^^
  ```

- Warning: `subworkflows/local/variants_bcftools/main.nf:61:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          fasta.map { [ [:], it ] }
                             ^^
  ```

- Warning: `subworkflows/local/variants_ivar/main.nf:45:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, tsv -> getNumLinesInFile(tsv) > 1 }
                    ^^^^
  ```

- Warning: `subworkflows/local/variants_long_table/main.nf:28:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          BCFTOOLS_QUERY.out.output.collect{it[1]},
                                            ^^
  ```

- Warning: `subworkflows/local/variants_long_table/main.nf:29:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          snpsift.collect{it[1]}.ifEmpty([]),
                          ^^
  ```

- Warning: `subworkflows/local/variants_long_table/main.nf:30:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

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

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:113:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_artic_scheme
      ^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:122:9`: Variable was declared but not used

  ```nextflow
      def valid_params = [
          ^^^^^^^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:153:41`: Variable was declared but not used

  ```nextflow
      if (params.input)                 { ch_input          = file(params.input)                 } else { exit 1, 'Input samplesheet file not specified!' }
                                          ^^^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:173:80`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def assemblers = params.assemblers ? params.assemblers.split(',').collect{ it.trim().toLowerCase() } : []
                                                                                 ^^
  ```

- Warning: `workflows/viralrecon.nf:238:33`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { isMultiFasta(it, log) }
                                  ^^
  ```

- Warning: `workflows/viralrecon.nf:244:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { checkPrimerSuffixes(it, params.primer_left_suffix, params.primer_right_suffix, log) }
                                             ^^
  ```

- Warning: `workflows/viralrecon.nf:249:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { [ getColFromFile(it, 0, true) ] }
                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:254:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { [ getColFromFile(it, 0, true) ] }
                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:263:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .map { checkIfSwiftProtocol(it, 'covid19genome', log) }
                                                  ^^
  ```

- Warning: `workflows/viralrecon.nf:289:100`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQ_TRIM_FASTP_FASTQC.out.fastqc_raw_zip.collect{it[1]}.ifEmpty([]))
                                                                                                     ^^
  ```

- Warning: `workflows/viralrecon.nf:290:95`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQ_TRIM_FASTP_FASTQC.out.trim_json.collect{it[1]}.ifEmpty([]))
                                                                                                ^^
  ```

- Warning: `workflows/viralrecon.nf:307:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map { meta, reads, json, pass -> if (pass) [ meta, reads ] }
                                      ^^^^
  ```

- Warning: `workflows/viralrecon.nf:312:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      meta, reads, json, pass ->
                            ^^^^^
  ```

- Warning: `workflows/viralrecon.nf:342:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files =  ch_multiqc_files.mix(KRAKEN2_KRAKEN2.out.report.collect{it[1]}.ifEmpty([]))
                                                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:365:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  genome.fasta.map { [ [:], it ] }
                                            ^^
  ```

- Warning: `workflows/viralrecon.nf:369:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQ_ALIGN_BOWTIE2.out.log_out.collect{it[1]}.ifEmpty([]))
                                                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:370:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FASTQ_ALIGN_BOWTIE2.out.flagstat.collect{it[1]}.ifEmpty([]))
                                                                                           ^^
  ```

- Warning: `workflows/viralrecon.nf:385:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map { meta, ofile, mapped, pass -> if (pass) [ meta, ofile ] }
                                      ^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:390:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map { meta, ofile, mapped, pass -> if (pass) [ meta, ofile ] }
                                      ^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:425:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  genome.fasta.map { [ [:], it ] }
                                            ^^
  ```

- Warning: `workflows/viralrecon.nf:429:96`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(BAM_TRIM_PRIMERS_IVAR.out.flagstat.collect{it[1]}.ifEmpty([]))
                                                                                                 ^^
  ```

- Warning: `workflows/viralrecon.nf:439:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  genome.fasta.map { [ [:], it ] },
                                            ^^
  ```

- Warning: `workflows/viralrecon.nf:444:100`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(BAM_MARKDUPLICATES_PICARD.out.flagstat.collect{it[1]}.ifEmpty([]))
                                                                                                     ^^
  ```

- Warning: `workflows/viralrecon.nf:454:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  genome.fasta.map { [ [:], it ] },
                                            ^^
  ```

- Warning: `workflows/viralrecon.nf:470:92`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(MOSDEPTH_GENOME.out.global_txt.collect{it[1]}.ifEmpty([]))
                                                                                             ^^
  ```

- Warning: `workflows/viralrecon.nf:473:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  MOSDEPTH_GENOME.out.regions_bed.collect { it[1] }
                                                            ^^
  ```

- Warning: `workflows/viralrecon.nf:486:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      MOSDEPTH_AMPLICON.out.regions_bed.collect { it[1] }
                                                                  ^^
  ```

- Warning: `workflows/viralrecon.nf:513:91`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(VARIANTS_IVAR.out.multiqc_tsv.collect{it[1]}.ifEmpty([]))
                                                                                            ^^
  ```

- Warning: `workflows/viralrecon.nf:514:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(VARIANTS_IVAR.out.stats.collect{it[1]}.ifEmpty([]))
                                                                                      ^^
  ```

- Warning: `workflows/viralrecon.nf:515:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(VARIANTS_IVAR.out.snpeff_csv.collect{it[1]}.ifEmpty([]))
                                                                                           ^^
  ```

- Warning: `workflows/viralrecon.nf:534:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(VARIANTS_BCFTOOLS.out.stats.collect{it[1]}.ifEmpty([]))
                                                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:535:94`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(VARIANTS_BCFTOOLS.out.snpeff_csv.collect{it[1]}.ifEmpty([]))
                                                                                               ^^
  ```

- Warning: `workflows/viralrecon.nf:568:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_genome_gff ? genome.gff.map { [ [:], it ] } : [ [:], [] ],
                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:574:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files    = ch_multiqc_files.mix(ch_pangolin_report.collect{it[1]}.ifEmpty([]))
                                                                                    ^^
  ```

- Warning: `workflows/viralrecon.nf:575:97`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files    = ch_multiqc_files.mix(CONSENSUS_IVAR.out.quast_results.collect{it[1]}.ifEmpty([]))
                                                                                                  ^^
  ```

- Warning: `workflows/viralrecon.nf:588:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_genome_gff ? genome.gff.map { [ [:], it ] } : [ [:], [] ],
                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:595:101`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files    = ch_multiqc_files.mix(CONSENSUS_BCFTOOLS.out.quast_results.collect{it[1]}.ifEmpty([]))
                                                                                                      ^^
  ```

- Warning: `workflows/viralrecon.nf:596:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files    = ch_multiqc_files.mix(ch_pangolin_report.collect{it[1]}.ifEmpty([]))
                                                                                    ^^
  ```

- Warning: `workflows/viralrecon.nf:647:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_annot       = GUNZIP_GFF.out.gunzip.map { it[1] }
                                                               ^^
  ```

- Warning: `workflows/viralrecon.nf:686:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_primers =  genome.primer_fasta.collect { it[1] }
                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:689:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      genome.primer_fasta.collect { it[1] }
                                                    ^^
  ```

- Warning: `workflows/viralrecon.nf:699:81`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files    = ch_multiqc_files.mix(CUTADAPT.out.log.collect{it[1]}.ifEmpty([]))
                                                                                  ^^
  ```

- Warning: `workflows/viralrecon.nf:719:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_genome_gff ? genome.gff.map { [ [:], it ] } : [ [:], [] ],
                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:725:95`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(ASSEMBLY_SPADES.out.quast_results.collect{it[1]}.ifEmpty([]))
                                                                                                ^^
  ```

- Warning: `workflows/viralrecon.nf:736:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_genome_gff ? genome.gff.map { [ [:], it ] } : [ [:], [] ],
                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:742:98`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(ASSEMBLY_UNICYCLER.out.quast_results.collect{it[1]}.ifEmpty([]))
                                                                                                   ^^
  ```

- Warning: `workflows/viralrecon.nf:753:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_genome_gff ? genome.gff.map { [ [:], it ] } : [ [:], [] ],
                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:759:94`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(ASSEMBLY_MINIA.out.quast_results.collect{it[1]}.ifEmpty([]))
                                                                                               ^^
  ```

- Warning: `workflows/viralrecon.nf:773:64`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  channel.of(ch_sequencing_summary).map { [ [:], it ] }
                                                                 ^^
  ```

- Warning: `workflows/viralrecon.nf:775:77`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(PYCOQC.out.json.collect{it[1]}.ifEmpty([]))
                                                                              ^^
  ```

- Warning: `workflows/viralrecon.nf:782:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { checkPrimerSuffixes(it, params.primer_left_suffix, params.primer_right_suffix, log) }
                                         ^^
  ```

- Warning: `workflows/viralrecon.nf:787:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { [ getColFromFile(it, 0, true) ] }
                                      ^^
  ```

- Warning: `workflows/viralrecon.nf:792:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .map { [ getColFromFile(it, 0, true) ] }
                                      ^^
  ```

- Warning: `workflows/viralrecon.nf:826:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { it[1] == null }
                                ^^
  ```

- Warning: `workflows/viralrecon.nf:827:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { it[-1] >= params.min_barcode_reads }
                                ^^
  ```

- Warning: `workflows/viralrecon.nf:844:31`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { it[-1] == null }
                                ^^
  ```

- Warning: `workflows/viralrecon.nf:859:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { (it[1] != null)  }
                                 ^^
  ```

- Warning: `workflows/viralrecon.nf:860:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .filter { (it[-1] != null) }
                                 ^^
  ```

- Warning: `workflows/viralrecon.nf:881:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { barcode, sample, dir, count  ->
                        ^^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:881:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { barcode, sample, dir, count  ->
                                         ^^^
  ```

- Warning: `workflows/viralrecon.nf:907:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              .filter { it[-1] > params.min_barcode_reads }
                        ^^
  ```

- Warning: `workflows/viralrecon.nf:908:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { barcode, sample, dir, count -> [ [ id: sample, barcode:barcode ], dir ] }
                                           ^^^^^
  ```

- Warning: `workflows/viralrecon.nf:934:89`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files =  ch_multiqc_files.mix(KRAKEN2_KRAKEN2.out.report.collect{it[1]}.ifEmpty([]))
                                                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:990:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ARTIC_GUPPYPLEX.out.fastq.filter { it[-1].countFastq() > params.min_guppyplex_reads },
                                                 ^^
  ```

- Warning: `workflows/viralrecon.nf:996:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(ARTIC_MINION.out.json.collect{it[1]}.ifEmpty([]))
                                                                                ^^
  ```

- Warning: `workflows/viralrecon.nf:1026:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(BCFTOOLS_STATS.out.stats.collect{it[1]}.ifEmpty([]))
                                                                                   ^^
  ```

- Warning: `workflows/viralrecon.nf:1036:90`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(FILTER_BAM_SAMTOOLS.out.flagstat.collect{it[1]}.ifEmpty([]))
                                                                                           ^^
  ```

- Warning: `workflows/viralrecon.nf:1053:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, bam, mapped, pass ->
                                ^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:1061:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, bai, mapped, pass ->
                                ^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:1069:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, fasta, mapped_reads, pass ->
                                  ^^^^^^^^^^^^
  ```

- Warning: `workflows/viralrecon.nf:1111:93`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files  = ch_multiqc_files.mix(MOSDEPTH_GENOME.out.global_txt.collect{it[1]}.ifEmpty([]))
                                                                                              ^^
  ```

- Warning: `workflows/viralrecon.nf:1115:59`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  MOSDEPTH_GENOME.out.regions_bed.collect { it[1] }
                                                            ^^
  ```

- Warning: `workflows/viralrecon.nf:1128:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  MOSDEPTH_AMPLICON.out.regions_bed.collect { it[1] }
                                                              ^^
  ```

- Warning: `workflows/viralrecon.nf:1130:108`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(PLOT_MOSDEPTH_REGIONS_AMPLICON.out.heatmap_tsv.collect{it[1]}.ifEmpty([]))
                                                                                                             ^^
  ```

- Warning: `workflows/viralrecon.nf:1150:71`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      ch_pango_database = UNTAR_PANGODB.out.untar.map { it[1] }
                                                                        ^^
  ```

- Warning: `workflows/viralrecon.nf:1161:84`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files    = ch_multiqc_files.mix(ch_pangolin_multiqc.collect{it[1]}.ifEmpty([]))
                                                                                     ^^
  ```

- Warning: `workflows/viralrecon.nf:1213:102`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files  = ch_multiqc_files.mix(BAM_VARIANT_DEMIX_BOOT_FREYJA.out.demix.collect{it[1]}.ifEmpty([]))
                                                                                                       ^^
  ```

- Warning: `workflows/viralrecon.nf:1221:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .collect{ it[1] }
                            ^^
  ```

- Warning: `workflows/viralrecon.nf:1226:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  genome.fasta.collect().map { [ [:], it ] },
                                                      ^^
  ```

- Warning: `workflows/viralrecon.nf:1227:57`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_genome_gff ? genome.gff.map { [ [:], it ] } : [ [:], [] ],
                                                          ^^
  ```

- Warning: `workflows/viralrecon.nf:1229:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files = ch_multiqc_files.mix(QUAST.out.results.collect{it[1]}.ifEmpty([]))
                                                                                ^^
  ```

- Warning: `workflows/viralrecon.nf:1244:85`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              ch_multiqc_files  = ch_multiqc_files.mix(SNPEFF_SNPSIFT.out.csv.collect{it[1]}.ifEmpty([]))
                                                                                      ^^
  ```

- Warning: `workflows/viralrecon.nf:1274:62`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  ch_annot       = GUNZIP_GFF.out.gunzip.map { it[1] }
                                                               ^^
  ```
