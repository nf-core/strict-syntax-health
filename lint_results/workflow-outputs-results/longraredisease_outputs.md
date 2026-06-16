# Workflow outputs migration: longraredisease

- Generated: 2026-06-16T14:20:37.100071+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 76 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:41`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L41)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:50`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L50)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:63`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L63)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:72`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L72)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:80`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L80)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:97`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L97)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:117`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L117)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:125`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L125)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:132`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L132)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:139`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L139)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:146`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L146)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:154`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L154)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:162`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L162)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:171`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L171)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:178`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L178)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:187`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L187)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:196`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L196)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:203`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L203)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:211`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L211)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:220`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L220)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:228`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L228)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:237`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L237)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:244`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L244)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:252`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L252)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:260`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L260)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:278`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L278)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:289`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L289)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:297`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L297)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:305`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L305)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:312`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L312)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:320`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L320)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:328`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L328)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:337`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L337)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:343`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L343)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:352`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L352)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:361`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L361)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:370`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L370)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:377`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L377)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:385`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L385)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:403`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L403)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:410`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L410)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:417`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L417)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:424`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L424)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:431`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L431)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:440`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L440)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:448`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L448)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:457`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L457)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:465`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L465)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:473`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L473)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:504`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L504)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:513`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L513)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:522`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L522)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:530`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L530)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:538`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L538)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:546`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L546)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:575`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L575)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:583`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L583)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:592`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L592)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:601`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L601)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:610`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L610)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:619`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L619)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:628`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L628)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:635`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L635)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:643`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L643)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:652`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L652)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:667`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L667)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:682`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L682)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:691`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L691)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:700`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L700)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:707`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L707)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:719`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L719)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:726`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/conf/modules.config#L726)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/local/call_sv/tests/nextflow.config:22`](https://github.com/nf-core/longraredisease/blob/36831ff50fe23d18cbc24ea510d3d76bfcd90403/subworkflows/local/call_sv/tests/nextflow.config#L22)

  ```nextflow
  publishDir = [ enabled: false ]
  ```
