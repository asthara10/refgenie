# Reference Genome Indexer (RefGenie) Recipes

## hg19

```
BUILDER=${CODEBASE}refgenie/src/refgenie.py
INPUT=http://hgdownload.cse.ucsc.edu/goldenPath/hg19/bigZips/hg19.2bit
GTF=ftp://ftp.sanger.ac.uk/pub/gencode/Gencode_human/release_19/gencode.v19.annotation.gtf.gz
${BUILDER} -i ${INPUT} -a ${GTF} -n hg19
```

## hg38
(use the NCBI's official version for sequence alignments without _alt sequences:)
```
INPUT=ftp://ftp.ncbi.nlm.nih.gov/genomes/all/GCA_000001405.15_GRCh38/seqs_for_alignment_pipelines.ucsc_ids/GCA_000001405.15_GRCh38_no_alt_analysis_set.fna.gz
GTF=ftp://ftp.sanger.ac.uk/pub/gencode/Gencode_human/release_23/gencode.v23.primary_assembly.annotation.gtf.gz
${BUILDER} -i ${INPUT} -a ${GTF} -n hg38
```
