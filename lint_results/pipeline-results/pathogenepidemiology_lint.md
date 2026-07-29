# Nextflow lint results

- Generated: 2026-07-29T00:29:39.730678460Z
- Nextflow version: 26.07.0-edge
- Summary: 17 errors, 13 warnings

## :x: Errors

- Error: `modules/nf-core/multiqc/main.nf:7:3`: Unexpected input: '<'

    ```nextflow
    <<<<<<< HEAD
      ^
    ```

- Error: `workflows/original_local.nf:16:1`: Invalid include source: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/pathogenepidemiology/workflows/modules/nf-core/fastqc/main.nf'

    ```nextflow
    include { FASTQC } from './modules/nf-core/fastqc/main'
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/original_local.nf:17:1`: Invalid include source: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/pathogenepidemiology/workflows/modules/local/bbduk_custom/main.nf'

    ```nextflow
    include { BBDUK_CUSTOM } from './modules/local/bbduk_custom/main'
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/original_local.nf:18:1`: Invalid include source: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/pathogenepidemiology/workflows/modules/nf-core/minimap2/index/main.nf'

    ```nextflow
    include { MINIMAP2_INDEX } from './modules/nf-core/minimap2/index/main'
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/original_local.nf:19:1`: Invalid include source: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/pathogenepidemiology/workflows/modules/nf-core/minimap2/align/main.nf'

    ```nextflow
    include { MINIMAP2_ALIGN } from './modules/nf-core/minimap2/align/main' 
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/original_local.nf:20:1`: Invalid include source: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/pathogenepidemiology/workflows/modules/nf-core/multiqc/main.nf'

    ```nextflow
    include { MULTIQC } from './modules/nf-core/multiqc/main'
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/original_local.nf:21:1`: Invalid include source: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/pathogenepidemiology/workflows/modules/local/clair3_custom/main.nf'

    ```nextflow
    include { CLAIR3_CUSTOM } from './modules/local/clair3_custom/main'
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/original_local.nf:24:1`: Invalid include source: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/pathogenepidemiology/workflows/modules/nf-core/clair3/main.nf'

    ```nextflow
    include { CLAIR3 } from './modules/nf-core/clair3/main'
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/original_local.nf:53:16`: `FASTQC` is not defined

    ```nextflow
      fastqc_out = FASTQC(ch_reads)
                   ^^^^^^
    ```

- Error: `workflows/original_local.nf:56:20`: `BBDUK_CUSTOM` is not defined

    ```nextflow
      hostrm_prepped = BBDUK_CUSTOM(ch_reads, ch_hostref.first(), ch_adapters.first())
                       ^^^^^^^^^^^^
    ```

- Error: `workflows/original_local.nf:63:20`: `MINIMAP2_INDEX` is not defined

    ```nextflow
      minimap2_index = MINIMAP2_INDEX(ch_reffasta)
                       ^^^^^^^^^^^^^^
    ```

- Error: `workflows/original_local.nf:64:15`: `MINIMAP2_ALIGN` is not defined

    ```nextflow
      aligned_l = MINIMAP2_ALIGN(
                  ^^^^^^^^^^^^^^
    ```

- Error: `workflows/original_local.nf:75:16`: `CLAIR3_CUSTOM` is not defined

    ```nextflow
      varcalls_l = CLAIR3_CUSTOM(
                   ^^^^^^^^^^^^^
    ```

- Error: `workflows/original_local.nf:103:3`: `MULTIQC` is not defined

    ```nextflow
      MULTIQC(ch_multiqc_input)
      ^^^^^^^
    ```

- Error: `workflows/pathogenepidemiology.nf:11:1`: Module could not be parsed: '/home/runner/work/strict-syntax-health/strict-syntax-health/pipelines/pathogenepidemiology/modules/nf-core/multiqc/main.nf'

    ```nextflow
    include { MULTIQC                } from '../modules/nf-core/multiqc/main'
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `workflows/pathogenepidemiology.nf:87:5`: `MULTIQC` is not defined

    ```nextflow
        MULTIQC(
        ^^^^^^^
    ```

- Error: `workflows/pathogenepidemiology.nf:101:27`: `MULTIQC` is not defined

    ```nextflow
        emit:multiqc_report = MULTIQC.out.report.map { _meta, report -> [report] }.toList() // channel: /path/to/multiqc_report.html
                              ^^^^^^^
    ```


## :warning: Warnings

- Warning: `workflows/download_references.nf:11:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        ch_refs = Channel.of(params.queryurl, params.hosturl)
                  ^^^^^^^
    ```

- Warning: `workflows/original_local.nf:29:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
      ch_samples = Channel
                   ^^^^^^^
    ```

- Warning: `workflows/original_local.nf:40:44`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
      ch_reads = ch_samples.map { meta, reads, platform -> 
                                               ^^^^^^^^
    ```

- Warning: `workflows/original_local.nf:43:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
      ch_hostref = Channel.of(params.hostref)
                   ^^^^^^^
    ```

- Warning: `workflows/original_local.nf:44:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
      ch_adapters = Channel.of("${workflow.launchDir}/adapters/adapters.fa")
                    ^^^^^^^
    ```

- Warning: `workflows/original_local.nf:45:17`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
      ch_reffasta = Channel.fromPath("${params.query_ref}")
                    ^^^^^^^
    ```

- Warning: `workflows/original_local.nf:57:3`: Variable was declared but not used

    ```nextflow
      ch_mm2align_input = hostrm_prepped.reads.map { meta, reads -> 
      ^^^^^^^^^^^^^^^^^
    ```

- Warning: `workflows/original_local.nf:75:3`: Variable was declared but not used

    ```nextflow
      varcalls_l = CLAIR3_CUSTOM(
      ^^^^^^^^^^
    ```

- Warning: `workflows/original_local.nf:89:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
      ch_multiqc_input = Channel.empty()
                         ^^^^^^^
    ```

- Warning: `workflows/original_local.nf:91:34`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            fastqc_out.zip.collect { meta, files -> files },
                                     ^^^^
    ```

- Warning: `workflows/original_local.nf:92:40`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            hostrm_prepped.stats.collect { meta, files -> files },
                                           ^^^^
    ```

- Warning: `workflows/original_local.nf:93:38`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            hostrm_prepped.log.collect { meta, files -> files },
                                         ^^^^
    ```

- Warning: `workflows/original_local.nf:94:44`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            hostrm_prepped.discarded.collect { meta, files -> files }
                                               ^^^^
    ```
