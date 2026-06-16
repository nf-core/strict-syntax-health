# Workflow outputs migration: pangenome

- Generated: 2026-06-16T14:26:17.990832+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 31 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:88`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L88)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:112`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L112)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:138`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L138)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:164`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L164)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:173`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L173)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:199`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L199)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:217`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L217)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:248`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L248)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:256`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L256)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:265`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L265)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:275`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L275)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:285`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L285)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:295`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L295)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:304`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L304)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:314`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L314)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:324`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L324)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:334`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L334)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:344`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L344)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:354`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L354)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:364`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L364)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:373`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L373)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:383`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L383)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:392`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L392)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:400`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L400)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:408`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L408)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:416`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L416)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:424`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L424)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:432`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L432)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:440`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L440)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:449`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L449)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:462`](https://github.com/nf-core/pangenome/blob/e8e7ced9efc1484b3189bb2e2a1f137fec6642ec/conf/modules.config#L462)

  ```nextflow
  publishDir = [
  ```
