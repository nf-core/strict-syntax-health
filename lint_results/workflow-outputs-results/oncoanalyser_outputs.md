# Workflow outputs migration: oncoanalyser

- Generated: 2026-06-16T14:25:39.876759+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 35 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:16`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:40`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L40)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:49`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L49)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:58`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L58)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:67`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L67)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:76`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L76)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:85`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L85)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:94`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L94)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:103`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L103)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:112`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L112)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:121`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L121)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:130`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L130)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:139`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L139)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:148`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L148)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:156`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L156)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:165`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L165)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:174`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L174)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:186`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L186)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:195`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L195)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:204`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L204)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:212`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L212)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:220`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L220)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:229`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L229)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:238`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L238)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:247`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L247)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:256`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L256)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:265`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L265)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:274`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L274)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:283`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L283)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:292`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L292)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:301`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L301)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:311`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L311)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:320`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L320)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:329`](https://github.com/nf-core/oncoanalyser/blob/a2d25435924a88c52437c5574581f9fa9b784bcc/conf/modules.config#L329)

  ```nextflow
  publishDir = [
  ```
