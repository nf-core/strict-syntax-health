# Workflow outputs migration: cutandrun

- Generated: 2026-06-16T14:12:15.360150+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 83 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:20`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L20)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:38`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L38)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:44`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L44)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:52`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L52)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:61`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L61)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:70`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:80`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L80)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:91`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L91)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:97`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L97)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:103`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L103)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:109`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L109)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:118`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L118)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:134`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L134)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:144`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L144)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:156`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L156)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:185`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L185)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:209`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L209)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:231`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L231)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:240`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L240)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:250`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L250)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:260`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L260)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:270`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L270)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:280`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L280)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:302`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L302)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:312`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L312)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:322`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L322)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:332`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L332)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:350`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L350)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:367`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L367)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:377`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L377)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:386`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L386)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:397`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L397)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:407`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L407)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:416`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L416)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:425`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L425)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:432`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L432)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:438`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L438)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:446`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L446)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:456`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L456)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:462`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L462)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:485`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L485)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:492`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L492)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:501`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L501)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:515`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L515)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:529`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L529)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:536`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L536)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:546`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L546)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:555`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L555)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:566`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L566)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:581`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L581)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:593`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L593)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:604`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L604)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:619`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L619)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:627`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L627)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:635`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L635)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:647`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L647)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:663`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L663)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:673`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L673)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:683`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L683)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:693`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L693)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:703`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L703)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:713`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L713)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:723`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L723)

  ```nextflow
  //     publishDir   = [
  ```

- [`conf/modules.config:733`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L733)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:743`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L743)

  ```nextflow
  //     publishDir   = [
  ```

- [`conf/modules.config:753`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L753)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:763`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L763)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:773`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L773)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:783`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L783)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:794`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L794)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:801`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L801)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:810`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L810)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:820`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L820)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:829`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L829)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:835`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L835)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:841`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L841)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:850`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L850)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:857`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L857)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:863`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L863)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:869`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L869)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:881`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L881)

  ```nextflow
  publishDir   = [
  ```

- [`conf/modules.config:890`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L890)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules.config:897`](https://github.com/nf-core/cutandrun/blob/d59714a50c67486951b480febb726e47a7833187/conf/modules.config#L897)

  ```nextflow
  publishDir = [
  ```
