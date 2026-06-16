# Workflow outputs migration: viralmetagenome

- Generated: 2026-06-16T14:39:02.517479+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 117 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:27`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:37`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:56`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L56)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:88`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L88)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:110`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L110)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:135`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L135)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:142`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L142)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:164`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L164)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:184`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L184)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:196`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L196)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:216`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L216)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:225`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L225)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:234`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L234)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:243`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L243)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:253`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L253)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:266`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L266)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:278`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L278)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:288`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L288)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:296`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L296)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:306`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L306)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:317`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L317)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:323`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L323)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:330`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L330)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:343`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L343)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:363`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L363)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:373`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L373)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:392`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L392)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:404`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L404)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:414`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L414)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:435`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L435)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:447`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L447)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:457`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L457)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:476`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L476)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:485`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L485)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:492`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L492)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:501`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L501)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:507`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L507)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:515`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L515)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:526`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L526)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:537`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L537)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:547`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L547)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:557`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L557)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:572`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L572)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:583`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L583)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:604`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L604)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:616`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L616)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:627`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L627)

  ```nextflow
  publishDir =[
  ```

- [`conf/modules.config:651`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L651)

  ```nextflow
  publishDir =[
  ```

- [`conf/modules.config:673`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L673)

  ```nextflow
  publishDir =[
  ```

- [`conf/modules.config:685`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L685)

  ```nextflow
  publishDir =[
  ```

- [`conf/modules.config:701`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L701)

  ```nextflow
  publishDir =[
  ```

- [`conf/modules.config:716`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L716)

  ```nextflow
  publishDir =[
  ```

- [`conf/modules.config:730`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L730)

  ```nextflow
  publishDir =[
  ```

- [`conf/modules.config:743`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L743)

  ```nextflow
  publishDir =[
  ```

- [`conf/modules.config:760`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L760)

  ```nextflow
  publishDir =[
  ```

- [`conf/modules.config:773`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L773)

  ```nextflow
  publishDir =[
  ```

- [`conf/modules.config:785`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L785)

  ```nextflow
  publishDir =[
  ```

- [`conf/modules.config:806`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L806)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:815`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L815)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:822`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L822)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:833`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L833)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:852`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L852)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:872`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L872)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:881`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L881)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:891`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L891)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:901`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L901)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:911`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L911)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:928`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L928)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:943`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L943)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:967`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L967)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:981`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L981)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1010`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1010)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1018`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1018)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1040`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1040)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1053`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1053)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1076`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1076)

  ```nextflow
  publishDir =  [ enabled: false ]
  ```

- [`conf/modules.config:1081`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1081)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1094`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1094)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1107`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1107)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1120`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1120)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1133`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1133)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1146`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1146)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1159`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1159)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1174`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1174)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1187`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1187)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1204`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1204)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1219`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1219)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1231`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1231)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1243`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1243)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1255`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1255)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1268`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1268)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1281`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1281)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1295`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1295)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1307`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1307)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1319`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1319)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1331`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1331)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1348`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1348)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1359`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1359)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1370`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1370)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1377`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1377)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1389`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1389)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1404`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1404)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1413`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1413)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1426`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1426)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1437`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1437)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1450`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1450)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1460`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1460)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1473`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1473)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1482`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1482)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1498`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1498)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1508`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1508)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1526`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/conf/modules.config#L1526)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/mmseqs/cluster/tests/nextflow.config:3`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/modules/nf-core/mmseqs/cluster/tests/nextflow.config#L3)

  ```nextflow
  publishDir = [ enabled : false ]
  ```

- [`modules/nf-core/mmseqs/linclust/tests/nextflow.config:3`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/modules/nf-core/mmseqs/linclust/tests/nextflow.config#L3)

  ```nextflow
  publishDir = [ enabled : false ]
  ```

- [`modules/nf-core/umitools/extract/tests/nextflow.config:3`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/modules/nf-core/umitools/extract/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`nextflow.config:279`](https://github.com/nf-core/viralmetagenome/blob/e53186ea9957a9ad800c4d2d964325635344a4cc/nextflow.config#L279)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
