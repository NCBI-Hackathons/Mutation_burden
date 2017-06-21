# Mutation_burden
Building a pipeline to assess effects of mutation burden based on tumor clonality. We will validate the clonality in pre-mixed cancer samples, separate the mutation burden based on segmented CNV calls, calculate clone-specific mutational burden and determine the potential benefit from immunotherapy treatment.

## Work Flow: 
1) Preprocessing: FASTQ files->BAM and VCF files
2) CNV calling: CNV variants 
3) Mutational burden calculation: SNV calculation per clone of cells (comparison among different tools)
4) Output: Appropriate for immunotherapy or not, which immunotherapy

Interval BED file for SureSelect Human All Exon V4 H. sapiens (hg19) is downloaded (S03723314). Recommended to use S03723314_AllTracks.bed which is uploaded at /gpfs/commons/projects/ncbi-nygc-hackathon/IntervalFiles.

## Related references:

CCLE paper:
http://www.nature.com/nature/journal/v483/n7391/full/nature11003.html#supplementary-information

Library construction for exam capture sequencing:
http://www.nature.com/nbt/journal/v27/n2/full/nbt.1523.html

## Clonality analysis tools:

ABSOLUTE
http://archive.broadinstitute.org/cancer/cga/sites/default/files/data/tools/absolute/ABSOLUTE_1.0.6.tar.gz

SEQUENZA
https://cran.r-project.org/web/packages/sequenza/index.html

FACETS
https://github.com/mskcc/facets

## List of CNV tools that might be used for variant calling:

EXCAVATOR
https://genomebiology.biomedcentral.com/articles/10.1186/gb-2013-14-10-r120

CONIFER
http://conifer.sourceforge.net/
download
http://conifer.sourceforge.net/download.html

CONTRA
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3348560/

ExomeCNV
https://academic.oup.com/bioinformatics/article/27/19/2648/231564/Exome-sequencing-based-copy-number-variation-and
download
https://cran.r-project.org/src/contrib/Archive/ExomeCNV/ (currently removed from cran, the link is archived versions)

