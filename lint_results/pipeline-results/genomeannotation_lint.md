# Nextflow lint results

- Generated: 2026-11-19T00:13:45.448477962Z
- Nextflow version: 26.11.0-edge
- Summary: 242 errors, 74 warnings

## :x: Errors

- Error: `main.nf:84:9`: Workflow `PIPELINE_INITIALISATION` cannot be used as a variable

    ```nextflow
            PIPELINE_INITIALISATION.out.samplesheet
            ^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `modules/local/agat/spextractsequences/main.nf:38:24`: Conditional expression has inconsistent types -- true branch has type String but false branch has type Path

    ```nextflow
        def genome_fasta = is_compressed ? fasta.getBaseName() : fasta
                           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `modules/local/agat/spfilterincompletegenecodingmodels/main.nf:32:24`: Conditional expression has inconsistent types -- true branch has type String but false branch has type Path

    ```nextflow
        def genome_fasta = is_compressed ? fasta.getBaseName() : fasta
                           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `modules/local/bbmap/bbnorm/main.nf:25:25`: `id` is not defined

    ```nextflow
            tuple('bbnorm', id, file('*.log')) >> 'logs'
                            ^^
    ```

- Error: `modules/local/bbmap/bbnorm/main.nf:26:9`: Invalid process topic statement

    ```nextflow
            tuple val("${task.process}"), val('bbmap'), eval('bbversion.sh | grep -v "Duplicate cpuset"'), emit: versions_bbmap, topic: versions
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `modules/local/bbmap/bbnorm/main.nf:32:14`: `meta` is not defined

    ```nextflow
        input  = meta.single_end ? "in=${fastq.join(',')}" : "in=${fastq[0]} in2=${fastq[1]}"
                 ^^^^
    ```

- Error: `modules/local/bbmap/bbnorm/main.nf:33:14`: `meta` is not defined

    ```nextflow
        output = meta.single_end ? "out=${prefix}.fastq.gz" : "out1=${prefix}_1.nm.fastq.gz out2=${prefix}_2.nm.fastq.gz"
                 ^^^^
    ```

- Error: `modules/local/busco/busco/main.nf:46:34`: Unrecognized property `Mb` for type Integer

    ```nextflow
        def bbtools_memory_minimum = 120.Mb
                                     ^^^^^^
    ```

- Error: `modules/local/fastp/main.nf:38:21`: The `[` operator is not defined for operands with types Iterable<Path> and Integer

    ```nextflow
                --in1 ${reads[0]} \\
                        ^^^^^^^^
    ```

- Error: `modules/local/fastp/main.nf:55:21`: The `[` operator is not defined for operands with types Iterable<Path> and Integer

    ```nextflow
                --in1 ${reads[0]} \\
                        ^^^^^^^^
    ```

- Error: `modules/local/fastp/main.nf:56:21`: The `[` operator is not defined for operands with types Iterable<Path> and Integer

    ```nextflow
                --in2 ${reads[1]} \\
                        ^^^^^^^^
    ```

