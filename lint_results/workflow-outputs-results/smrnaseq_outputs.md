# Workflow outputs migration: smrnaseq

- Generated: 2026-06-16T14:35:37.595089+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 54 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:20`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L20)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:30`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L30)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:37`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:46`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L46)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:64`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L64)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:101`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L101)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:118`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L118)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:128`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L128)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:147`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L147)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:171`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L171)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:182`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L182)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:197`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L197)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:212`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L212)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:231`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L231)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:242`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L242)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:254`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L254)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:259`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L259)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:265`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L265)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:271`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L271)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:278`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L278)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:285`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L285)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:292`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L292)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:298`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L298)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:305`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L305)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:312`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L312)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:316`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L316)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:328`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L328)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:336`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L336)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:344`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L344)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:352`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L352)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:368`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L368)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:377`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L377)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:393`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L393)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:402`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L402)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:410`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L410)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:417`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L417)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:435`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L435)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:447`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L447)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:456`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L456)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:460`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L460)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:465`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L465)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:473`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L473)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:477`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L477)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:486`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L486)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:500`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L500)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:510`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L510)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:517`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L517)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:532`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L532)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:547`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L547)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:553`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L553)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:557`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L557)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:570`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/conf/modules.config#L570)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/umitools/extract/tests/nextflow.config:3`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/modules/nf-core/umitools/extract/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`nextflow.config:108`](https://github.com/nf-core/smrnaseq/blob/a4a3530919f1563e9fe8d6ed4ca071a2fd77f521/nextflow.config#L108)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
