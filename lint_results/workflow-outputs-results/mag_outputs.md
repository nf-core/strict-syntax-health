# Workflow outputs migration: mag

- Generated: 2026-06-16T14:21:15.741302+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 87 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:16`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:25`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L25)

  ```nextflow
  publishDir = [path: { "${params.outdir}/QC_shortreads/fastqc" }, mode: params.publish_dir_mode, pattern: "*.html"]
  ```

- [`conf/modules.config:39`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:58`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L58)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:82`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L82)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:106`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L106)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:117`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L117)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:137`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L137)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:156`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L156)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:169`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L169)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:187`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L187)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:197`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L197)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:216`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L216)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:231`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L231)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:248`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L248)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:269`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L269)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:294`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L294)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:309`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L309)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:317`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L317)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:335`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L335)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:354`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L354)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:365`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L365)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:375`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L375)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:385`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L385)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:395`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L395)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:405`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L405)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:415`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L415)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:424`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L424)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:432`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L432)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:440`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L440)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:449`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L449)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:462`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L462)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:472`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L472)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:488`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L488)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:495`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L495)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:509`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L509)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:526`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L526)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:538`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L538)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:548`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L548)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:558`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L558)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:565`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L565)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:577`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L577)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:585`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L585)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:594`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L594)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:602`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L602)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:610`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L610)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:623`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L623)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:633`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L633)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:642`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L642)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:654`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L654)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:664`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L664)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:673`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L673)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:691`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L691)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:699`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L699)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:713`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L713)

  ```nextflow
  publishDir = [path: { "${params.outdir}/Annotation/Prokka/${meta.assembler}" }, mode: params.publish_dir_mode, saveAs: { filename -> filename.equals('versions.yml') ? null : filename }]
  ```

- [`conf/modules.config:719`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L719)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:729`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L729)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:739`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L739)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:748`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L748)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:758`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L758)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:767`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L767)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:777`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L777)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:785`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L785)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:803`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L803)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:813`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L813)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:823`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L823)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:837`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L837)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:857`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L857)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:873`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L873)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:891`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L891)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:908`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L908)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:932`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L932)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:944`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L944)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:970`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L970)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:997`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L997)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`conf/modules.config:1001`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L1001)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1027`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L1027)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1041`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L1041)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1051`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L1051)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1066`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L1066)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1082`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L1082)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1091`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L1091)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1102`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L1102)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1111`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L1111)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1118`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/conf/modules.config#L1118)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/dastool/dastool/tests/nextflow.config:3`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/modules/nf-core/dastool/dastool/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`nextflow.config:227`](https://github.com/nf-core/mag/blob/e8eb3e154d16a0d39b72aa2d27f8653a87fdfafd/nextflow.config#L227)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
