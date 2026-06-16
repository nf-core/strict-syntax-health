# Workflow outputs migration: bacass

- Generated: 2026-06-16T14:08:56.854644+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 33 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:18`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L18)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:27`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:36`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L36)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:46`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L46)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:64`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L64)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:91`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L91)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:108`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L108)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:130`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L130)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:152`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L152)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:162`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L162)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:181`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L181)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:200`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L200)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:210`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L210)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:220`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L220)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:242`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L242)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:251`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L251)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:260`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L260)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:269`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L269)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:279`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L279)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:295`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L295)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:313`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L313)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:322`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L322)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:332`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L332)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:341`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L341)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:350`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L350)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:359`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L359)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:367`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L367)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:376`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L376)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:405`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L405)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:415`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L415)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:425`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L425)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:435`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L435)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:449`](https://github.com/nf-core/bacass/blob/5444383ce0451be672571c10094766fed17edb06/conf/modules.config#L449)

  ```nextflow
  publishDir  = [
  ```
