# Workflow outputs migration: diseasemodulediscovery

- Generated: 2026-06-16T14:14:34.688465+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 21 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:17`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:27`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:39`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:65`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L65)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:73`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L73)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:86`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L86)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:102`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L102)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:110`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L110)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:121`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L121)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:130`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L130)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:138`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L138)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:150`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L150)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:162`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L162)

  ```nextflow
  publishDir = [enabled: false]
  ```

- [`conf/modules.config:166`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L166)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:179`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L179)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:187`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L187)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:196`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L196)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:204`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L204)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:212`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L212)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:220`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/conf/modules.config#L220)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:98`](https://github.com/nf-core/diseasemodulediscovery/blob/4d35338c037b7fc01b731a41f1e060f94129bfcc/nextflow.config#L98)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
