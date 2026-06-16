# Workflow outputs migration: riboseq

- Generated: 2026-06-16T14:30:50.746807+00:00
- Status: :x: **error** — no `output {}` block found; still relies on the legacy `publishDir` directive

This report tracks migration from the legacy `publishDir` directive to the new [workflow outputs](https://docs.seqera.io/nextflow/tutorials/workflow-outputs) syntax.

## Workflow `output {}` blocks

No top-level `output {}` block found. See the docs for how to add one:
https://docs.seqera.io/nextflow/tutorials/workflow-outputs

## Legacy `publishDir` references

Found 93 `publishDir` references that should be migrated to the workflow `output {}` block:

- [`conf/modules.config:18`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L18)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:29`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L29)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:41`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L41)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:50`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L50)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:62`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L62)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:74`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L74)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:82`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L82)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:90`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L90)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:99`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L99)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:107`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L107)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:115`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L115)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:124`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L124)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:133`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L133)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:147`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L147)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:154`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L154)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:165`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L165)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:173`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L173)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:181`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L181)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:189`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L189)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:203`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L203)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:213`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L213)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:223`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L223)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:233`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L233)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:248`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L248)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:270`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L270)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:297`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L297)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:307`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L307)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:322`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L322)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:343`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L343)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:360`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L360)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:376`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L376)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:385`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L385)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:402`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L402)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:414`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L414)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:422`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L422)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:445`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L445)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:463`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L463)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:473`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L473)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:481`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L481)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:492`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L492)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:501`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L501)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:509`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L509)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:530`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L530)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:547`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L547)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:556`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L556)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:584`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L584)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:607`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L607)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:615`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L615)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:624`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L624)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:633`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L633)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:641`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L641)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:651`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L651)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:659`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L659)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:668`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L668)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:677`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L677)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:685`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L685)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:697`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L697)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:702`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L702)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:738`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L738)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:756`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L756)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:766`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L766)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:778`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L778)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:788`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L788)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:805`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L805)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:814`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L814)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:824`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L824)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:833`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L833)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:843`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L843)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:857`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L857)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:863`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L863)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:868`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L868)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:878`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L878)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:890`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L890)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:898`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L898)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:906`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L906)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:918`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L918)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:948`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L948)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:957`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L957)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:976`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L976)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:988`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L988)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1002`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L1002)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1014`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L1014)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1025`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L1025)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:1028`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L1028)

  ```nextflow
  publishDir = [ enabled: false ]
  ```

- [`conf/modules.config:1033`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L1033)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1047`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L1047)

  ```nextflow
  publishDir = [
  ```

- [`conf/modules.config:1061`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/conf/modules.config#L1061)

  ```nextflow
  publishDir = [
  ```

- [`modules/nf-core/umitools/extract/tests/nextflow.config:3`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/modules/nf-core/umitools/extract/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`subworkflows/nf-core/fastq_align_star/tests/nextflow.config:3`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/subworkflows/nf-core/fastq_align_star/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config:3`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/subworkflows/nf-core/fastq_align_star/tests/with_transcripts.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```

- [`subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config:22`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config#L22)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config:29`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/subworkflows/nf-core/fastq_qc_trim_filter_setstrandedness/tests/nextflow.config#L29)

  ```nextflow
  publishDir = [
  ```

- [`subworkflows/nf-core/fastq_subsample_fq_salmon/tests/nextflow.config:3`](https://github.com/nf-core/riboseq/blob/bbcd3aef5937b936fdf811611774e339036e1dc3/subworkflows/nf-core/fastq_subsample_fq_salmon/tests/nextflow.config#L3)

  ```nextflow
  publishDir = { "${params.outdir}/${task.process.tokenize(':')[-1].tokenize('_')[0].toLowerCase()}" }
  ```
