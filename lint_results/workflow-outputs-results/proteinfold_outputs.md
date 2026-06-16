# Workflow outputs migration: proteinfold

- Generated: 2026-06-16T14:28:23.735068+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 62 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:18`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules.config#L18)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:32`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules.config#L32)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:41`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules.config#L41)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:49`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules.config#L49)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:57`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules.config#L57)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:66`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules.config#L66)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold2.config:19`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold2.config#L19)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold2.config:28`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold2.config#L28)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold2.config:34`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold2.config#L34)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold2.config:43`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold2.config#L43)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold2.config:52`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold2.config#L52)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold2.config:58`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold2.config#L58)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold2.config:67`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold2.config#L67)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold2.config:73`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold2.config#L73)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold2.config:79`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold2.config#L79)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold2.config:92`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold2.config#L92)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold2.config:122`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold2.config#L122)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold2.config:151`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold2.config#L151)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold3.config:19`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold3.config#L19)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold3.config:27`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold3.config#L27)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold3.config:71`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold3.config#L71)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold3.config:88`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold3.config#L88)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_alphafold3.config:100`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold3.config#L100)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules_alphafold3.config:149`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_alphafold3.config#L149)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_boltz.config:18`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_boltz.config#L18)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_boltz.config:31`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_boltz.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_boltz.config:38`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_boltz.config#L38)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_boltz.config:45`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_boltz.config#L45)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_boltz.config:52`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_boltz.config#L52)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_boltz.config:61`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_boltz.config#L61)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_boltz.config:78`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_boltz.config#L78)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_colabfold.config:17`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_colabfold.config#L17)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_colabfold.config:40`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_colabfold.config#L40)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_colabfold.config:71`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_colabfold.config#L71)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_colabfold.config:78`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_colabfold.config#L78)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_colabfold.config:84`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_colabfold.config#L84)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_esmfold.config:16`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_esmfold.config#L16)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_esmfold.config:29`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_esmfold.config#L29)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_helixfold3.config:20`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_helixfold3.config#L20)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_helixfold3.config:31`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_helixfold3.config#L31)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_helixfold3.config:37`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_helixfold3.config#L37)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_helixfold3.config:43`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_helixfold3.config#L43)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_helixfold3.config:52`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_helixfold3.config#L52)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_helixfold3.config:58`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_helixfold3.config#L58)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_helixfold3.config:64`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_helixfold3.config#L64)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_helixfold3.config:70`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_helixfold3.config#L70)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_helixfold3.config:76`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_helixfold3.config#L76)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_helixfold3.config:82`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_helixfold3.config#L82)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_helixfold3.config:88`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_helixfold3.config#L88)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_helixfold3.config:94`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_helixfold3.config#L94)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_helixfold3.config:110`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_helixfold3.config#L110)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_rosettafold2na.config:25`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_rosettafold2na.config#L25)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_rosettafold2na.config:36`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_rosettafold2na.config#L36)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_rosettafold2na.config:45`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_rosettafold2na.config#L45)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules_rosettafold_all_atom.config:15`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_rosettafold_all_atom.config#L15)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules_rosettafold_all_atom.config:24`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_rosettafold_all_atom.config#L24)

  ```nextflow
  publishDir  = [
  ```

- [`conf/modules_rosettafold_all_atom.config:60`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/conf/modules_rosettafold_all_atom.config#L60)

  ```nextflow
  publishDir = [
  ```

- [`modules/local/run_alphafold2/main.nf:89`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/modules/local/run_alphafold2/main.nf#L89)

  ```nextflow
  # Can't use fasta.baseName to batch outputs in publishDir
  ```

- [`modules/local/run_alphafold2_msa/main.nf:66`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/modules/local/run_alphafold2_msa/main.nf#L66)

  ```nextflow
  # Can't use fasta.baseName to batch outputs in publishDir
  ```

- [`modules/local/run_alphafold2_pred/main.nf:68`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/modules/local/run_alphafold2_pred/main.nf#L68)

  ```nextflow
  # Can't use fasta.baseName to batch outputs in publishDir
  ```

- [`modules/nf-core/mmseqs/createindex/tests/nextflow.config:3`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/modules/nf-core/mmseqs/createindex/tests/nextflow.config#L3)

  ```nextflow
  publishDir = [ enabled : false ]
  ```

- [`nextflow.config:257`](https://github.com/nf-core/proteinfold/blob/adda74069284af8d1f3d14abe8d63b6ee5708819/nextflow.config#L257)

  ```nextflow
  // Backwards compatibility for publishDir syntax
  ```