- Error: `modules/local/fastqc/main.nf:31:46`: List expression has inconsistent element types -- some elements have type ? while others have type String

    ```nextflow
        def old_new_pairs = reads.size() == 1 ? [[reads[0], "${prefix}.${reads[0].extension}"]] : reads.withIndex().collect { entry, index -> [entry, "${prefix}_${index + 1}.${entry.extension}"] }
                                                 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `modules/local/fastqc/main.nf:31:47`: The `[` operator is not defined for operands with types Iterable<Path> and Integer

    ```nextflow
        def old_new_pairs = reads.size() == 1 ? [[reads[0], "${prefix}.${reads[0].extension}"]] : reads.withIndex().collect { entry, index -> [entry, "${prefix}_${index + 1}.${entry.extension}"] }
                                                  ^^^^^^^^
    ```

- Error: `modules/local/fastqc/main.nf:31:70`: The `[` operator is not defined for operands with types Iterable<Path> and Integer

    ```nextflow
        def old_new_pairs = reads.size() == 1 ? [[reads[0], "${prefix}.${reads[0].extension}"]] : reads.withIndex().collect { entry, index -> [entry, "${prefix}_${index + 1}.${entry.extension}"] }
                                                                         ^^^^^^^^
    ```

- Error: `modules/local/fastqc/main.nf:31:101`: Unrecognized method `withIndex` for type Iterable<Path>

    ```nextflow
        def old_new_pairs = reads.size() == 1 ? [[reads[0], "${prefix}.${reads[0].extension}"]] : reads.withIndex().collect { entry, index -> [entry, "${prefix}_${index + 1}.${entry.extension}"] }
                                                                                                        ^^^^^^^^^
    ```

- Error: `modules/local/fastqc/main.nf:32:21`: Unrecognized method `join` for element type ?

    ```nextflow
        def rename_to = old_new_pairs*.join(' ').join(' ')
                        ^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `modules/local/gffread/main.nf:35:24`: Conditional expression has inconsistent types -- true branch has type String but false branch has type Path

    ```nextflow
        def genome_fasta = is_compressed ? fasta.getBaseName() : fasta
                           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `modules/local/hisat2/align/main.nf:64:18`: The `[` operator is not defined for operands with types Set<Path> and Integer

    ```nextflow
                -U ${reads[0]} \\
                     ^^^^^^^^
    ```

- Error: `modules/local/hisat2/align/main.nf:90:18`: The `[` operator is not defined for operands with types Set<Path> and Integer

    ```nextflow
                -1 ${reads[0]} \\
                     ^^^^^^^^
    ```

- Error: `modules/local/hisat2/align/main.nf:91:18`: The `[` operator is not defined for operands with types Set<Path> and Integer

    ```nextflow
                -2 ${reads[1]} \\
                     ^^^^^^^^
    ```

- Error: `modules/local/interproscan5/download_db/main.nf:6:12`: The `-` operator is not defined for operands with types String and String

    ```nextflow
        tag "${db_url.tokenize('/')[-1] - '.tar.gz'}"
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `modules/local/interproscan6/main.nf:76:10`: Unrecognized method `findAll` for type Map<String, String>

    ```nextflow
            .findAll { k, v -> !(k.startsWith('NXF') || k.startsWith('TOWER')) || k in nxf_passthrough }
             ^^^^^^^
    ```

- Error: `modules/local/interproscan6/main.nf:86:65`: Closure with signature () -> ? is not compatible with expected signature: (E) -> Boolean

    ```nextflow
        def valid_profiles = workflow.profile.tokenize(',').findAll { !it.startsWith('test_') }
                                                                    ^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `modules/local/interproscan6/main.nf:110:19`: List expression has inconsistent element types -- some elements have type String while others have type ?

    ```nextflow
        def nxf_cmd = [
                      ^
    ```

- Error: `modules/local/interproscan6/main.nf:125:7`: Unrecognized method `minus` for type List<?>

    ```nextflow
        ].minus("").join(" ")
          ^^^^^
    ```

- Error: `modules/local/interproscan6/main.nf:135:57`: Unrecognized method `toFile` for type Path

    ```nextflow
        def process = nxf_cmd.execute(child_env, cache_path.toFile())
                                                            ^^^^^^
    ```

- Error: `modules/local/interproscan6/main.nf:158:35`: Unrecognized method `execute` for type List<String>

    ```nextflow
        def clean_process = clean_cmd.execute(child_env, cache_path.toFile())
                                      ^^^^^^^
    ```

- Error: `modules/local/interproscan6/main.nf:158:65`: Unrecognized method `toFile` for type Path

    ```nextflow
        def clean_process = clean_cmd.execute(child_env, cache_path.toFile())
                                                                    ^^^^^^
    ```

- Error: `modules/local/repeatmodeler/repeatmodeler/main.nf:37:24`: The `[` operator is not defined for operands with types Set<Path> and Integer

    ```nextflow
        def db_name = file(db[0]).getBaseName()
                           ^^^^^
    ```

- Error: `modules/local/seqtk/sample/main.nf:36:19`: The `>=` operator is not defined for operands with types Number and Integer

    ```nextflow
        sample_size = sample_size >= 1 ? sample_size.toInteger() : sample_size
                      ^^^^^^^^^^^^^^^^
    ```

- Error: `modules/local/seqtk/sample/main.nf:36:50`: Unrecognized method `toInteger` for type Number

    ```nextflow
        sample_size = sample_size >= 1 ? sample_size.toInteger() : sample_size
                                                     ^^^^^^^^^
    ```

- Error: `modules/local/sratools/prefetch/main.nf:20:27`: The `[` operator is not defined for operands with types String and List<Integer>

    ```nextflow
                sra: files("${id[0..1]}*", type: 'dir')
                              ^^^^^^^^
    ```

- Error: `modules/local/sratools/prefetch/main.nf:29:29`: The `[` operator is not defined for operands with types String and List<Integer>

    ```nextflow
        def two_first_letters = id[0..1]
                                ^^^^^^^^
    ```

- Error: `modules/local/star/align/main.nf:38:33`: The `[` operator is not defined for operands with types Set<Path> and Integer

    ```nextflow
        def read_file_command_arg = reads[0].extension == 'gz' ? "--readFilesCommand zcat": ''
                                    ^^^^^^^^
    ```

- Error: `modules/local/tiberius/tiberius/main.nf:4:10`: `id` is not defined

    ```nextflow
        tag "$id"
             ^^^
    ```

- Error: `modules/local/tiberius/tiberius/main.nf:13:9`: Invalid input declaration in typed process

    ```nextflow
            record(
            ^
    ```

- Error: `modules/local/tiberius/tiberius/main.nf:28:38`: `id` is not defined

    ```nextflow
        def prefix = task.ext.prefix ?: "$id"
                                         ^^^
    ```

- Error: `modules/local/tiberius/tiberius/main.nf:29:25`: `fasta` is not defined

    ```nextflow
        def is_compressed = fasta.getExtension() == "gz"    ? true : false
                            ^^^^^
    ```

- Error: `modules/local/tiberius/tiberius/main.nf:30:59`: `fasta` is not defined

    ```nextflow
        def fasta_name    = is_compressed                   ? fasta.getBaseName() : fasta.name
                                                              ^^^^^
    ```

- Error: `modules/local/tiberius/tiberius/main.nf:30:81`: `fasta` is not defined

    ```nextflow
        def fasta_name    = is_compressed                   ? fasta.getBaseName() : fasta.name
                                                                                    ^^^^^
    ```

- Error: `modules/local/tiberius/tiberius/main.nf:41:93`: `tiberius_lineage` is not defined

    ```nextflow
        MODEL_URL="https://raw.githubusercontent.com/Gaius-Augustus/Tiberius/v2.0.7/model_cfg/${tiberius_lineage}.yaml"
                                                                                                ^^^^^^^^^^^^^^^^
    ```

- Error: `modules/local/tiberius/tiberius/main.nf:42:41`: `tiberius_lineage` is not defined

    ```nextflow
        wget \$MODEL_URL -O \${MODEL_CFG}/${tiberius_lineage}.yaml
                                            ^^^^^^^^^^^^^^^^
    ```

- Error: `modules/local/tiberius/tiberius/main.nf:49:22`: `fasta` is not defined

    ```nextflow
            gzip -c -d ${fasta} > ${fasta_name}
                         ^^^^^
    ```

- Error: `modules/local/tiberius/tiberius/main.nf:58:21`: `tiberius_lineage` is not defined

    ```nextflow
            --model_cfg $tiberius_lineage \\
                        ^^^^^^^^^^^^^^^^^
    ```

- Error: `modules/local/tsebra/tsebra/main.nf:34:44`: Closure with signature () -> ? is not compatible with expected signature: (E) -> R

    ```nextflow
        def gtf_arg     = '-g ' + gtfs.collect { "$it" }.join(',')
                                               ^^^^^^^^^
    ```

- Error: `modules/local/tsebra/tsebra/main.nf:35:50`: Closure with signature () -> ? is not compatible with expected signature: (E) -> R

    ```nextflow
        def hints_arg   = '-e ' + hintsfiles.collect { "$it" }.join(',')
                                                     ^^^^^^^^^
    ```

- Error: `subworkflows/local/bam_sort_index_stats/main.nf:34:9`: Argument with type Record is not compatible with process input of type Record {
    id: String
    fasta: Path
}

    ```nextflow
            ch_input.map { rec -> rec.subMap(['id', 'fasta']) }.unique()
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/bam_sort_index_stats/main.nf:46:26`: Unrecognized property `read_id` for type Bam

    ```nextflow
                    read_id: subrec.read_id,
                             ^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/bam_sort_index_stats/main.nf:48:22`: Unrecognized property `bai` for type Bam

    ```nextflow
                    bai: subrec.bai,
                         ^^^^^^^^^^
    ```

- Error: `subworkflows/local/bam_sort_index_stats/main.nf:51:22`: Unrecognized property `fai` for type Input

    ```nextflow
                    fai: rec.fai,
                         ^^^^^^^
    ```

- Error: `subworkflows/local/bam_sort_index_stats/main.nf:52:32`: Unrecognized property `user_supplied` for type Bam

    ```nextflow
                    user_supplied: subrec.user_supplied
                                   ^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:48:57`: Unrecognized property `short_read_mappings` for type Input

    ```nextflow
        ch_merge_me               = ch_input.filter{ rec -> rec.short_read_mappings.size() > 1 }
                                                            ^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:49:57`: Unrecognized property `short_read_mappings` for type Input

    ```nextflow
        ch_not_no_merge           = ch_input.filter{ rec -> rec.short_read_mappings.size() == 1 }
                                                            ^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:50:57`: Unrecognized property `short_read_mappings` for type Input

    ```nextflow
        ch_no_short_read_mappings = ch_input.filter{ rec -> rec.short_read_mappings.size() == 0 }
                                                            ^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:53:20`: Unrecognized property `short_read_mappings` for type Input

    ```nextflow
            def bams = rec.short_read_mappings.collect { r -> r.bam }.toSorted()
                       ^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:54:20`: Unrecognized property `short_read_mappings` for type Input

    ```nextflow
            def bais = rec.short_read_mappings.collect { r -> r.bai }.toSorted()
                       ^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:61:71`: Unrecognized property `short_read_mappings` for type Input

    ```nextflow
        ch_not_no_merge  = ch_not_no_merge.map { rec -> rec + record(bam: rec.short_read_mappings[0].bam) }
                                                                          ^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:112:5`: Assignment target with type Channel<Record {
    id: String
    braker_gtf: Path
    braker_hintsfile: Path
}> cannot be assigned to value with type Channel<Record {
    id: String
    isoseq_braker_gtf: Path
    isoseq_braker_hintsfile: Path
}>

    ```nextflow
        ch_isoseq_braker_out = ch_isoseq_braker_out
        ^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:132:5`: Assignment target with type Channel<Input> cannot be assigned to value with type Channel<Record {
    tsebra_gtfs: ?
    tsebra_hintsfiles: ?
}>

    ```nextflow
        ch_input = ch_input
        ^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:135:63`: Unrecognized property `isoseq_braker_gtf` for type Record {
    id: String
    fasta: Path
    species: String
    mappings: List<Mapping>
    long_read_mappings: List<Mapping>
    proteins_fasta: Path
    tsebra_gtfs: Set<Path>
    tsebra_hintsfiles: Set<Path>
    braker_gtf: Path
    braker_hintsfile: Path
}

    ```nextflow
                        .filter{ rec -> rec.braker_gtf != null || rec.isoseq_braker_gtf != null } // keeping only ercords for which at least a braker gtf is present
                                                                  ^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:137:53`: Unrecognized method `keySet` for type Record {
    id: String
    fasta: Path
    species: String
    mappings: List<Mapping>
    long_read_mappings: List<Mapping>
    proteins_fasta: Path
    tsebra_gtfs: Set<Path>
    tsebra_hintsfiles: Set<Path>
    braker_gtf: Path
    braker_hintsfile: Path
}

    ```nextflow
                            def newrec = rec.subMap(rec.keySet() - ['braker_gtf', 'braker_hintsfile', 'isoseq_braker_gtf', 'isoseq_braker_hintsfile']) + record(
                                                        ^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:138:42`: Unrecognized property `supplied_tsebra_gtfs` for type Record {
    id: String
    fasta: Path
    species: String
    mappings: List<Mapping>
    long_read_mappings: List<Mapping>
    proteins_fasta: Path
    tsebra_gtfs: Set<Path>
    tsebra_hintsfiles: Set<Path>
    braker_gtf: Path
    braker_hintsfile: Path
}

    ```nextflow
                                tsebra_gtfs: rec.supplied_tsebra_gtfs + [rec.braker_gtf, rec.isoseq_braker_gtf].findAll(),
                                             ^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:138:69`: List expression has inconsistent element types -- some elements have type Path while others have type ?

    ```nextflow
                                tsebra_gtfs: rec.supplied_tsebra_gtfs + [rec.braker_gtf, rec.isoseq_braker_gtf].findAll(),
                                                                        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:138:86`: Unrecognized property `isoseq_braker_gtf` for type Record {
    id: String
    fasta: Path
    species: String
    mappings: List<Mapping>
    long_read_mappings: List<Mapping>
    proteins_fasta: Path
    tsebra_gtfs: Set<Path>
    tsebra_hintsfiles: Set<Path>
    braker_gtf: Path
    braker_hintsfile: Path
}

    ```nextflow
                                tsebra_gtfs: rec.supplied_tsebra_gtfs + [rec.braker_gtf, rec.isoseq_braker_gtf].findAll(),
                                                                                         ^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:138:109`: Function `findAll` expects 1 argument(s) but received 0

    ```nextflow
                                tsebra_gtfs: rec.supplied_tsebra_gtfs + [rec.braker_gtf, rec.isoseq_braker_gtf].findAll(),
                                                                                                                ^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:139:48`: Unrecognized property `supplied_tsebra_hintsfiles` for type Record {
    id: String
    fasta: Path
    species: String
    mappings: List<Mapping>
    long_read_mappings: List<Mapping>
    proteins_fasta: Path
    tsebra_gtfs: Set<Path>
    tsebra_hintsfiles: Set<Path>
    braker_gtf: Path
    braker_hintsfile: Path
}

    ```nextflow
                                tsebra_hintsfiles: rec.supplied_tsebra_hintsfiles + [rec.braker_hintsfile, rec.isoseq_braker_hintsfile].findAll()
                                                   ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:139:81`: List expression has inconsistent element types -- some elements have type Path while others have type ?

    ```nextflow
                                tsebra_hintsfiles: rec.supplied_tsebra_hintsfiles + [rec.braker_hintsfile, rec.isoseq_braker_hintsfile].findAll()
                                                                                    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:139:104`: Unrecognized property `isoseq_braker_hintsfile` for type Record {
    id: String
    fasta: Path
    species: String
    mappings: List<Mapping>
    long_read_mappings: List<Mapping>
    proteins_fasta: Path
    tsebra_gtfs: Set<Path>
    tsebra_hintsfiles: Set<Path>
    braker_gtf: Path
    braker_hintsfile: Path
}

    ```nextflow
                                tsebra_hintsfiles: rec.supplied_tsebra_hintsfiles + [rec.braker_hintsfile, rec.isoseq_braker_hintsfile].findAll()
                                                                                                           ^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:139:133`: Function `findAll` expects 1 argument(s) but received 0

    ```nextflow
                                tsebra_hintsfiles: rec.supplied_tsebra_hintsfiles + [rec.braker_hintsfile, rec.isoseq_braker_hintsfile].findAll()
                                                                                                                                        ^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:167:5`: Assignment target with type Channel<Record {
    id: String
    bam: Path
}> cannot be assigned to value with type Channel<Record {
    id: String
    fasta: Path
    species: String
    mappings: List<Mapping>
    long_read_mappings: List<Mapping>
    proteins_fasta: Path
    tsebra_gtfs: Set<Path>
    tsebra_hintsfiles: Set<Path>
    merged_gtf: Path
}>

    ```nextflow
        ch_merged = ch_to_merge_with_tsebra.join(ch_tsebra_out, by: 'id')
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:173:87`: Unrecognized property `merged_gtf` for type Record {
    id: String
    bam: Path
}

    ```nextflow
        ch_merged       = ch_merged.map      { rec -> rec + record(structural_annotation: rec.merged_gtf) }
                                                                                          ^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:175:87`: The `[` operator is not defined for operands with types Set<Path> and Integer

    ```nextflow
        ch_not_to_merge = ch_not_to_merge.map{ rec -> rec + record(structural_annotation: rec.tsebra_gtfs[0]) }
                                                                                          ^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/braker3/main.nf:178:15`: Function `mix` (with multiple signatures) was called with incorrect number of arguments and/or incorrect argument types

    ```nextflow
        ch_merged.mix( ch_not_to_merge )
                  ^^^
    ```

- Error: `subworkflows/local/busco/main.nf:51:47`: Unrecognized property `busco_lineage` for type Input

    ```nextflow
        ch_busco_input = ch_input.filter { rec -> rec.busco_lineage != null }
                                                  ^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/busco/main.nf:54:37`: Unrecognized property `busco_lineage` for type Input

    ```nextflow
            ch_busco_input.map { rec -> rec.busco_lineage }.unique()
                                        ^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/busco/main.nf:57:67`: Join field `busco_lineage` is not present in left-hand side

    ```nextflow
        ch_busco_input = ch_busco_input.join( ch_busco_downloads, by: 'busco_lineage' )
                                                                      ^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/busco/main.nf:66:24`: Unrecognized property `fasta` for type Input

    ```nextflow
                    fasta: rec.fasta, 
                           ^^^^^^^^^
    ```

- Error: `subworkflows/local/busco/main.nf:67:26`: Unrecognized property `busco_lineage` for type Input

    ```nextflow
                    lineage: rec.busco_lineage, 
                             ^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/busco/main.nf:68:32`: Unrecognized property `busco_download_path` for type Input

    ```nextflow
                    download_path: rec.busco_download_path
                                   ^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/busco/main.nf:82:22`: Unrecognized property `busco_lineage` for type Input

    ```nextflow
                lineage: rec.busco_lineage, 
                         ^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/busco/main.nf:83:28`: Unrecognized property `busco_download_path` for type Input

    ```nextflow
                download_path: rec.busco_download_path,
                               ^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/busco/main.nf:89:22`: Unrecognized property `busco_lineage` for type Input

    ```nextflow
                lineage: rec.busco_lineage, 
                         ^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/busco/main.nf:90:28`: Unrecognized property `busco_download_path` for type Input

    ```nextflow
                download_path: rec.busco_download_path,
                               ^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/busco/main.nf:93:9`: The `+` operator is not defined for operands with types List<Record {
    id: String
    fasta: Path
    lineage: ?
    download_path: ?
    reference: Boolean
}> and Iterable<Record {
    id: String
    fasta: Path
    lineage: ?
    download_path: ?
    reference: Boolean
}>

    ```nextflow
            [ main_proteome ] + other_proteomes
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/clean_annotation/main.nf:70:59`: Argument with type Input is not compatible with process input of type Record {
    id: String
    gff: Path
}

    ```nextflow
            ch_out = AGAT_FIX_FEATURE_LOCATIONS_DUPLICATIONS( ch_input )
                                                              ^^^^^^^^
    ```

- Error: `subworkflows/local/clean_annotation/main.nf:76:46`: Argument with type Input is not compatible with process input of type Record {
    id: String
    gff: Path
}

    ```nextflow
            ch_out = AGAT_FIX_OVERLAPPING_GENES( ch_input )
                                                 ^^^^^^^^
    ```

- Error: `subworkflows/local/clean_annotation/main.nf:82:61`: Argument with type Input is not compatible with process input of type Record {
    id: String
    gff: Path
    fasta: Path
}

    ```nextflow
            ch_out = AGAT_FILTER_INCOMPLETE_GENE_CODING_MODELS( ch_input )
                                                                ^^^^^^^^
    ```

- Error: `subworkflows/local/complement_annotation/main.nf:36:5`: Assignment target with type Channel<Input> cannot be assigned to value with type Channel<Record {
    id: String
    ref_gff: Path
    other_gff: Path
}>

    ```nextflow
        ch_to_complement = ch_to_complement.map { rec ->
        ^
    ```

- Error: `subworkflows/local/complement_annotation/main.nf:52:53`: Argument with type Input is not compatible with process input of type Record {
    id: String
    gff: Path
    reference_gff: Path
}

    ```nextflow
        ch_complemented = AGAT_SPCOMPLEMENTANNOTATIONS( ch_to_complement )
                                                        ^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/complement_annotation/main.nf:54:5`: Assignment target with type Channel<Record {
    id: String
    gff: Path
}> cannot be assigned to value with type Channel<Record {
    id: String
    structural_annotation: Path
    reference_gff: Path
}>

    ```nextflow
        ch_complemented = ch_to_complement.join( 
        ^
    ```

- Error: `subworkflows/local/complement_annotation/main.nf:61:21`: Function `mix` (with multiple signatures) was called with incorrect number of arguments and/or incorrect argument types

    ```nextflow
        ch_complemented.mix( ch_leave_me_alone )
                        ^^^
    ```

- Error: `subworkflows/local/deinterleave/main.nf:35:60`: Unrecognized property `interleaved` for type Input

    ```nextflow
        ch_interleaved_reads = ch_single_reads.filter { rec -> rec.interleaved == true }
                                                               ^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/deinterleave/main.nf:36:60`: Unrecognized property `interleaved` for type Input

    ```nextflow
        ch_single_end_reads  = ch_single_reads.filter { rec -> rec.interleaved == false }
                                                               ^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/deinterleave/main.nf:46:52`: Function `mix` (with multiple signatures) was called with incorrect number of arguments and/or incorrect argument types

    ```nextflow
        ch_paired_end_reads.mix( ch_single_end_reads ).mix( ch_deinterleaved )
                                                       ^^^
    ```

- Error: `subworkflows/local/download_reads/main.nf:28:39`: Unrecognized property `short_read_sra_ids` for type ExperimentIDs

    ```nextflow
                            .map { rec -> rec.short_read_sra_ids + rec.long_read_sra_ids }
                                          ^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/download_reads/main.nf:28:64`: Unrecognized property `long_read_sra_ids` for type ExperimentIDs

    ```nextflow
                            .map { rec -> rec.short_read_sra_ids + rec.long_read_sra_ids }
                                                                   ^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/download_reads/main.nf:59:13`: Argument with type Float is not compatible with process input of type Number

    ```nextflow
                read_sampling_size
                ^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/download_reads/main.nf:72:5`: Assignment target with type Channel<Record {
    id: String
    reads: Set<Path>
}> cannot be assigned to value with type Channel<Record {
    sra_id: String
    reads: Set<Path>
}>

    ```nextflow
        ch_downloaded_reads = ch_downloaded_reads.map{ rec -> record(sra_id: rec.id, reads: rec.reads) }
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/download_reads/main.nf:77:48`: Unrecognized property `short_read_sra_ids` for type ExperimentIDs

    ```nextflow
                                            rec -> rec.short_read_sra_ids.collect{ value -> record(id: rec.id, sra_id: value) }
                                                   ^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/download_reads/main.nf:91:48`: Unrecognized property `long_read_sra_ids` for type ExperimentIDs

    ```nextflow
                                            rec -> rec.long_read_sra_ids.collect{ value -> record(id: rec.id, sra_id: value) }
                                                   ^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/extract_sequences/main.nf:31:41`: Argument with type Input is not compatible with process input of type Record {
    id: String
    gff: Path
    fasta: Path
}

    ```nextflow
        ch_proteome = FROM_MAIN_ANNOTATION( ch_input )
                                            ^^^^^^^^
    ```

- Error: `subworkflows/local/extract_sequences/main.nf:44:23`: Conditional expression has inconsistent types -- true branch has type Set<Path> but false branch has type List<E>

    ```nextflow
            def alt_gff = rec.alternative_annotations ?: []
                          ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/extract_sequences/main.nf:45:27`: Conditional expression has inconsistent types -- true branch has type Set<Path> but false branch has type List<E>

    ```nextflow
            def interm_gffs = rec.intermediate_annotations ?: []
                              ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/extract_sequences/main.nf:55:34`: Closure with signature (?, ?) -> ? is not compatible with expected signature: (E) -> R

    ```nextflow
                                .map { id, fasta_list -> record(id: id, other_proteomes: fasta_list) }
                                     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/fastq_align_hisat2/main.nf:67:9`: Argument with type Record is not compatible with process input of type Record {
    id: String
    fasta: Path
    splice_sites: Path?
    exons: Path?
}

    ```nextflow
            ch_input.map { rec -> rec.subMap(['id', 'fasta', 'splice_sites', 'exons']) }.unique()
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/fastq_align_hisat2/main.nf:83:9`: Argument with type Record {
    id: String
    read_id: String
    reads: List<Path>
    fasta: Path
    reference_gtf: Path
    index: Path
} is not compatible with process input of type Record {
    id: String
    reads: Set<Path>
    read_id: String
    index: Path
    strandedness: String?
}

    ```nextflow
            ch_input_with_index.join(ch_strandedness_inferred, by: 'read_id')
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/fastq_align_hisat2/main.nf:83:64`: Join field `read_id` is not present in right-hand side

    ```nextflow
            ch_input_with_index.join(ch_strandedness_inferred, by: 'read_id')
                                                                   ^^^^^^^^^
    ```

- Error: `subworkflows/local/fastq_align_minimap2/main.nf:32:9`: Argument with type Record is not compatible with process input of type Record {
    id: String
    fasta: Path
}

    ```nextflow
            ch_input.map { rec -> rec.subMap(['id', 'fasta']) }.unique()
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/fastq_align_minimap2/main.nf:41:34`: Argument with type Record {
    id: String
    read_id: String
    reads: List<Path>
    fasta: Path
    index: Path
} is not compatible with process input of type Record {
    id: String
    read_id: String
    fastq: Path
    index: Path
}

    ```nextflow
        ch_aligned = MINIMAP2_ALIGN( ch_input_with_index )
                                     ^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/fastq_align_star/main.nf:36:9`: Argument with type Record {
    id: String
    read_id: String
    reads: List<Path>
    fasta: Path
    reference_gtf: Path
    index: Path
} is not compatible with process input of type Record {
    id: String
    reads: Set<Path>
    read_id: String
    index: Path
}

    ```nextflow
            ch_input.join(ch_star_index, by: 'id')
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/functional_annotation/main.nf:53:107`: Unrecognized property `eggnog_mapper_db` for type Input

    ```nextflow
                ch_input.map { rec -> record(id: rec.id, fasta: rec.proteome, gff: rec.gff, eggnog_mapper_db: rec.eggnog_mapper_db) },
                                                                                                              ^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/functional_annotation/main.nf:87:71`: Named param `checkExists` is not defined

    ```nextflow
                    interproscan_db = channel.fromPath( interproscan5_db, checkExists: true )
                                                                          ^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/functional_annotation/main.nf:89:17`: Assignment target with type Channel<Path> cannot be assigned to value with type Value<Path>

    ```nextflow
                    interproscan_db = INTERPROSCAN5_DOWNLOADDB( channel.value( interproscan5_db_url ) )
                    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/functional_annotation/main.nf:96:35`: Process `INTERPROSCAN5_INTERPROSCAN` was called with multiple channel arguments which can lead to non-deterministic behavior -- make sure that at most one argument is a channel and that all other arguments are dataflow values

    ```nextflow
                ch_interproscan_out = INTERPROSCAN5( 
                                      ^
    ```

- Error: `subworkflows/local/functional_annotation/main.nf:114:69`: Argument with type Input is not compatible with process input of type Record {
    id: String
    gff: Path
    interproscan_gff: Path
}

    ```nextflow
                ch_complemented = COMPLEMENT_GFF_WITH_INTERPROSCAN_GFF( ch_input )
                                                                        ^^^^^^^^
    ```

- Error: `subworkflows/local/genome_masking/main.nf:50:55`: Unrecognized property `lib` for type Genome

    ```nextflow
            ch_can_be_masked    = ch_input.filter{ rec -> rec.lib != null }
                                                          ^^^^^^^
    ```

- Error: `subworkflows/local/genome_masking/main.nf:51:55`: Unrecognized property `lib` for type Genome

    ```nextflow
            ch_cannot_be_masked = ch_input.filter{ rec -> rec.lib == null }
                                                          ^^^^^^^
    ```

- Error: `subworkflows/local/genome_masking/main.nf:53:35`: Argument with type Genome is not compatible with process input of type Record {
    id: String
    fasta: Path
    lib: Path
}

    ```nextflow
            ch_masked = REPEATMASKER( ch_can_be_masked )
                                      ^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/genome_masking/main.nf:68:13`: Assignment target with type Channel<Path> cannot be assigned to value with type Channel<Record {
    taxid: String
    dfam_db: Path
}>

    ```nextflow
                ch_dfam_db = FAMDB_DOWNLOAD_DFAM(
                ^
    ```

- Error: `subworkflows/local/genome_masking/main.nf:69:17`: Argument with type Record {
    taxid: ?
    taxid_lineage: Integer
} is not compatible with process input of type Record {
    taxid: String
    taxid_lineage: String
}

    ```nextflow
                    ch_input.map { rec -> record(taxid: rec.taxid, taxid_lineage: rec.taxid_lineage) }.unique()
                    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/genome_masking/main.nf:69:53`: Unrecognized property `taxid` for type Genome

    ```nextflow
                    ch_input.map { rec -> record(taxid: rec.taxid, taxid_lineage: rec.taxid_lineage) }.unique()
                                                        ^^^^^^^^^
    ```

- Error: `subworkflows/local/genome_masking/main.nf:72:39`: Argument with type Channel<Path> is not compatible with parameter of type Channel<Record>

    ```nextflow
                ch_input = ch_input.join( ch_dfam_db, by: 'taxid' )
                                          ^^^^^^^^^^
    ```

- Error: `subworkflows/local/genome_masking/main.nf:76:31`: Argument with type Genome is not compatible with process input of type Record {
    id: String
    taxid: String
    fasta: Path
    dfam_db: Path
}

    ```nextflow
            ch_masked = EARLGREY( ch_input )
                                  ^^^^^^^^
    ```

- Error: `subworkflows/local/genome_masking/main.nf:80:5`: Assignment target with type Channel<Record {
    id: String
    softmasked: Path
}> cannot be assigned to value with type Channel<Record>

    ```nextflow
        ch_masked = ch_input
        ^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/genome_masking/main.nf:87:40`: Unrecognized method `keySet` for type Record {
    id: String
    taxid_lineage: Integer
    fasta: Path
    softmasked: Path
}

    ```nextflow
                            rec.subMap(rec.keySet() - ['softmasked'])
                                           ^^^^^^
    ```

- Error: `subworkflows/local/genome_masking/main.nf:93:25`: Function `mix` (with multiple signatures) was called with incorrect number of arguments and/or incorrect argument types

    ```nextflow
        masked  = ch_masked.mix( ch_cannot_be_masked )
                            ^^^
    ```

- Error: `subworkflows/local/genome_preparation/main.nf:45:95`: Function `collect` expects 1 argument(s) but received 0

    ```nextflow
                                def csv = rec.stats.splitCsv( header: true, sep: '\t', limit: 1 ).collect()
                                                                                                  ^^^^^^^
    ```

- Error: `subworkflows/local/helixer/main.nf:38:26`: Unrecognized property `helixer_lineage` for type Input

    ```nextflow
            .filter { rec -> rec.helixer_lineage == null }
                             ^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/helixer/main.nf:48:58`: Unrecognized property `helixer_lineage` for type Input

    ```nextflow
                                            .filter { rec -> rec.helixer_lineage != null }
                                                             ^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/helixer/main.nf:49:55`: Unrecognized property `helixer_lineage` for type Input

    ```nextflow
                                            .map { rec -> rec.helixer_lineage }
                                                          ^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/helixer/main.nf:61:33`: Join field `helixer_lineage` is not present in left-hand side

    ```nextflow
                                by: 'helixer_lineage'
                                    ^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/helixer/main.nf:72:5`: Assignment target with type Channel<Record {
    id: String
    gff: Path
}> cannot be assigned to value with type Channel<Record {
    id: String
    structural_annotation: Path
}>

    ```nextflow
        ch_helixer_out = ch_helixer_out
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/helixer/main.nf:74:69`: Closure with signature () -> ? is not compatible with expected signature: (E) -> Boolean

    ```nextflow
                    def gff_lines = rec.gff.splitCsv(sep: '\t').findAll { !it[0].startsWith('#') }
                                                                        ^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/infer_strandedness/main.nf:39:9`: Argument with type Record {
    id: String
    reads: List<Path>
} is not compatible with process input of type Record {
    id: String
    reads: Set<Path>
}

    ```nextflow
            ch_input.map { rec -> record(id: rec.read_id, reads: rec.reads) },
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/infer_strandedness/main.nf:40:9`: Argument with type Float is not compatible with process input of type Number

    ```nextflow
            sample_size
            ^^^^^^^^^^^
    ```

- Error: `subworkflows/local/infer_strandedness/main.nf:42:5`: Assignment target with type Channel<Input> cannot be assigned to value with type Channel<Record {
    id: String
    read_id: String
    reads: Set<Path>
    fasta: Path
    reference_gtf: Path?
    index: Path
}>

    ```nextflow
        ch_input = ch_input.join(
        ^
    ```

- Error: `subworkflows/local/infer_strandedness/main.nf:51:32`: Argument with type Input is not compatible with process input of type Record {
    id: String
    reads: Set<Path>
    read_id: String
    index: Path
    strandedness: String?
}

    ```nextflow
        ch_aligned = HISAT2_ALIGN( ch_input )
                                   ^^^^^^^^
    ```

- Error: `subworkflows/local/infer_strandedness/main.nf:70:40`: Argument with type Record {
    id: String
    read_id: String
    reads: List<Path>
    fasta: Path
    reference_gtf: Path?
    index: Path
    bed: Path
} is not compatible with process input of type Record {
    read_id: String
    bed: Path
    bam: Path
}

    ```nextflow
        ch_report = RSEQC_INFEREXPERIMENT( ch_input_with_bed )
                                           ^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/infer_strandedness/main.nf:80:48`: Argument with type Input is not compatible with process input of type Record {
    read_id: String
    bam: Path
}

    ```nextflow
        ch_xs_strandedness = INFER_STRAND_FROM_XS( ch_input_no_gtf )
                                                   ^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/long_read_preparation/main.nf:94:39`: Argument with type Channel<Record {
    id: String
    fasta: Path
    read_id: String
    fastq: Path
}> is not compatible with parameter of type Channel<MappingInput>

    ```nextflow
        ch_mapped = FASTQ_ALIGN_MINIMAP2( ch_reads )
                                          ^^^^^^^^
    ```

- Error: `subworkflows/local/long_read_preparation/main.nf:100:5`: Assignment target with type Channel<Record {
    id: String
    fasta: Path
    read_id: String
    fastq: Path
}> cannot be assigned to value with type Channel<Record {
    id: String
    new_long_reads: List<Record>
}>

    ```nextflow
        ch_reads = ch_reads
        ^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/metaeuk/main.nf:34:9`: Argument with type Channel<Record> is not compatible with parameter of type Channel<Input>

    ```nextflow
            ch_input.map { rec -> rec.subMap(['id', 'training_proteins', 'mmseqs_db']) },
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/metaeuk/main.nf:39:5`: Assignment target with type Channel<Input> cannot be assigned to value with type Channel<Record>

    ```nextflow
        ch_input = ch_input.join( ch_mmseqs_db, by: 'id' )
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/metaeuk/main.nf:46:9`: Argument with type Record {
    id: String
    fasta: Path
    db: String
} is not compatible with process input of type Record {
    id: String
    fasta: Path
    db: Path
}

    ```nextflow
            ch_input.map{ rec -> record(id: rec.id, fasta: rec.fasta, db: rec.mmseqs_db)}
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/mmseqs_db_preparation/main.nf:49:35`: Unrecognized property `mmseqs_db_to_download` for type Input

    ```nextflow
                ch_input.map { rec -> rec.mmseqs_db_to_download }.unique()
                                      ^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/mmseqs_db_preparation/main.nf:52:9`: Assignment target with type Channel<Record {
    id: String
    db: Path
}> cannot be assigned to value with type Channel<Record {
    mmseqs_db_to_download: String
    public_mmseqs_db: Path
}>

    ```nextflow
            ch_downloaded_mmseqs_db = ch_downloaded_mmseqs_db.map{ rec ->
            ^
    ```

- Error: `subworkflows/local/mmseqs_db_preparation/main.nf:56:64`: Join field `mmseqs_db_to_download` is not present in left-hand side

    ```nextflow
            ch_input = ch_input.join( ch_downloaded_mmseqs_db, by: 'mmseqs_db_to_download' )
                                                                   ^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/mmseqs_db_preparation/main.nf:56:64`: Join field `mmseqs_db_to_download` is not present in right-hand side

    ```nextflow
            ch_input = ch_input.join( ch_downloaded_mmseqs_db, by: 'mmseqs_db_to_download' )
                                                                   ^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/mmseqs_db_preparation/main.nf:76:37`: Function `mix` (with multiple signatures) was called with incorrect number of arguments and/or incorrect argument types

    ```nextflow
        ch_input = ch_mmseqs_db_created.mix( ch_leave_me_alone )
                                        ^^^
    ```

- Error: `subworkflows/local/mmseqs_db_preparation/main.nf:83:35`: Unrecognized property `public_mmseqs_db` for type Input

    ```nextflow
            rec + record(mmseqs_dbs: [rec.public_mmseqs_db, rec.custom_mmseqs_db].findAll{ db -> db != null } )
                                      ^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/mmseqs_db_preparation/main.nf:83:57`: Unrecognized property `custom_mmseqs_db` for type Input

    ```nextflow
            rec + record(mmseqs_dbs: [rec.public_mmseqs_db, rec.custom_mmseqs_db].findAll{ db -> db != null } )
                                                            ^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/mmseqs_db_preparation/main.nf:86:56`: Unrecognized property `mmseqs_dbs` for type Input

    ```nextflow
        ch_mmseqs_dbs_to_concat = ch_input.filter { rec -> rec.mmseqs_dbs.size() > 1 }
                                                           ^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/mmseqs_db_preparation/main.nf:87:56`: Unrecognized property `mmseqs_dbs` for type Input

    ```nextflow
        ch_single_mmseqs_db     = ch_input.filter { rec -> rec.mmseqs_dbs.size() == 1 }
                                                           ^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/mmseqs_db_preparation/main.nf:88:56`: Unrecognized property `mmseqs_dbs` for type Input

    ```nextflow
        ch_no_mmseqs_db         = ch_input.filter { rec -> rec.mmseqs_dbs.size() == 0 }
                                                           ^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/mmseqs_db_preparation/main.nf:90:51`: Argument with type Input is not compatible with process input of type Record {
    id: String
    mmseqs_dbs: Set<Path>
}

    ```nextflow
        ch_mmseqs_concatenated_db = MMSEQS_CONCATDBS( ch_mmseqs_dbs_to_concat )
                                                      ^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/mmseqs_db_preparation/main.nf:93:84`: Unrecognized property `mmseqs_dbs` for type Input

    ```nextflow
        ch_single_mmseqs_db = ch_single_mmseqs_db.map { rec -> rec + record(mmseqs_db: rec.mmseqs_dbs[0]) }
                                                                                       ^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/mmseqs_db_preparation/main.nf:97:40`: Function `mix` (with multiple signatures) was called with incorrect number of arguments and/or incorrect argument types

    ```nextflow
        ch_mmseqs_db = ch_concatenated_dbs.mix( ch_single_mmseqs_db )
                                           ^^^
    ```

- Error: `subworkflows/local/omark/main.nf:37:52`: Named param `checkExists` is not defined

    ```nextflow
            ch_omark_db = channel.fromPath( omamer_db, checkExists: true )
                                                       ^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/omark/main.nf:39:9`: Assignment target with type Channel<Path> cannot be assigned to value with type Value<Path>

    ```nextflow
            ch_omark_db = DOWNLOADDB( omamer_db_url )
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/omark/main.nf:46:28`: Process `OMARK_OMAMERSEARCH` was called with multiple channel arguments which can lead to non-deterministic behavior -- make sure that at most one argument is a channel and that all other arguments are dataflow values

    ```nextflow
        ch_omamer_search_out = OMAMERSEARCH(
                               ^
    ```

- Error: `subworkflows/local/omark/main.nf:61:5`: Cannot assign the result of a call that does not return a value

    ```nextflow
        ch_omark_out = RUN_OMARK( 
        ^
    ```

- Error: `subworkflows/local/omark/main.nf:61:20`: Process `OMARK_OMARK` was called with multiple channel arguments which can lead to non-deterministic behavior -- make sure that at most one argument is a channel and that all other arguments are dataflow values

    ```nextflow
        ch_omark_out = RUN_OMARK( 
                       ^
    ```

- Error: `subworkflows/local/omark/main.nf:62:79`: Unrecognized property `omamer` for type Input

    ```nextflow
            ch_input.map { rec -> record(id: rec.id, fasta: rec.proteome, omamer: rec.omamer, transcript_isoforms: rec.transcript_isoforms) },
                                                                                  ^^^^^^^^^^
    ```

- Error: `subworkflows/local/omark/main.nf:62:112`: Unrecognized property `transcript_isoforms` for type Input

    ```nextflow
            ch_input.map { rec -> record(id: rec.id, fasta: rec.proteome, omamer: rec.omamer, transcript_isoforms: rec.transcript_isoforms) },
                                                                                                                   ^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/post_process_annotation/main.nf:46:9`: Assignment target with type Channel<Input> cannot be assigned to value with type Channel<Record>

    ```nextflow
            ch_input = ch_input.join( ch_complemented, by: 'id' )
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/post_process_annotation/main.nf:76:9`: Assignment target with type Channel<Input> cannot be assigned to value with type Channel<Record>

    ```nextflow
            ch_input = ch_input.join( ch_alternative_annotations, by: 'id' )
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:62:13`: Argument with type Channel<Input> is not compatible with parameter of type Channel<Input>

    ```nextflow
                ch_input,
                ^^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:69:9`: Assignment target with type Channel<Input> cannot be assigned to value with type Channel<Record>

    ```nextflow
            ch_input = ch_input.join( ch_sra_ids, by: 'id', remainder: true )
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:81:79`: Unrecognized property `fetched_short_read_sra_ids` for type Input

    ```nextflow
                            short_read_sra_ids: rec.supplied_short_read_sra_ids + rec.fetched_short_read_sra_ids,
                                                                                  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:82:77`: Unrecognized property `fetched_long_read_sra_ids` for type Input

    ```nextflow
                            long_read_sra_ids: rec.supplied_long_read_sra_ids + rec.fetched_long_read_sra_ids
                                                                                ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:91:9`: Argument with type Channel<Input> is not compatible with parameter of type Channel<ExperimentIDs>

    ```nextflow
            ch_input,
            ^^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:94:5`: Assignment target with type Channel<Input> cannot be assigned to value with type Channel<Record>

    ```nextflow
        ch_input = ch_input.join( ch_downloaded_reads, by: 'id', remainder: true )
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:103:26`: List expression has inconsistent element types -- some elements have type List<Read> while others have type ?

    ```nextflow
                short_reads: [rec.supplied_short_reads, rec.downloaded_short_reads].flatten().findAll(),
                             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:103:53`: Unrecognized property `downloaded_short_reads` for type Input

    ```nextflow
                short_reads: [rec.supplied_short_reads, rec.downloaded_short_reads].flatten().findAll(),
                                                        ^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:103:81`: Unrecognized method `flatten` for type List<?>

    ```nextflow
                short_reads: [rec.supplied_short_reads, rec.downloaded_short_reads].flatten().findAll(),
                                                                                    ^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:104:25`: List expression has inconsistent element types -- some elements have type List<Read> while others have type ?

    ```nextflow
                long_reads: [rec.supplied_long_reads, rec.downloaded_long_reads].flatten().findAll()
                            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:104:51`: Unrecognized property `downloaded_long_reads` for type Input

    ```nextflow
                long_reads: [rec.supplied_long_reads, rec.downloaded_long_reads].flatten().findAll()
                                                      ^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:104:78`: Unrecognized method `flatten` for type List<?>

    ```nextflow
                long_reads: [rec.supplied_long_reads, rec.downloaded_long_reads].flatten().findAll()
                                                                                 ^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:113:33`: Unrecognized property `short_reads` for type Input

    ```nextflow
            ch_input.filter{ rec -> rec.short_reads.size() > 0 }, // pass only samples for which there are short reads
                                    ^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:128:9`: Argument with type Channel<Input> is not compatible with parameter of type Channel<Input>

    ```nextflow
            ch_input.filter{ rec -> rec.long_reads.size() > 0 }, // pass only samples for which there are long reads
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:128:33`: Unrecognized property `long_reads` for type Input

    ```nextflow
            ch_input.filter{ rec -> rec.long_reads.size() > 0 }, // pass only samples for which there are long reads
                                    ^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:171:17`: Unrecognized property `id` for type Record {
    short_read_bams: ?
    long_read_bams: ?
}

    ```nextflow
                id: rec.id, 
                    ^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:172:20`: Unrecognized property `fasta` for type Record {
    short_read_bams: ?
    long_read_bams: ?
}

    ```nextflow
                fasta: rec.fasta,
                       ^^^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:181:5`: Assignment target with type Channel<Input> cannot be assigned to value with type Channel<Record {
    short_read_mappings: ?
    long_read_mappings: ?
}>

    ```nextflow
        ch_input = ch_input
        ^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:185:131`: Unrecognized method `keySet` for type Record {
    bam: Path
    bai: Path
    type: String
}

    ```nextflow
                        def short_read_mappings = rec.mappings.collect{ subrec -> subrec.type == 'short_reads' ? subrec.subMap(subrec.keySet() - ['type']) : null }.findAll()
                                                                                                                                      ^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:185:161`: Function `findAll` expects 1 argument(s) but received 0

    ```nextflow
                        def short_read_mappings = rec.mappings.collect{ subrec -> subrec.type == 'short_reads' ? subrec.subMap(subrec.keySet() - ['type']) : null }.findAll()
                                                                                                                                                                    ^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:186:129`: Unrecognized method `keySet` for type Record {
    bam: Path
    bai: Path
    type: String
}

    ```nextflow
                        def long_read_mappings = rec.mappings.collect{ subrec -> subrec.type == 'long_reads' ? subrec.subMap(subrec.keySet() - ['type']) : null }.findAll()
                                                                                                                                    ^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:186:159`: Function `findAll` expects 1 argument(s) but received 0

    ```nextflow
                        def long_read_mappings = rec.mappings.collect{ subrec -> subrec.type == 'long_reads' ? subrec.subMap(subrec.keySet() - ['type']) : null }.findAll()
                                                                                                                                                                  ^^^^^^^
    ```

- Error: `subworkflows/local/prepare_rnaseq_data/main.nf:188:36`: Unrecognized method `keySet` for type Record {
    id: String
    supplied_short_reads: List<Read>
    supplied_long_reads: List<Read>
    supplied_short_read_bams: List<Path>
    supplied_long_read_bams: List<Path>
    supplied_short_read_sra_ids: List<String>
    supplied_long_read_sra_ids: List<String>
    fasta: Path
    reference_gff: Path
    bams: Set<Bam>
    mappings: Bag<Record {
    bam: Path
    bai: Path
    type: String
}>
}

    ```nextflow
                        rec.subMap(rec.keySet() - ['mappings']) + record(
                                       ^^^^^^
    ```

- Error: `subworkflows/local/quality_controls/main.nf:41:16`: Argument with type Channel<Input> is not compatible with parameter of type Channel<Input>

    ```nextflow
            BUSCO( ch_input )
                   ^^^^^^^^
    ```

- Error: `subworkflows/local/quality_controls/main.nf:53:13`: Argument with type Boolean is not compatible with parameter of type String

    ```nextflow
                omamer_db_url,
                ^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/quality_controls/main.nf:54:13`: Argument with type Boolean is not compatible with parameter of type String

    ```nextflow
                omamer_db
                ^^^^^^^^^
    ```

- Error: `subworkflows/local/reporting/main.nf:35:38`: Closure with signature (?, ?, ?) -> ? is not compatible with expected signature: (E) -> R

    ```nextflow
                                    .map { process, tool, version ->
                                         ^
    ```

- Error: `subworkflows/local/reporting/main.nf:68:32`: Conditional expression has inconsistent types -- true branch has type Channel<Path> but false branch has type Channel<List<E>>

    ```nextflow
        ch_multiqc_logo          = multiqc_logo ?
                                   ^
    ```

- Error: `subworkflows/local/reporting/main.nf:78:25`: Unrecognized method `collectFile` for type Value<?>

    ```nextflow
        ch_workflow_summary.collectFile(name: 'workflow_summary_mqc.yaml')
                            ^^^^^^^^^^^
    ```

- Error: `subworkflows/local/reporting/main.nf:103:73`: Function `flatMap` (with multiple signatures) was called with incorrect number of arguments and/or incorrect argument types

    ```nextflow
                            .mix( channel.topic('agat_functs_tats_multiqc').flatMap{ id, files -> files.collect{ file -> [id, file] } } )
                                                                            ^^^^^^^
    ```

- Error: `subworkflows/local/reporting/main.nf:110:56`: Unrecognized method `collectFile` for type Value<?>

    ```nextflow
                                    ch_methods_description.collectFile(
                                                           ^^^^^^^^^^^
    ```

- Error: `subworkflows/local/reporting/main.nf:120:33`: List expression has inconsistent element types -- some elements have type Map<String, ?> while others have type ?

    ```nextflow
                                    [ meta, data_files.flatten().toSorted() ] 
                                    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/reporting/main.nf:133:29`: List expression has inconsistent element types -- some elements have type ? while others have type List<Path>

    ```nextflow
                                [meta, data_files, configs, logo, [], []] 
                                ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/short_read_preparation/main.nf:155:5`: Assignment target with type Channel<Record {
    id: String
    read_id: String
    reads: List<Path>
    fasta: Path
    reference_gtf: Path
    bam: Path
}> cannot be assigned to value with type Channel<Record {
    id: String
    new_short_read_bams: List<Record>
}>

    ```nextflow
        ch_mapped = ch_mapped
        ^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/structural_annotation/main.nf:43:33`: Argument with type Channel<Input> is not compatible with parameter of type Channel<Input>

    ```nextflow
            ch_annotated = BRAKER3( ch_input )
                                    ^^^^^^^^
    ```

- Error: `subworkflows/local/structural_annotation/main.nf:52:13`: Argument with type Channel<Input> is not compatible with parameter of type Channel<Input>

    ```nextflow
                ch_input,
                ^^^^^^^^
    ```

- Error: `subworkflows/local/training_protein_preparation/main.nf:46:36`: Function `fromPath` (with multiple signatures) was called with incorrect number of arguments and/or incorrect argument types

    ```nextflow
            ch_orthodb_local = channel.fromPath( orthodb_local, checkExists: true )
                                       ^^^^^^^^
    ```

- Error: `subworkflows/local/training_protein_preparation/main.nf:49:9`: Assignment target with type Channel<Input> cannot be assigned to value with type Channel<Tuple<Input, ?>>

    ```nextflow
            ch_input = ch_input.combine( ch_orthodb_local )
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/training_protein_preparation/main.nf:56:17`: Argument with type Record is not compatible with process input of type Record {
    species: String
    taxid_lineage: String
}

    ```nextflow
                    ch_input.map { rec -> rec.subMap(['species', 'taxid_lineage']) }.unique()
                    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/training_protein_preparation/main.nf:58:63`: Join field `species` is not present in left-hand side

    ```nextflow
                ch_input = ch_input.join(ch_prepared_orthodb, by: 'species')
                                                                  ^^^^^^^^^
    ```

- Error: `subworkflows/local/training_protein_preparation/main.nf:67:32`: Unrecognized property `orthodb_proteins` for type Input

    ```nextflow
            def orthodb_proteins = rec.orthodb_proteins ? [rec.orthodb_proteins] : []
                                   ^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/training_protein_preparation/main.nf:67:56`: Unrecognized property `orthodb_proteins` for type Input

    ```nextflow
            def orthodb_proteins = rec.orthodb_proteins ? [rec.orthodb_proteins] : []
                                                           ^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/training_protein_preparation/main.nf:75:53`: Unrecognized property `all_training_proteins` for type Input

    ```nextflow
        ch_proteins_to_concat = ch_input.filter{ rec -> rec.all_training_proteins.size() > 1 }
                                                        ^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/training_protein_preparation/main.nf:76:53`: Unrecognized property `all_training_proteins` for type Input

    ```nextflow
        ch_single_protein_db  = ch_input.filter{ rec -> rec.all_training_proteins.size() == 1 }
                                                        ^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/training_protein_preparation/main.nf:77:53`: Unrecognized property `all_training_proteins` for type Input

    ```nextflow
        ch_no_protein_db      = ch_input.filter{ rec -> rec.all_training_proteins.size() == 0 }
                                                        ^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/training_protein_preparation/main.nf:80:76`: Unrecognized property `all_training_proteins` for type Input

    ```nextflow
            ch_proteins_to_concat.map { rec -> record(id: rec.id, fasta_files: rec.all_training_proteins) }
                                                                               ^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/training_protein_preparation/main.nf:83:82`: Unrecognized property `all_training_proteins` for type Input

    ```nextflow
        ch_single_protein_db = ch_single_protein_db.map { rec -> rec + record(fasta: rec.all_training_proteins[0]) }
                                                                                     ^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/training_protein_preparation/main.nf:92:30`: Function `mix` (with multiple signatures) was called with incorrect number of arguments and/or incorrect argument types

    ```nextflow
            ch_single_protein_db.mix( ch_concatenated_proteins ),
                                 ^^^
    ```

- Error: `subworkflows/local/training_protein_preparation/main.nf:96:5`: Assignment target with type Channel<Record {
    id: String
    fasta: Path
}> cannot be assigned to value with type Channel<Record {
    id: String
    proteins_fasta: Path
}>

    ```nextflow
        ch_proteins = ch_proteins.map { rec -> record(id: rec.id, proteins_fasta: rec.fasta) }
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:277:30`: Unrecognized method `toMap` for namespace `workflow`

    ```nextflow
        meta.workflow = workflow.toMap()
                                 ^^^^^
    ```

- Error: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:278:46`: Unrecognized method `toMap` for namespace `workflow.manifest`

    ```nextflow
        meta["manifest_map"] = workflow.manifest.toMap()
                                                 ^^^^^
    ```

- Error: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:308:29`: Unrecognized method `toString` for type Writable

    ```nextflow
        return description_html.toString()
                                ^^^^^^^^
    ```

- Error: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:317:24`: Legacy type annotations are not supported with static typing -- use `name: Type` instead

    ```nextflow
    def removeKeyValueArgs(Map opts){
                           ^^^^^^^^
    ```

- Error: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:343:12`: Legacy type annotations are not supported with static typing -- use `name: Type` instead

    ```nextflow
    def sha256(Map map) {
               ^^^^^^^
    ```

- Error: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:355:27`: Unrecognized method `getBytes` for type String

    ```nextflow
        return md.digest(json.getBytes('UTF-8'))
                              ^^^^^^^^
    ```

- Error: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:356:14`: Unrecognized method `collect` for type byte

    ```nextflow
                .collect { String.format('%02x', it) }
                 ^^^^^^^
    ```

- Error: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:368:48`: Unrecognized method `findResults` for type List<Tuple>

    ```nextflow
        def config_paths_list = tokens.withIndex().findResults { token, i ->
                                                   ^^^^^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:68:13`: Argument with type Channel<Samplesheet> is not compatible with parameter of type Channel<Genome>

    ```nextflow
                ch_main,
                ^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:72:9`: Assignment target with type Channel<Samplesheet> cannot be assigned to value with type Channel<Record>

    ```nextflow
            ch_main = ch_main.join( ch_masked, by: 'id' )
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:82:13`: Argument with type Channel<Samplesheet> is not compatible with parameter of type Channel<Input>

    ```nextflow
                ch_main,
                ^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:97:9`: Assignment target with type Channel<Samplesheet> cannot be assigned to value with type Channel<Record>

    ```nextflow
            ch_main = ch_main.join( ch_prepared_rnaseq_data, by: 'id', remainder: true )
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:108:13`: Argument with type Channel<Samplesheet> is not compatible with parameter of type Channel<Input>

    ```nextflow
                ch_main,
                ^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:114:9`: Assignment target with type Channel<Samplesheet> cannot be assigned to value with type Channel<Record>

    ```nextflow
            ch_main = ch_main.join( ch_proteins, by: 'id', remainder: true )
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:125:13`: Argument with type Channel<Samplesheet> is not compatible with parameter of type Channel<Input>

    ```nextflow
                ch_main,
                ^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:133:9`: Assignment target with type Channel<Samplesheet> cannot be assigned to value with type Channel<Record>

    ```nextflow
            ch_main = ch_main.join( ch_structural_annotation, by: 'id' )
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:137:76`: Unrecognized property `reference_gff` for type Samplesheet

    ```nextflow
            ch_main = ch_main.map { rec -> rec + record(structural_annotation: rec.reference_gff) }
                                                                               ^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:148:9`: Argument with type Channel<Samplesheet> is not compatible with parameter of type Channel<Input>

    ```nextflow
            ch_main.filter { rec -> rec.structural_annotation != null },
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:148:33`: Unrecognized property `structural_annotation` for type Samplesheet

    ```nextflow
            ch_main.filter { rec -> rec.structural_annotation != null },
                                    ^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:157:5`: Assignment target with type Channel<Samplesheet> cannot be assigned to value with type Channel<Record>

    ```nextflow
        ch_main = ch_main.join( ch_post_processed_annotation, by: 'id', remainder: true )
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:169:13`: Argument with type Channel<Samplesheet> is not compatible with parameter of type Channel<Input>

    ```nextflow
                ch_main.filter { rec -> rec.gff != null }
                ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:171:9`: Assignment target with type Channel<Samplesheet> cannot be assigned to value with type Channel<Record>

    ```nextflow
            ch_main = ch_main.join( ch_extracted_sequences, by: 'id' )
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:185:13`: Argument with type Channel<Samplesheet> is not compatible with parameter of type Channel<Input>

    ```nextflow
                ch_main.filter { rec -> rec.proteome != null },
                ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:185:37`: Unrecognized property `proteome` for type Samplesheet

    ```nextflow
                ch_main.filter { rec -> rec.proteome != null },
                                        ^^^^^^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:192:9`: Assignment target with type Channel<Samplesheet> cannot be assigned to value with type Channel<Record>

    ```nextflow
            ch_main = ch_main.join( ch_functional_annotation, by: 'id' )
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:203:13`: Argument with type Channel<Samplesheet> is not compatible with parameter of type Channel<Input>

    ```nextflow
                ch_main,
                ^^^^^^^
    ```

- Error: `workflows/genomeannotator.nf:223:5`: Assignment target with type Channel<Samplesheet> cannot be assigned to value with type Channel<Record>

    ```nextflow
        ch_main = ch_main.join( ch_reporting, by: 'id' )
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```


## :warning: Warnings

- Warning: `main.nf:36:5`: Typed workflow input should have a type annotation

    ```nextflow
        samplesheet // channel: samplesheet read in from --input
        ^^^^^^^^^^^
    ```

- Warning: `main.nf:68:5`: Variable was declared but not used

    ```nextflow
        ch_samplesheet = PIPELINE_INITIALISATION (
        ^^^^^^^^^^^^^^
    ```

- Warning: `modules/local/agat/spmergeannotations/main.nf:19:9`: Variable was declared but not used

    ```nextflow
        def args         = task.ext.args   ?: ''
            ^^^^
    ```

- Warning: `modules/local/interproscan5/download_db/main.nf:8:5`: Closure is no longer required for dynamic process directives

    ```nextflow
        errorStrategy {
        ^^^^^^^^^^^^^
    ```

- Warning: `modules/local/interproscan6/main.nf:76:23`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            .findAll { k, v -> !(k.startsWith('NXF') || k.startsWith('TOWER')) || k in nxf_passthrough }
                          ^
    ```

- Warning: `modules/local/interproscan6/main.nf:86:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        def valid_profiles = workflow.profile.tokenize(',').findAll { !it.startsWith('test_') }
                                                                       ^^
    ```

- Warning: `modules/local/red/main.nf:23:9`: Variable was declared but not used

    ```nextflow
        def args    = task.ext.args ?: ''
            ^^^^
    ```

- Warning: `modules/local/red/main.nf:24:9`: Variable was declared but not used

    ```nextflow
        def prefix  = task.ext.prefix ?: "${id}"
            ^^^^^^
    ```

- Warning: `modules/local/repeatmodeler/repeatmodeler/main.nf:7:5`: Closure is no longer required for dynamic process directives

    ```nextflow
        errorStrategy {
        ^^^^^^^^^^^^^
    ```

- Warning: `modules/local/seqtk/sample/main.nf:31:9`: Variable was declared but not used

    ```nextflow
        def prefix = task.ext.prefix ?: "$id"
            ^^^^^^
    ```

- Warning: `modules/local/star/genomegenerate/main.nf:31:9`: Variable was declared but not used

    ```nextflow
        def args_list   = args.tokenize()
            ^^^^^^^^^
    ```

- Warning: `modules/local/tiberius/tiberius/main.nf:27:9`: Variable was declared but not used

    ```nextflow
        def args = task.ext.args ?: ''
            ^^^^
    ```

- Warning: `modules/local/tsebra/tsebra/main.nf:34:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        def gtf_arg     = '-g ' + gtfs.collect { "$it" }.join(',')
                                                  ^^
    ```

- Warning: `modules/local/tsebra/tsebra/main.nf:35:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        def hints_arg   = '-e ' + hintsfiles.collect { "$it" }.join(',')
                                                        ^^
    ```

- Warning: `modules/nf-core/custom/sratoolsncbisettings/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

    ```nextflow
        when:
        ^^^^
    ```

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

    ```nextflow
        when:
        ^^^^
    ```

- Warning: `subworkflows/local/alternative_annotation/main.nf:15:5`: Typed workflow input should have a type annotation

    ```nextflow
        ch_input
        ^^^^^^^^
    ```

- Warning: `subworkflows/local/bam_sort_index_stats/main.nf:69:54`: Join fields [id, bai] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
        ch_bam_bai = ch_bam.join( ch_sorted_bam_bai, by: 'read_id' )
                                                         ^^^^^^^^^
    ```

- Warning: `subworkflows/local/braker3/main.nf:91:5`: Variable was declared but not used

    ```nextflow
        ch_no_long_read_mappings = ch_input.filter{ rec -> rec.long_read_mappings.size() == 0 }
        ^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/braker3/main.nf:134:53`: Join fields [braker_gtf, braker_hintsfile] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
                        .join(ch_isoseq_braker_out, by: 'id', remainder: true)
                                                        ^^^^
    ```

- Warning: `subworkflows/local/complement_annotation/main.nf:56:13`: Join fields [structural_annotation] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
            by: 'id' 
                ^^^^
    ```

- Warning: `subworkflows/local/deinterleave/main.nf:42:81`: Join fields [reads] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
        ch_deinterleaved = ch_interleaved_reads.join(ch_bbmap_deinterleave_out, by: 'read_id')
                                                                                    ^^^^^^^^^
    ```

- Warning: `subworkflows/local/download_reads/main.nf:61:79`: Join fields [reads] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
            ch_downloaded_reads = ch_downloaded_reads.join( ch_sampled_reads, by: 'id' )
                                                                                  ^^^^
    ```

- Warning: `subworkflows/local/extract_sequences/main.nf:54:30`: Operator `groupTuple` is discouraged from use with static typing

    ```nextflow
                                .groupTuple()
                                 ^^^^^^^^^^
    ```

- Warning: `subworkflows/local/fastq_align_hisat2/main.nf:87:44`: Join fields [id] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
        mapped = ch_input.join(ch_aligned, by: 'read_id')
                                               ^^^^^^^^^
    ```

- Warning: `subworkflows/local/fastq_align_minimap2/main.nf:44:44`: Join fields [id] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
        mapped = ch_input.join(ch_aligned, by: 'read_id')
                                               ^^^^^^^^^
    ```

- Warning: `subworkflows/local/fastq_align_star/main.nf:40:44`: Join fields [id] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
        mapped = ch_input.join(ch_aligned, by: 'read_id')
                                               ^^^^^^^^^
    ```

- Warning: `subworkflows/local/functional_annotation/main.nf:58:61`: Join fields [gff] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
            ch_input = ch_input.join( ch_eggnog_mapper_out, by: 'id' )
                                                                ^^^^
    ```

- Warning: `subworkflows/local/functional_annotation/main.nf:115:60`: Join fields [gff] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
                ch_input = ch_input.join( ch_complemented, by: 'id' )
                                                               ^^^^
    ```

- Warning: `subworkflows/local/genome_preparation/main.nf:33:56`: Join fields [fasta] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
        ch_prepared = ch_input.join(ch_checked_genome, by: 'id')
                                                           ^^^^
    ```

- Warning: `subworkflows/local/helixer/main.nf:74:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
                    def gff_lines = rec.gff.splitCsv(sep: '\t').findAll { !it[0].startsWith('#') }
                                                                           ^^
    ```

- Warning: `subworkflows/local/infer_strandedness/main.nf:44:13`: Join fields [reads] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
            by: 'read_id'
                ^^^^^^^^^
    ```

- Warning: `subworkflows/local/infer_strandedness/main.nf:53:47`: Join fields [id] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
        ch_input = ch_input.join( ch_aligned, by: 'read_id' )
                                                  ^^^^^^^^^
    ```

- Warning: `subworkflows/local/long_read_preparation/main.nf:80:56`: Join fields [id, fastq] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
            ch_reads = ch_reads.join(ch_cleaned_reads, by: 'read_id')
                                                           ^^^^^^^^^
    ```

- Warning: `subworkflows/local/mmseqs_db_preparation/main.nf:32:5`: Typed workflow input should have a type annotation

    ```nextflow
        mmseqs_db
        ^^^^^^^^^
    ```

- Warning: `subworkflows/local/mmseqs_db_preparation/main.nf:33:5`: Typed workflow input should have a type annotation

    ```nextflow
        skip_mmseqs_db_download
        ^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/mmseqs_db_preparation/main.nf:92:88`: Join fields [mmseqs_db] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
        ch_concatenated_dbs = ch_mmseqs_dbs_to_concat.join( ch_mmseqs_concatenated_db, by: 'id' )
                                                                                           ^^^^
    ```

- Warning: `subworkflows/local/omark/main.nf:61:5`: Variable was declared but not used

    ```nextflow
        ch_omark_out = RUN_OMARK( 
        ^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/post_process_annotation/main.nf:64:51`: Join fields [structural_annotation, reference_gff, fasta] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
            ch_input = ch_input.join( ch_cleaned, by: 'id' )
                                                      ^^^^
    ```

- Warning: `subworkflows/local/prepare_rnaseq_data/main.nf:38:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        skip_fastqc: Boolean
        ^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/prepare_rnaseq_data/main.nf:39:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        skip_fastqc_raw: Boolean
        ^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/prepare_rnaseq_data/main.nf:40:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        skip_fastqc_cleaned: Boolean
        ^^^^^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/prepare_rnaseq_data/main.nf:41:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        skip_umi_extract: Boolean
        ^^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/prepare_rnaseq_data/main.nf:42:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        skip_short_read_cleaning: Boolean
        ^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/prepare_rnaseq_data/main.nf:49:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        short_read_mapper: String
        ^^^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/prepare_rnaseq_data/main.nf:50:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        ignore_existing_gff_for_mapping: Boolean
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/prepare_rnaseq_data/main.nf:182:47`: Join fields [fasta] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
                    .join( ch_sorted_indexed, by: 'id')
                                                  ^^^^
    ```

- Warning: `subworkflows/local/reporting/main.nf:20:5`: Typed workflow input should have a type annotation

    ```nextflow
        multiqc_config
        ^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/reporting/main.nf:21:5`: Typed workflow input should have a type annotation

    ```nextflow
        multiqc_logo
        ^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/reporting/main.nf:22:5`: Typed workflow input should have a type annotation

    ```nextflow
        multiqc_methods_description
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/reporting/main.nf:23:5`: Typed workflow input should have a type annotation

    ```nextflow
        outdir
        ^^^^^^
    ```

- Warning: `subworkflows/local/reporting/main.nf:107:30`: Operator `groupTuple` is discouraged from use with static typing

    ```nextflow
                                .groupTuple()
                                 ^^^^^^^^^^
    ```

- Warning: `subworkflows/local/short_read_preparation/main.nf:33:5`: Typed workflow input should have a type annotation

    ```nextflow
        ch_input
        ^^^^^^^^
    ```

- Warning: `subworkflows/local/training_protein_preparation/main.nf:34:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        orthodb_version: String
        ^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:31:5`: Typed workflow input should have a type annotation

    ```nextflow
        version           // boolean: Display version and exit
        ^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:32:5`: Typed workflow input should have a type annotation

    ```nextflow
        validate_params   // boolean: Boolean whether to validate parameters against the schema at runtime
        ^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:33:5`: Typed workflow input should have a type annotation

    ```nextflow
        monochrome_logs   // boolean: Do not use coloured log outputs
        ^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:34:5`: Typed workflow input should have a type annotation

    ```nextflow
        nextflow_cli_args //   array: List of positional nextflow CLI args
        ^^^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:35:5`: Typed workflow input should have a type annotation

    ```nextflow
        outdir            //  string: The output directory where the results will be saved
        ^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:36:5`: Typed workflow input should have a type annotation

    ```nextflow
        input             //  string: Path to input samplesheet
        ^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:36:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        input             //  string: Path to input samplesheet
        ^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:37:5`: Typed workflow input should have a type annotation

    ```nextflow
        help              // boolean: Display help message and exit
        ^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:38:5`: Typed workflow input should have a type annotation

    ```nextflow
        help_full         // boolean: Show the full help message
        ^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:39:5`: Typed workflow input should have a type annotation

    ```nextflow
        show_hidden       // boolean: Show hidden parameters in the help message
        ^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:127:5`: Typed workflow input should have a type annotation

    ```nextflow
        email           //  string: email address
        ^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:128:5`: Typed workflow input should have a type annotation

    ```nextflow
        email_on_fail   //  string: email address sent on pipeline failure
        ^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:129:5`: Typed workflow input should have a type annotation

    ```nextflow
        plaintext_email // boolean: Send plain-text email instead of HTML
        ^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:130:5`: Typed workflow input should have a type annotation

    ```nextflow
        outdir          //    path: Path to output directory where results will be published
        ^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:131:5`: Typed workflow input should have a type annotation

    ```nextflow
        monochrome_logs // boolean: Disable ANSI colour codes in log output
        ^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:132:5`: Typed workflow input should have a type annotation

    ```nextflow
        multiqc_report  //  string: Path to MultiQC report
        ^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeannotator_pipeline/main.nf:356:46`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
                .collect { String.format('%02x', it) }
                                                 ^^
    ```

- Warning: `workflows/genomeannotation.nf:21:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        ch_samplesheet // channel: samplesheet read in from --input
        ^^^^^^^^^^^^^^
    ```

- Warning: `workflows/genomeannotator.nf:60:46`: Join fields [fasta, species] are present in both records -- the left-hand values will be overwritten by the right-hand values

    ```nextflow
        ch_main = ch_main.join( ch_prepared, by: 'id' )
                                                 ^^^^
    ```

- Warning: `workflows/genomeannotator.nf:202:9`: Variable was declared but not used

    ```nextflow
            ch_qc = QUALITY_CONTROLS(
            ^^^^^
    ```
