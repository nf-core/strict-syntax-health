# Workflow outputs migration: ampliseq

- Generated: 2026-06-16T14:08:09.702890+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 96 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:28`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L28)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:37`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:56`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L56)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:71`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L71)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:89`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L89)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:99`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L99)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:107`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L107)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:116`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L116)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:137`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L137)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:155`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L155)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:165`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L165)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:195`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L195)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:237`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L237)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:254`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L254)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:266`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L266)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:274`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L274)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:288`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L288)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:298`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L298)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:307`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L307)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:317`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L317)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:327`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L327)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:345`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L345)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:367`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L367)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:384`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L384)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:392`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L392)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:409`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L409)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:427`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L427)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:437`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L437)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:445`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L445)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:453`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L453)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:463`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L463)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:475`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L475)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:483`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L483)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:497`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L497)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:508`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L508)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:517`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L517)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:525`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L525)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:538`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L538)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:559`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L559)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:574`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L574)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:584`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L584)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:594`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L594)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:604`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L604)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:612`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L612)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:621`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L621)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:632`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L632)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:642`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L642)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:652`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L652)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:668`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L668)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:678`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L678)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:688`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L688)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:696`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L696)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:704`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L704)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:713`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L713)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:724`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L724)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:733`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L733)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:742`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L742)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:751`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L751)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:760`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L760)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:769`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L769)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:779`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L779)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:789`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L789)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:798`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L798)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:806`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L806)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:815`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L815)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:824`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L824)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:842`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L842)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:859`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L859)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:874`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L874)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:882`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L882)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:890`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L890)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:899`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L899)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:914`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L914)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:922`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L922)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:930`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L930)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:938`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L938)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:963`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L963)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:971`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L971)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:984`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L984)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1000`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L1000)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1027`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L1027)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1049`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L1049)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1065`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L1065)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1081`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L1081)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1108`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L1108)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1128`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L1128)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1154`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L1154)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1176`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L1176)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1189`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L1189)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1197`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L1197)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1205`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L1205)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1213`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L1213)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1222`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L1222)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1230`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/conf/modules.config#L1230)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:204`](https://github.com/nf-core/ampliseq/blob/b4d98050ada6c133dbab0f1983de90b0bc9c670b/nextflow.config#L204)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
