# Nextflow lint results

- Generated: 2026-02-27T00:23:29.230052426Z
- Nextflow version: 26.01.1-edge
- Summary: 1 error, 16 warnings

## :x: Errors

- Error: `modules/nf-core/samtools/merge/main.nf:51:9`: `index` is already declared

  ```nextflow
      def index = args.contains("--write-index") ? "touch ${prefix}.${index_type}" : ""
          ^^^^^
  ```

## :warning: Warnings

- Warning: `modules/nf-core/bcftools/concat/main.nf:32:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input = vcfs.sort{it.toString()}.join(" ")
                            ^^
  ```

- Warning: `modules/nf-core/bcftools/convert/main.nf:87:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          hap = args_split.findIndexOf{ it == '--haplegendsample'}
                                        ^^
  ```

- Warning: `modules/nf-core/bcftools/index/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/bcftools/index/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/bcftools/merge/main.nf:27:58`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input = (vcfs.collect().size() > 1) ? vcfs.sort{ it.name } : vcfs
                                                           ^^
  ```

- Warning: `modules/nf-core/bcftools/norm/main.nf:56:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          if (['--write-index=tbi', '-W=tbi'].any { args.contains(it) }  && extension == 'vcf.gz') {
                                                                  ^^
  ```

- Warning: `modules/nf-core/bcftools/norm/main.nf:58:126`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          } else if (['--write-index=tbi', '-W=tbi', '--write-index=csi', '-W=csi', '--write-index', '-W'].any { args.contains(it) }) {
                                                                                                                               ^^
  ```

- Warning: `modules/nf-core/glimpse/chunk/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args    = task.ext.args   ?: ""
          ^^^^
  ```

- Warning: `modules/nf-core/glimpse/ligate/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args    = task.ext.args   ?: ""
          ^^^^
  ```

- Warning: `modules/nf-core/glimpse/phase/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args   ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/glimpse2/phase/main.nf:45:9`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          it.toString().endsWithAny("cram", "bam")          ? "bam" :
          ^^
  ```

- Warning: `modules/nf-core/glimpse2/phase/main.nf:46:9`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          it.toString().endsWithAny("vcf", "bcf", "vcf.gz") ? "gl"  :
          ^^
  ```

- Warning: `modules/nf-core/glimpse2/phase/main.nf:47:9`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          it.getExtension()
          ^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `workflows/phaseimpute/main.nf:240:63`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  VCF_NORMALIZE_BCFTOOLS.out.vcf_tbi.map{ meta, vcf, index -> [meta, [], []]}, // No scaffold
                                                                ^^^
  ```

- Warning: `workflows/phaseimpute/main.nf:240:68`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  VCF_NORMALIZE_BCFTOOLS.out.vcf_tbi.map{ meta, vcf, index -> [meta, [], []]}, // No scaffold
                                                                     ^^^^^
  ```
