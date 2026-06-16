# Workflow outputs migration: scdownstream

- Generated: 2026-06-16T14:33:58.175289+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 64 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:15`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:23`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L23)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:33`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L33)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:43`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L43)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:53`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L53)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:59`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L59)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:76`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L76)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:86`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L86)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:99`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L99)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:109`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L109)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:121`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L121)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:132`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L132)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:142`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L142)

  ```nextflow
  publishDir       = [
  ```

- [`conf/modules.config:152`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L152)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:165`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L165)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:178`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L178)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:188`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L188)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:198`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L198)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:208`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L208)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:217`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L217)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:227`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L227)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:237`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L237)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:249`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L249)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:260`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L260)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:268`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L268)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:274`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L274)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:283`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L283)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:300`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L300)

  ```nextflow
  publishDir             = [
  ```

- [`conf/modules.config:311`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L311)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:320`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L320)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:331`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L331)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:340`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L340)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:359`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L359)

  ```nextflow
  publishDir                 = [
  ```

- [`conf/modules.config:375`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L375)

  ```nextflow
  publishDir                 = [
  ```

- [`conf/modules.config:383`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L383)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:399`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L399)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:408`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L408)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:417`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L417)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:426`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L426)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:432`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L432)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:441`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L441)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:450`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L450)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:459`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L459)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:465`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L465)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:475`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L475)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:484`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L484)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:496`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L496)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:507`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L507)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:514`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L514)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:523`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L523)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:533`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L533)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:545`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L545)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:555`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L555)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:565`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L565)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:574`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L574)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:583`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L583)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:591`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L591)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:600`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L600)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:610`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L610)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:620`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L620)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:629`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L629)

  ```nextflow
  publishDir    = [
  ```

- [`conf/modules.config:638`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L638)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:648`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/conf/modules.config#L648)

  ```nextflow
  publishDir = [
  ```

- [`nextflow.config:132`](https://github.com/nf-core/scdownstream/blob/bcb4c67210cff40a150a558dd82a8b48ca7db3d7/nextflow.config#L132)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
