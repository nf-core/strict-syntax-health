# Workflow outputs migration: viralrecon

- Generated: 2026-06-16T14:39:34.888105+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 174 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:18`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules.config#L18)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:34`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules.config#L34)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:19`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L19)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:29`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L29)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:38`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L38)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:47`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L47)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:57`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L57)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:68`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L68)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:92`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L92)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:102`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L102)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:112`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L112)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:127`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L127)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:138`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L138)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:155`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L155)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:163`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L163)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:172`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L172)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:183`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L183)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:193`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L193)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:204`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L204)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:214`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L214)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:230`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L230)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:239`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L239)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:248`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L248)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:258`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L258)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:273`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L273)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:288`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L288)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:297`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L297)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:308`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L308)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:326`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L326)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:335`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L335)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:345`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L345)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:355`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L355)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:364`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L364)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:378`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L378)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:389`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L389)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:397`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L397)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:406`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L406)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:414`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L414)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:428`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L428)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:438`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L438)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:447`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L447)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:455`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L455)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:465`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L465)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:473`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L473)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:482`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L482)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:491`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L491)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:500`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L500)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:508`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L508)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:523`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L523)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:531`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L531)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:541`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L541)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:550`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L550)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:559`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L559)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:568`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L568)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:577`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L577)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:586`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L586)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:594`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L594)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:607`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L607)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:616`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L616)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:631`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L631)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:655`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L655)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:664`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L664)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:675`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L675)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:685`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L685)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:693`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L693)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:701`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L701)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:709`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L709)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:719`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L719)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:726`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L726)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:733`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L733)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:742`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L742)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:753`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L753)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:764`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L764)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:775`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L775)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:782`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L782)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:789`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L789)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:796`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L796)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:804`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L804)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:811`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L811)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:820`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L820)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:831`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L831)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:838`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L838)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:846`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L846)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:855`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L855)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:864`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L864)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:873`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L873)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:881`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L881)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:894`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L894)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:904`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L904)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:916`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L916)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:926`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L926)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:934`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L934)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:946`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L946)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:957`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L957)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:972`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L972)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:979`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L979)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:989`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L989)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1000`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1000)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1008`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1008)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1019`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1019)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1030`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1030)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1041`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1041)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1051`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1051)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1066`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1066)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1073`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1073)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1083`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1083)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1094`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1094)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1102`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1102)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1113`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1113)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1124`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1124)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1135`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1135)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1146`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1146)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1153`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1153)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1164`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1164)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1172`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1172)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1183`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1183)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1194`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1194)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1205`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1205)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_illumina.config:1219`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_illumina.config#L1219)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:19`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L19)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:28`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L28)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:38`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L38)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:46`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L46)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:55`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L55)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:64`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L64)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:72`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L72)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:81`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L81)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:90`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L90)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:99`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L99)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:108`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L108)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:118`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L118)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:127`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L127)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:137`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L137)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:147`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L147)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:156`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L156)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:166`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L166)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:174`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L174)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:183`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L183)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:191`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L191)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:202`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L202)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:212`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L212)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:220`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L220)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:228`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L228)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:236`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L236)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:251`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L251)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:261`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L261)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:271`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L271)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:281`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L281)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:290`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L290)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:299`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L299)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:308`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L308)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:318`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L318)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:325`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L325)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:332`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L332)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:341`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L341)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:350`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L350)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:359`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L359)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:369`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L369)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:380`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L380)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:392`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L392)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:403`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L403)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:413`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L413)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:423`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L423)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:432`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L432)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:441`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L441)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:450`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L450)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:459`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L459)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:467`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L467)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:479`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L479)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:487`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L487)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:495`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L495)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_nanopore.config:509`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/conf/modules_nanopore.config#L509)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/pycoqc/tests/nextflow.config:3`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/modules/nf-core/pycoqc/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`nextflow.config:145`](https://github.com/nf-core/viralrecon/blob/d1668569b89d8f15856ba0505c3a40b1fde8d9a0/nextflow.config#L145)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
