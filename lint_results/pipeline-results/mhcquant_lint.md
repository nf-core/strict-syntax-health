# Nextflow lint results

- Generated: 2026-10-24T00:21:05.743733668Z
- Nextflow version: 26.10.3
- Summary: 82 warnings

## :warning: Warnings

- Warning: `conf/modules.config:109:106`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              "-fixed_modifications ${meta.fixed_mods.trim() ? meta.fixed_mods.tokenize(',').collect { "'${it.trim()}'" }.join(' ') : ''}",
                                                                                                           ^^
  ```

- Warning: `conf/modules.config:110:115`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              meta.variable_mods.trim() ? "-variable_modifications ${meta.variable_mods.tokenize(',').collect { "'${it.trim()}'" }.join(' ')}" : "",
                                                                                                                    ^^
  ```

- Warning: `modules/local/epicore/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/ms2rescore/main.nf:22:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/openms/idmassaccuracy/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/openms/idmassaccuracy/main.nf:35:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/openmsthirdparty/featurelinkerunlabeledkd/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/openmsthirdparty/percolatoradapter/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms/chromatogramextractor/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms/chromatogramextractor/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args  ?: ''
          ^^^^
  ```

- Warning: `modules/local/pyopenms/ionannotator/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/pyopenms/ionannotator/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/untar/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/local/unzip/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/easypqp/convert/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/easypqp/library/main.nf:18:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/multiqc/main.nf:20:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/decoydatabase/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/featurefinderidentification/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/fileconverter/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/filefilter/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/idconflictresolver/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/idfilter/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/idmerger/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/idripper/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/idscoreswitcher/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/mapaligneridentification/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/maprttransformer/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/mztabexporter/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/peakpickerhires/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/peptideindexer/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/psmfeatureextractor/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openms/textexporter/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/openmsthirdparty/cometadapter/main.nf:19:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/parsesdrf/convert/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pridepy/downloadfile/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/pridepy/fetchsdrf/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `modules/nf-core/thermorawfileparser/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:22:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .flatMap { group_meta, trafoxmls -> [trafoxmls].flatten().collect { trafoxml -> [[spectra: trafoxml.baseName.replace("_fdr_filtered", "")], trafoxml] } }
                         ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:27:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .flatMap { group_meta, idxmls -> [idxmls].flatten().collect { idxml -> [[spectra: idxml.baseName.replace("_fdr_filtered","")], idxml] } }
                         ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:29:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .flatMap { group_meta, metas -> metas }
                                 ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:34:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { spectra, idxml, meta, mzml, trafoxml -> [meta, idxml, mzml, trafoxml] }
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:35:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { meta, idxml, mzml, trafoxml ->
                        ^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:35:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { meta, idxml, mzml, trafoxml ->
                              ^^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:35:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .branch { meta, idxml, mzml, trafoxml ->
                                     ^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:43:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, idxml, mzml, trafoxml -> [id: "${meta.sample}_${meta.condition}"] }
                           ^^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:43:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, idxml, mzml, trafoxml -> [id: "${meta.sample}_${meta.condition}"] }
                                  ^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:43:39`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, idxml, mzml, trafoxml -> [id: "${meta.sample}_${meta.condition}"] }
                                        ^^^^^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:52:78`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          OPENMS_MAPRTTRANSFORMERMZML(ch_runs_by_alignment.aligned.map { meta, idxml, mzml, trafoxml -> [meta, mzml, trafoxml] })
                                                                               ^^^^^
  ```

- Warning: `subworkflows/local/map_alignment/main.nf:53:86`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          OPENMS_MAPRTTRANSFORMERIDXML(ch_runs_by_alignment.aligned.map { meta, idxml, mzml, trafoxml -> [meta, idxml, trafoxml] })
                                                                                       ^^^^
  ```

- Warning: `subworkflows/local/process_feature/main.nf:27:61`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .map { key, featurexmls -> [key, featurexmls.sort { it.name.tokenize('_')[0] as int }] }
                                                              ^^
  ```

- Warning: `subworkflows/local/quant/main.nf:30:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .flatMap { group_meta, idxmls -> [idxmls].flatten().collect { idxml -> [[spectra: idxml.baseName], idxml] } }
                         ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/quant/main.nf:33:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                      .flatMap { group_meta, metas -> metas }
                                 ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/quant/main.nf:35:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { spectra, idxmls, meta -> [meta, idxmls] }
                     ^^^^^^^
  ```

- Warning: `subworkflows/local/quant/main.nf:51:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { group_meta, meta, idxml, q_value -> [meta, idxml, q_value] }
                     ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/quant/main.nf:79:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map { group_meta, meta, aligned_mzml, idxml, merged_idxml -> [meta, aligned_mzml, idxml, merged_idxml] }
                         ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/rescore/main.nf:56:73`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def extra = feature_names.readLines().drop(1).findAll { it.contains('\t') }.collect { it.split('\t', -1) }.findAll { !it[0].contains('psm_file') }.collect { it[1] }
                                                                          ^^
  ```

- Warning: `subworkflows/local/rescore/main.nf:56:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def extra = feature_names.readLines().drop(1).findAll { it.contains('\t') }.collect { it.split('\t', -1) }.findAll { !it[0].contains('psm_file') }.collect { it[1] }
                                                                                                        ^^
  ```

- Warning: `subworkflows/local/rescore/main.nf:56:135`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def extra = feature_names.readLines().drop(1).findAll { it.contains('\t') }.collect { it.split('\t', -1) }.findAll { !it[0].contains('psm_file') }.collect { it[1] }
                                                                                                                                        ^^
  ```

- Warning: `subworkflows/local/rescore/main.nf:56:174`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def extra = feature_names.readLines().drop(1).findAll { it.contains('\t') }.collect { it.split('\t', -1) }.findAll { !it[0].contains('psm_file') }.collect { it[1] }
                                                                                                                                                                               ^^
  ```

- Warning: `subworkflows/local/rescore/main.nf:65:100`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_multiqc_files = ch_multiqc_files.mix(OPENMS_PERCOLATORADAPTER.out.feature_weights.map { meta, feature_weights -> feature_weights })
                                                                                                     ^^^^
  ```

- Warning: `subworkflows/local/rescore/main.nf:86:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  ).map { preset, group_meta, local_idxml, global_filtered_idxml ->
                          ^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mhcquant_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mhcquant_pipeline/main.nf:163:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { group_meta, metas, files, fastas -> [group_meta, files.size()] }
                             ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mhcquant_pipeline/main.nf:163:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { group_meta, metas, files, fastas -> [group_meta, files.size()] }
                                           ^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mhcquant_pipeline/main.nf:165:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { group_meta, group_count, meta, file, fasta ->
                 ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mhcquant_pipeline/main.nf:173:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, file, fasta, presetsMap ->
                             ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mhcquant_pipeline/main.nf:186:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map{ meta, file, fasta -> fasta }
                    ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mhcquant_pipeline/main.nf:186:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map{ meta, file, fasta -> fasta }
                          ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mhcquant_pipeline/main.nf:198:51`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_fasta = ch_samplesheet_raw.map { meta, file, fasta -> [groupKey([id: "${meta.sample}_${meta.condition}"], meta.group_count), fasta] }
                                                    ^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_mhcquant_pipeline/main.nf:200:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, fasta -> fasta }
                     ^^^^
  ```

- Warning: `workflows/mhcquant.nf:89:89`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(PYOPENMS_CHROMATOGRAMEXTRACTOR.out.csv.map{ meta, mzml -> mzml })
                                                                                          ^^^^
  ```

- Warning: `workflows/mhcquant.nf:93:53`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_clean_mzml_file.combine(ch_decoy_db.map{ meta, fasta -> [fasta] }) :
                                                      ^^^^
  ```

- Warning: `workflows/mhcquant.nf:97:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { groupKey, meta, mzml, fasta -> [meta, mzml, fasta] }
                     ^^^^^^^^
  ```

- Warning: `workflows/mhcquant.nf:104:74`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          OPENMSTHIRDPARTY_COMETADAPTER.out.idxml.combine(ch_decoy_db.map{ meta, fasta -> [fasta] }) :
                                                                           ^^^^
  ```

- Warning: `workflows/mhcquant.nf:108:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { groupKey, meta, idxml, fasta -> [meta, idxml, fasta] }
                     ^^^^^^^^
  ```

- Warning: `workflows/mhcquant.nf:117:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, idxml -> [ groupKey([id: "${meta.sample}_${meta.condition}"], meta.group_count), meta] }
                       ^^^^^
  ```

- Warning: `workflows/mhcquant.nf:134:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { gkey, metas, mzmls, idxml ->
                     ^^^^
  ```

- Warning: `workflows/mhcquant.nf:161:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .map { groupKey, meta, comet_idxml, fdr_filtered_idxml -> [meta, comet_idxml, fdr_filtered_idxml] }
                         ^^^^^^^^
  ```

- Warning: `workflows/mhcquant.nf:246:88`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          params.epicore ? EPICORE.out.stats : SUMMARIZE_RESULTS.out.epicore_input.map { meta, tsv, stats -> stats }
                                                                                         ^^^^
  ```

- Warning: `workflows/mhcquant.nf:246:94`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          params.epicore ? EPICORE.out.stats : SUMMARIZE_RESULTS.out.epicore_input.map { meta, tsv, stats -> stats }
                                                                                               ^^^
  ```
