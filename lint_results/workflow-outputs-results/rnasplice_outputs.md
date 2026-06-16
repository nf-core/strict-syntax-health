# Workflow outputs migration: rnasplice

- Generated: 2026-06-16T14:32:23.534569+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 67 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:16`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:27`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:36`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L36)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:49`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L49)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:63`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L63)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:90`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L90)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:106`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L106)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:119`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L119)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:132`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L132)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:145`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L145)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:157`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L157)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:169`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L169)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:181`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L181)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:193`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L193)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:221`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L221)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:244`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L244)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:254`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L254)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:264`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L264)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:273`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L273)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:285`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L285)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:302`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L302)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:311`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L311)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:320`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L320)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:329`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L329)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:338`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L338)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:351`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L351)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:360`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L360)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:377`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L377)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:389`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L389)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:400`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L400)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:409`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L409)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:418`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L418)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:427`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L427)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:436`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L436)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:446`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L446)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:455`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L455)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:464`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L464)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:474`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L474)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:483`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L483)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:492`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L492)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:503`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L503)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:516`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L516)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:528`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L528)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:541`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L541)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:558`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L558)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:567`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L567)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:576`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L576)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:599`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L599)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:616`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L616)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:634`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L634)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:651`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L651)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:660`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L660)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:669`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L669)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:692`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L692)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:709`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L709)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:728`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L728)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:740`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L740)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:753`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L753)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:766`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L766)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:778`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L778)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:790`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L790)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:803`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L803)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:814`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/conf/modules.config#L814)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/subread/featurecounts/tests/nextflow.config:3`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/modules/nf-core/subread/featurecounts/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`modules/nf-core/umitools/extract/tests/nextflow.config:3`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/modules/nf-core/umitools/extract/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`nextflow.config:179`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/nextflow.config#L179)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```

- [`subworkflows/nf-core/bedgraph_bedclip_bedgraphtobigwig/tests/nextflow.config:3`](https://github.com/nf-core/rnasplice/blob/41d41cd209dbc3e8aaf3261f3ba26d59c9e24735/subworkflows/nf-core/bedgraph_bedclip_bedgraphtobigwig/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```
