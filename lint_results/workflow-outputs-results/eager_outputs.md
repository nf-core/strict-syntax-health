# Workflow outputs migration: eager

- Generated: 2026-06-16T14:15:38.941934+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 131 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:36`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L36)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:44`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L44)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:56`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L56)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:69`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L69)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:82`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L82)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:95`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L95)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:114`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L114)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:141`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L141)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:171`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L171)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:202`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L202)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:220`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L220)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:235`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L235)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:246`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L246)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:252`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L252)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:263`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L263)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:274`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L274)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:285`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L285)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:297`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L297)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:309`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L309)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:320`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L320)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:331`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L331)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:346`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L346)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:355`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L355)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:363`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L363)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:374`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L374)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:384`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L384)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:398`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L398)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:415`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L415)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:429`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L429)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:442`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L442)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:454`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L454)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:471`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L471)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:484`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L484)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:498`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L498)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:510`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L510)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:524`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L524)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:533`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L533)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:549`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L549)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:573`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L573)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:596`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L596)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:604`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L604)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:613`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L613)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:621`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L621)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:630`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L630)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:643`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L643)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:655`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L655)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:670`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L670)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:679`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L679)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:688`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L688)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:704`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L704)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:713`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L713)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:721`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L721)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:727`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L727)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:736`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L736)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:744`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L744)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:752`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L752)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:765`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L765)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:777`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L777)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:797`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L797)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:812`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L812)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:825`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L825)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:846`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L846)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:857`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L857)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:866`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L866)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:879`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L879)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:897`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L897)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:905`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L905)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:915`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L915)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:926`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L926)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:933`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L933)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:946`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L946)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:965`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L965)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:975`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L975)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:988`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L988)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:997`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L997)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1006`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1006)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1027`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1027)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1039`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1039)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1047`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1047)

  ```nextflow
  publishDir    = [
  ```

- [`conf/modules.config:1056`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1056)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1065`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1065)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1084`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1084)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1105`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1105)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1118`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1118)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1126`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1126)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1140`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1140)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1161`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1161)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1179`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1179)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1199`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1199)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1211`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1211)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1223`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1223)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1238`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1238)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1250`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1250)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1269`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1269)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1289`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1289)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1317`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1317)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1333`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1333)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1343`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1343)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1353`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1353)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1368`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1368)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1384`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1384)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1406`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1406)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1420`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1420)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1430`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1430)

  ```nextflow
  publishDir    = [
  ```

- [`conf/modules.config:1440`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1440)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1451`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1451)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1466`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1466)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1474`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1474)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1487`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1487)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1499`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1499)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1511`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1511)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1519`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1519)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1532`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1532)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1544`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1544)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1564`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1564)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1582`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1582)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1590`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1590)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1603`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1603)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1618`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1618)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1629`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1629)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1652`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1652)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1665`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1665)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1685`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1685)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1706`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1706)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1719`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1719)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1731`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1731)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1752`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1752)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1774`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/conf/modules.config#L1774)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_align_bwaaln/nextflow.config:7`](https://github.com/nf-core/eager/blob/f77d2464a7c6fe06b67ce1832f2fe72ba21c8fde/subworkflows/nf-core/fastq_align_bwaaln/nextflow.config#L7)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```
