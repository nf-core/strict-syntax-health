# Workflow outputs migration: scnanoseq

- Generated: 2026-06-16T14:34:20.044012+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 92 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:38`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L38)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:50`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L50)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:62`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L62)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:75`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L75)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:87`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L87)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:99`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L99)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:111`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L111)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:125`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L125)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:137`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L137)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:149`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L149)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:162`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L162)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:174`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L174)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:190`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L190)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:198`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L198)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:206`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L206)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:214`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L214)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:228`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L228)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:237`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L237)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:250`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L250)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:258`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L258)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:267`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L267)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:276`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L276)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:284`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L284)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:298`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L298)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:306`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L306)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:321`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L321)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:341`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L341)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:353`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L353)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:363`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L363)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:372`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L372)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:381`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L381)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:392`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L392)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:402`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L402)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:414`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L414)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:422`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L422)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:443`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L443)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:461`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L461)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:481`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L481)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:497`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L497)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:508`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L508)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:518`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L518)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:528`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L528)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:538`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L538)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:549`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L549)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:560`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L560)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:571`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L571)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:581`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L581)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:591`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L591)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:601`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L601)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:613`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L613)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:625`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L625)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:637`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L637)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:649`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L649)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:661`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L661)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:672`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L672)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:685`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L685)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:697`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L697)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:715`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L715)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:726`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L726)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:738`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L738)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:753`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L753)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:761`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L761)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:769`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L769)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:777`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L777)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:791`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L791)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:807`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L807)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:816`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L816)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:825`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L825)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:834`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L834)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:845`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L845)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:856`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L856)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:871`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L871)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:885`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L885)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:901`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L901)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:910`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L910)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:919`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L919)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:928`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L928)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:940`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L940)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:952`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L952)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:980`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L980)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1002`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L1002)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1018`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L1018)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1030`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L1030)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1039`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L1039)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1057`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L1057)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1070`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L1070)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1085`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L1085)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1097`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L1097)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1110`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L1110)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1122`](https://github.com/nf-core/scnanoseq/blob/c4ecbf5bd974fd2e70e5f909b484117ea37d814e/conf/modules.config#L1122)

  ```nextflow
  publishDir = [
  ```
