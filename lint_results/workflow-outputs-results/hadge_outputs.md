# Workflow outputs migration: hadge

- Generated: 2026-06-16T14:19:13.374772+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 33 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:29`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L29)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:35`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L35)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:43`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L43)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:49`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L49)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:56`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L56)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:65`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L65)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:74`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L74)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:82`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L82)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:90`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L90)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:99`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L99)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:115`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L115)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:145`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L145)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:173`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L173)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:205`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L205)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:234`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L234)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:260`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L260)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:287`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L287)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:295`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L295)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:304`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L304)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:327`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L327)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:352`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L352)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:369`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L369)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:402`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L402)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:427`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L427)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:453`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L453)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:499`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L499)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:507`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L507)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:515`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L515)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:530`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L530)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:537`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L537)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:555`](https://github.com/nf-core/hadge/blob/067f0a18b0bc6422c7665ac6b1e83b36a3bfb5de/conf/modules.config#L555)

  ```nextflow
  publishDir = [
  ```
