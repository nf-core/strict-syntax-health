# Workflow outputs migration: hlatyping

- Generated: 2026-06-16T14:19:43.193770+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 20 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:22`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L22)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:30`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L30)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:35`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L35)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:41`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L41)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:48`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L48)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:53`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L53)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:61`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L61)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:69`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L69)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:83`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L83)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:87`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L87)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:91`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L91)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:95`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L95)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:99`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L99)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:104`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L104)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:109`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L109)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:116`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L116)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:125`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/conf/modules.config#L125)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/hlala/preparegraph/tests/nextflow.config:7`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/modules/nf-core/hlala/preparegraph/tests/nextflow.config#L7)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:75`](https://github.com/nf-core/hlatyping/blob/2bce66c4869373feeb1247fa6a85165802da57c5/nextflow.config#L75)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
