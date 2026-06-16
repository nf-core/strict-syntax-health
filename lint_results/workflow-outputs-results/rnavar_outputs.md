# Workflow outputs migration: rnavar

- Generated: 2026-06-16T14:32:44.401764+00:00
- Status: :warning: **warn** — uses the new `output {}` syntax but still has legacy `publishDir` references to migrate

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` block

Found 1 top-level `output {}` block:

- [`main.nf:223`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/main.nf#L223)

  ```nextflow
  output {
  ```

## Legacy `publishDir` references

Found 34 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:16`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:25`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L25)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:39`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L39)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:48`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L48)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:57`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L57)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:66`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L66)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:76`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L76)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:84`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L84)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:116`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L116)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:153`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L153)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:174`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L174)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:184`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L184)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:194`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L194)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:208`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L208)

  ```nextflow
  publishDir  = [ enabled: false ]
  ```

- [`conf/modules.config:222`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L222)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:233`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L233)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:246`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L246)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:266`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L266)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:280`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L280)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:289`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L289)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:304`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L304)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:324`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L324)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:329`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L329)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:338`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L338)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:355`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L355)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:374`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules.config#L374)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/annotate.config:37`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules/annotate.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/annotate.config:50`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules/annotate.config#L50)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/annotate.config:80`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules/annotate.config#L80)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/annotate.config:88`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules/annotate.config#L88)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_cache.config:14`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules/prepare_cache.config#L14)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules/prepare_cache.config:23`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/conf/modules/prepare_cache.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:134`](https://github.com/nf-core/rnavar/blob/cc14a0e752e4bdfd5740d0478cf519743b5b6000/nextflow.config#L134)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
