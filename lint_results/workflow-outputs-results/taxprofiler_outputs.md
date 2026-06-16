# Workflow outputs migration: taxprofiler

- Generated: 2026-06-16T14:37:01.635569+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 87 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:33`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L33)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:43`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L43)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:52`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L52)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:61`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L61)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:77`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L77)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:110`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L110)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:138`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L138)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:168`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L168)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:193`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L193)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:202`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L202)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:211`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L211)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:220`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L220)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:230`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L230)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:243`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L243)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:272`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L272)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:301`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L301)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:330`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L330)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:359`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L359)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:387`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L387)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:410`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L410)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:423`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L423)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:453`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L453)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:463`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L463)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:473`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L473)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:485`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L485)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:495`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L495)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:514`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L514)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:523`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L523)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:543`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L543)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:554`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L554)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:565`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L565)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:576`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L576)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:587`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L587)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:596`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L596)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:605`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L605)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:621`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L621)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:630`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L630)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:639`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L639)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:655`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L655)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:666`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L666)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:675`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L675)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:686`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L686)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:697`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L697)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:706`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L706)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:717`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L717)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:732`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L732)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:741`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L741)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:752`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L752)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:762`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L762)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:779`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L779)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:795`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L795)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:806`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L806)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:817`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L817)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:828`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L828)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:839`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L839)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:858`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L858)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:867`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L867)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:879`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L879)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:891`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L891)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:902`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L902)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:915`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L915)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:928`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L928)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:949`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L949)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:968`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L968)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:977`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/modules.config#L977)

  ```nextflow
  publishDir = [
  ```

- [`conf/test.config:67`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test.config#L67)

  ```nextflow
  publishDir = [
  ```

- [`conf/test.config:78`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test.config#L78)

  ```nextflow
  publishDir = [
  ```

- [`conf/test.config:93`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test.config#L93)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_alternativepreprocessing.config:62`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_alternativepreprocessing.config#L62)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_alternativepreprocessing.config:71`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_alternativepreprocessing.config#L71)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_falcobbduk.config:61`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_falcobbduk.config#L61)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_falcobbduk.config:70`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_falcobbduk.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_fastpnonpareilkrakenuniq.config:73`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_fastpnonpareilkrakenuniq.config#L73)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_fastpnonpareilkrakenuniq.config:84`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_fastpnonpareilkrakenuniq.config#L84)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_fastpnonpareilkrakenuniq.config:99`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_fastpnonpareilkrakenuniq.config#L99)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_malt.config:63`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_malt.config#L63)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_malt.config:72`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_malt.config#L72)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_minimal.config:59`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_minimal.config#L59)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_minimal.config:68`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_minimal.config#L68)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_motus.config:68`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_motus.config#L68)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_motus.config:77`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_motus.config#L77)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_nopreprocessing.config:62`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_nopreprocessing.config#L62)

  ```nextflow
  publishDir = [
  ```

- [`conf/test_nopreprocessing.config:71`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/conf/test_nopreprocessing.config#L71)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/nonpareil/nonpareil/tests/nextflow.config:3`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/modules/nf-core/nonpareil/nonpareil/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`nextflow.config:216`](https://github.com/nf-core/taxprofiler/blob/4fd02bfbe8d7980159190b9ec1eda71f437f7e54/nextflow.config#L216)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
