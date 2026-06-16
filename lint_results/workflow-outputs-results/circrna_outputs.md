# Workflow outputs migration: circrna

- Generated: 2026-06-16T14:10:56.997263+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 128 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:30`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:38`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L38)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:46`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L46)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:60`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L60)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:78`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L78)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:87`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L87)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:96`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L96)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:105`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L105)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:113`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L113)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:121`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L121)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:130`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L130)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:138`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L138)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:146`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L146)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:158`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L158)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:168`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L168)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:176`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L176)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:185`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L185)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:195`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L195)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:208`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L208)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:219`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L219)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:229`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L229)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:240`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L240)

  ```nextflow
  publishDir      = [
  ```

- [`conf/modules.config:250`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L250)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:271`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L271)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:279`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L279)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:303`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L303)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:316`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L316)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:324`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L324)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:334`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L334)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:343`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L343)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:354`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L354)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:368`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L368)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:376`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L376)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:386`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L386)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:394`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L394)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:407`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L407)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:417`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L417)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:427`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L427)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:437`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L437)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:447`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L447)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:456`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L456)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:466`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L466)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:477`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L477)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:484`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L484)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:491`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L491)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:498`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L498)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:504`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L504)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:512`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L512)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:520`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L520)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:529`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L529)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:536`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L536)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:544`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L544)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:552`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L552)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:561`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L561)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:575`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L575)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:592`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L592)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:600`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L600)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:610`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L610)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:619`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L619)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:629`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L629)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:638`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L638)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:646`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L646)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:654`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L654)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:662`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L662)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:668`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L668)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:676`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L676)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:682`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L682)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:691`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L691)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:702`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L702)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:712`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L712)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:722`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L722)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:730`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L730)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:741`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L741)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:750`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L750)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:760`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L760)

  ```nextflow
  publishDir          = [
  ```

- [`conf/modules.config:769`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L769)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:777`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L777)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:796`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L796)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:805`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L805)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:814`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L814)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:824`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L824)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:832`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L832)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:843`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L843)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:851`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L851)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:859`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L859)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:868`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L868)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:893`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L893)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:899`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L899)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:907`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L907)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:915`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L915)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:925`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L925)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:935`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L935)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:945`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L945)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:959`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L959)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:969`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L969)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:978`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L978)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:988`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L988)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:996`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L996)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1021`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1021)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1031`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1031)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1039`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1039)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1051`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1051)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1059`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1059)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1067`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1067)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1075`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1075)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1083`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1083)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1094`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1094)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1102`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1102)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1110`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1110)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1118`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1118)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1126`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1126)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1134`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1134)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1142`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1142)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1152`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1152)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1163`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1163)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1172`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1172)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1181`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1181)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1189`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1189)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1197`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1197)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1205`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1205)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1213`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1213)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1221`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1221)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1229`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1229)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1237`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1237)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1246`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/conf/modules.config#L1246)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:123`](https://github.com/nf-core/circrna/blob/bdba2f02bc819da073fc80b18ba9cc9d76292620/nextflow.config#L123)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
