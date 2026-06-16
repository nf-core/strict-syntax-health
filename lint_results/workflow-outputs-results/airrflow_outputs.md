# Workflow outputs migration: airrflow

- Generated: 2026-06-16T14:07:26.359308+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 85 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:41`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L41)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:65`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L65)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:74`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L74)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:86`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L86)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:95`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L95)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:101`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L101)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:107`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L107)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:118`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L118)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:126`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L126)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:134`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L134)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:143`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L143)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:152`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L152)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:162`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L162)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:172`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L172)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:181`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L181)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:190`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L190)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:199`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L199)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:209`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L209)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:219`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L219)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:228`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L228)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:237`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L237)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:247`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L247)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:258`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L258)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:267`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L267)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:276`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L276)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:285`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L285)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:295`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L295)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:303`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L303)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:312`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L312)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:323`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L323)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:333`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L333)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:342`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L342)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:350`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L350)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:360`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L360)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:370`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L370)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:380`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L380)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:388`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L388)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:395`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L395)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:403`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L403)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:410`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L410)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:417`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L417)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:427`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L427)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:437`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L437)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:447`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L447)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:457`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L457)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:466`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L466)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:479`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L479)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:488`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L488)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:494`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L494)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:502`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L502)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:512`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L512)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:521`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L521)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:530`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L530)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:538`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L538)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:546`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L546)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:554`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L554)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:562`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L562)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:574`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L574)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:582`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L582)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:590`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L590)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:598`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L598)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:610`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L610)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:622`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L622)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:631`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L631)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:639`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L639)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:649`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L649)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:658`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L658)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:670`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L670)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:684`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L684)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:698`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L698)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:708`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L708)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:717`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L717)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:728`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L728)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:737`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L737)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:748`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L748)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:759`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L759)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:771`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L771)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:786`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L786)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:795`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L795)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:803`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L803)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:812`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/conf/modules.config#L812)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:33`](https://github.com/nf-core/airrflow/blob/5aef057db77f5b99afed70e36a3d945ec51eee48/nextflow.config#L33)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
