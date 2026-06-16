# Workflow outputs migration: pacsomatic

- Generated: 2026-06-16T14:25:48.734052+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 40 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:31`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:37`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:47`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L47)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:53`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L53)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:59`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L59)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:80`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L80)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:87`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L87)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:95`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L95)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:103`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L103)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:111`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L111)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:119`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L119)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:127`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L127)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:135`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L135)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:155`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L155)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:165`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L165)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:177`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L177)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:185`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L185)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:193`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L193)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:205`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L205)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:216`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L216)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:237`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L237)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:246`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L246)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:259`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L259)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:267`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L267)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:275`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L275)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:283`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L283)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:293`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L293)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:303`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L303)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:311`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L311)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:333`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L333)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:347`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L347)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:365`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L365)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:379`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L379)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:387`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L387)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:395`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L395)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:407`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L407)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:415`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L415)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:423`](https://github.com/nf-core/pacsomatic/blob/24c84cb371b0339c1d65a4de9451671945e19772/conf/modules.config#L423)

  ```nextflow
  publishDir = [
  ```
