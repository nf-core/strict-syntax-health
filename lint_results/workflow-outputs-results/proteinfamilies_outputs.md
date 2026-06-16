# Workflow outputs migration: proteinfamilies

- Generated: 2026-06-16T14:28:02.503117+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:106`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/main.nf#L106)

  ```nextflow
  output {
  ```

## Legacy `publishDir` references

Found 74 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:48`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:60`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L60)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:70`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:78`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L78)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:87`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L87)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:96`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L96)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:107`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L107)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:116`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L116)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:125`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L125)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:134`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L134)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:146`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L146)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:155`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L155)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:166`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L166)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:177`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L177)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:191`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L191)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:207`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L207)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:223`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L223)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:237`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L237)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:253`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L253)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:269`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L269)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:278`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L278)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:288`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L288)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:298`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L298)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:306`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L306)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:314`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L314)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:325`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L325)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:335`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L335)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:345`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L345)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:355`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L355)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:365`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L365)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:375`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L375)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:385`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L385)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:395`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L395)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:409`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L409)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:424`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L424)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:439`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L439)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:450`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L450)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:461`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L461)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:472`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L472)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:484`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L484)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:497`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L497)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:510`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L510)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:523`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L523)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:535`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L535)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:546`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L546)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:557`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L557)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:568`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L568)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:578`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L578)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:586`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L586)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:596`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L596)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:605`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L605)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:613`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L613)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:621`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L621)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:630`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L630)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:641`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L641)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:652`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L652)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:662`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L662)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:672`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L672)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:684`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L684)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:696`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L696)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:707`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L707)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:716`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L716)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:724`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L724)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:732`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L732)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:740`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L740)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:748`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L748)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:758`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L758)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:767`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/conf/modules.config#L767)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/mmseqs/cluster/tests/nextflow.config:3`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/modules/nf-core/mmseqs/cluster/tests/nextflow.config#L3)

  ```nextflow
  publishDir = [ enabled : false ]
  ```

- [`modules/nf-core/mmseqs/linclust/tests/nextflow.config:3`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/modules/nf-core/mmseqs/linclust/tests/nextflow.config#L3)

  ```nextflow
  publishDir = [ enabled : false ]
  ```

- [`nextflow.config:98`](https://github.com/nf-core/proteinfamilies/blob/0ba6da73682d7008c6ea997e679318ea9e5f8aae/nextflow.config#L98)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
